# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Investigate missing trade. The trade referenced in the email (EP95329750) was not found in the HOST system by reference number or by field combination.

**Reason:** Trade not found in HOST system despite being reported as 'closed' in external documentation mentioned by the sender.

---

## 2. Email Summary

**Email ID:** email_062.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Santander

Sender states they have no record of the trade and asks for advice on whether it was booked under an alternative reference.

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
| reference_number | EP95329750 | null | missing_in_host | high |
| security_isin | null | CH0012221716 | missing_in_email | none |
| security_name | Novartis AG | Novartis AG | match | none |
| settlement_date | 2026-01-28 | null | missing_in_host | high |
| trade_date | 2026-01-27 | null | missing_in_host | high |
| quantity | 20185 | null | missing_in_host | high |
| amount | 612506.76 | null | missing_in_host | high |
| currency | EUR | null | missing_in_host | high |
| side | sell | null | missing_in_host | high |
| counterparty_name | Santander | Santander | match | none |
| status | closed | null | missing_in_host | high |

### Discrepancy Flags
- trade_not_found_in_host
- missing_confirmation

---

## 6. Findings

The trade referenced in the email (EP95329750) was not found in the HOST system by reference number or by field combination (Settlement Date, ISIN, Quantity, Amount, Currency).
The sender states they have no record of the trade in their system despite it appearing in external documentation as closed.

---

## 7. Next Steps

1. Investigate internal systems to determine if trade EP95329750 was booked under an alternative reference.
2. Verify the trade details (Novartis AG, Sell, 20,185 @ EUR 612,506.76, Settlement 2026-01-28) against other internal booking records.
3. Contact the counterparty (Santander) to clarify the external documentation they are referencing.
4. Keep the case under analyst review until the missing trade discrepancy is resolved.

---
