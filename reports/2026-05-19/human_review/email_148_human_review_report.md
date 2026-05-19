# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Host returned no matching trade for reference IP36951687 (404). Human review required: contact sender to confirm whether this is a new trade to be booked or a re-submission with a different reference; if new booking, create trade in host system using provided details; if a re-submission, request correct/alternate reference or provide host-facing identifiers. Record outcome and re-run lookup after corrective info is obtained.

**Reason:** Host lookup by trade reference returned 404 (no match). Email explicitly requests verification of whether this is a new booking or a resubmission; human decision needed.

---

## 2. Email Summary

**Email ID:** email_148.eml  
**Subject:** Trade Exception – IP36951687  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Citigroup

The sender says they cannot locate a matching record for the referenced trade notification and requests verification of trade details and whether it is a new booking or resubmission.

---

## 3. Classification
- **Primary Type:** generic_trade_details_request
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | IP36951687 | null | missing_in_host | high |
| security_name | Roche Holding AG | null | missing_in_host | medium |
| isin | null | null | missing_in_host | none |
| trade_date | 2025-12-22 | null | missing_in_host | high |
| settlement_date | 2025-12-23 | null | missing_in_host | high |
| quantity | 98076 | null | missing_in_host | high |
| amount | 1538459.01 | null | missing_in_host | high |
| currency | EUR | null | missing_in_host | high |
| side | buy | null | missing_in_host | medium |
| counterparty_name | Citigroup | null | missing_in_host | high |
| reported_status | unknown | null | missing_in_host | none |

### Discrepancy Flags
- no_host_match
- reference_not_found
- requires_manual_booking_decision

---

## 6. Findings

The trade was not found in HOST (404 Not Found). The email explicitly requests verification of whether this is a new booking or a resubmission. No host-side data is available to confirm or reconcile fields; manual intervention is required.

---

## 7. Next Steps

1. Contact the sender to confirm whether this is a new trade to be booked or a re-submission with a different reference.
2. If it is a new booking, create the trade in the host system using the provided details.
3. If it is a re-submission, request the correct/alternate reference or provide host-facing identifiers.
4. Record the outcome and re-run the lookup after corrective info is obtained.

---
