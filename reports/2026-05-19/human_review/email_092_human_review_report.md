# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Investigate why the trade (Ref: MN17277022) is missing from the host system.

**Reason:** The trade reference MN17277022 was not found in the host system. The counterparty reports they cannot locate the record, and a search by trade details in the host system also returned no match.

---

## 2. Email Summary

**Email ID:** email_092  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** ING Bank

The counterparty reports a missing confirmation and states they are unable to locate a matching record in their system.

---

## 3. Classification
- **Primary Type:** missing_confirmation (originally confirmation_missing)
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
| security_isin | null | CH0012530207 | missing_in_email | none |
| security_name | ABB Ltd. | ABB Ltd. | match | none |
| counterparty_name | ING Bank | ING Bank | match | none |
| settlement_date | 2025-11-12 | null | missing_in_host | high |
| trade_date | 2025-11-11 | null | missing_in_host | high |
| quantity | 27666 | null | missing_in_host | high |
| amount | 532733.74 | null | missing_in_host | high |
| currency | USD | null | missing_in_host | high |
| side | sell | null | missing_in_host | high |

### Discrepancy Flags
- trade_not_found_in_host

---

## 6. Findings

The trade was not found in the host system. A search by trade details (Mode B) returned a 404 Not Found response. Security and counterparty identifiers were successfully resolved, confirming the search parameters were accurate.

---

## 7. Next Steps

1. Investigate why the trade (Ref: MN17277022) is missing from the host system.
2. Verify internal trade booking records for any unbooked or failed trades matching the provided details.
3. Keep the case under analyst review until the discrepancy is resolved.

---