# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Investigate the missing trade record. The counterparty (Morgan Stanley) reports having no record of trade PH61323120, and the trade cannot be found in the internal HOST system using either the reference number or the provided trade details.

**Reason:** Trade PH61323120 is missing from HOST. This matches the counterparty's claim of having no record, but prevents automated reconciliation or confirmation.

---

## 2. Email Summary

**Email ID:** email_166  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Morgan Stanley

Sender states they have no record of the trade and asks for confirmation of details.

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
| reference_number | PH61323120 | null | missing_in_host | high |
| security_name | BASF SE | null | missing_in_host | high |
| isin | null | null | unknown | none |
| trade_date | 2026-01-25 | null | missing_in_host | medium |
| settlement_date | 2026-01-26 | null | missing_in_host | high |
| quantity | 24489 | null | missing_in_host | high |
| amount | 189842.96 | null | missing_in_host | high |
| currency | CHF | null | missing_in_host | high |
| side | sell | null | missing_in_host | high |
| counterparty_name | Morgan Stanley | null | missing_in_host | high |

### Discrepancy Flags
- trade_not_found_in_host

---

## 6. Findings

The trade PH61323120 was not found in the HOST system. The counterparty (Morgan Stanley) also reports having no record of this trade. The missing trade prevents automated reconciliation or confirmation.

---

## 7. Next Steps

1. Investigate internal systems to determine why trade PH61323120 is missing from HOST.
2. Verify if the trade was booked under a different reference number or if it failed to book.
3. Communicate with the counterparty (Morgan Stanley) once the internal status of the trade is clarified.
4. Keep the case under analyst review until the missing trade is resolved.

---