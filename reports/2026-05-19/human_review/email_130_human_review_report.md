# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Human review required: investigate host systems for trade TW95561154 (search other reference fields and alternative booking systems). If not found, contact front office/back office to confirm whether trade was booked under a different reference or whether a new booking instruction should be raised and advise the counterparty accordingly.

**Reason:** The trade is missing in the HOST system (404 Not Found).

---

## 2. Email Summary

**Email ID:** email_130.eml  
**Subject:** Trade Confirmation Request – TW95561154  
**Sender:** Michael Hartmann <m.hartmann@eurofin.de>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Bank of America

Counterparty cannot find a corresponding booking and requests confirmation whether the trade is captured under another reference or needs a new booking instruction.

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
| reference_number | TW95561154 | null | missing_in_host | high |
| security_name | JPMorgan Chase & Co. | null | missing_in_host | medium |
| isin | null | null | missing_in_email | none |
| settlement_date | 2025-11-30 | null | missing_in_host | high |
| trade_date | 2025-11-29 | null | missing_in_host | high |
| quantity | 26244 | null | missing_in_host | high |
| amount | 1287754.02 | null | missing_in_host | high |
| currency | EUR | null | missing_in_host | high |
| side | buy | null | missing_in_host | high |
| counterparty_name | Bank of America | null | missing_in_host | high |
| reported_status | unknown | null | missing_in_host | medium |

### Discrepancy Flags
- trade_not_found_on_host
- reference_missing_on_host
- settlement_and_trade_dates_missing_on_host
- amount_and_quantity_missing_on_host

---

## 6. Findings

The trade TW95561154 was not found in the HOST system using the reference number provided in the email (Host returned 404 Not Found). The email extraction of trade fields is high confidence and complete, so absence on host likely indicates a missing booking or a different reference.

---

## 7. Next Steps

1. Investigate host systems for trade TW95561154 (search other reference fields and alternative booking systems).
2. If not found, contact front office/back office to confirm whether trade was booked under a different reference or whether a new booking instruction should be raised.
3. Advise the counterparty accordingly.
4. Keep the case under analyst review until the discrepancy is resolved.

---
