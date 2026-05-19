# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required. Investigate missing trade reference MN17277022 in host systems.

**Reason:** The trade is missing in the HOST system (404 Not Found).

---

## 2. Email Summary

**Email ID:** email_092.eml  
**Subject:** Trade Confirmation Request – MN17277022  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** 2026-04-28T15:38:48+02:00  
**Counterparty:** ING Bank

The sender received a trade notification referencing MN17277022, but is unable to locate a matching record in their system. They ask to verify trade details and confirm whether the notification is a new trade or resubmission.

---

## 3. Classification
- **Primary Type:** generic_trade_details_request (originally generic_trade_details_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | MN17277022 | null | missing_in_host | high |
| security_name | ABB Ltd. | null | missing_in_host | medium |
| isin | null | null | missing_in_email | none |
| trade_date | 2025-11-11 | null | missing_in_host | high |
| settlement_date | 2025-11-12 | null | missing_in_host | high |
| quantity | 27666 | null | missing_in_host | high |
| amount | 532733.74 | null | missing_in_host | high |
| currency | USD | null | missing_in_host | high |
| side | sell | null | missing_in_host | medium |
| counterparty_name | ING Bank | null | missing_in_host | medium |
| reported_status | unknown | null | missing_in_host | none |

### Discrepancy Flags
- trade_not_found_on_host
- reference_number_unmatched
- missing_host_data
- escalate_to_human

---

## 6. Findings

HOST `/trades` lookup by reference_number returned 404 (no match). The email provides a single clear trade reference and parsed attachment, but the host system has no corresponding record. Because core fields (reference, dates, quantity, amount, currency) could not be confirmed on host, automated reconciliation confidence is low (0.15).

---

## 7. Next Steps

1. Search alternate/internal systems and audit logs for trade reference MN17277022.
2. Verify with operations desk and ING Bank (counterparty) using attached `trade_details.txt`.
3. If trade exists in a different system, reconcile identifiers (ISIN) and enter/route accordingly.
4. If this is a legitimate new trade, advise counterparty to re-submit and provide any missing identifiers.

---