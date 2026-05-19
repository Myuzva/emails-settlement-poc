# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Human review required to resolve settlement date mismatch.

**Reason:** HOST reflects 2026-03-19 (matching the sender's internal booking claim), while the instruction/extracted fact indicates 2026-04-27.

---

## 2. Email Summary

**Email ID:** email_137  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** JP Morgan

The counterparty reports a value date mismatch on trade SL99789329. Internal booking reflects 19-Mar-2026, whereas the instruction received indicates 27-Apr-2026.

---

## 3. Classification
- **Primary Type:** wrong_date (originally settlement_date_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | SL99789329 | SL99789329 | match | none |
| security_isin | null | US0378331005 | missing_in_email | none |
| security_name | Apple Inc. | Apple Inc. | match | none |
| settlement_date | 2026-04-27 | 2026-03-19 | mismatch | high |
| trade_date | 2026-03-18 | 2026-03-18 | match | none |
| quantity | 84028 | 84028 | match | none |
| amount | 1795415.75 | 1795415.75 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | sell | match | none |
| counterparty_name | JP Morgan | JP Morgan | match | none |
| status | unknown | Offen | missing_in_email | none |

### Discrepancy Flags
- settlement_date_mismatch

---

## 6. Findings

The trade was found in HOST, but the settlement date differs from the counterparty’s email instruction.

The likely cause of the settlement break is a settlement date mismatch. The case should be reviewed before any confirmation is sent externally.

---

## 7. Next Steps

1. Verify the correct settlement date against internal trade booking records.

2. Confirm whether the counterparty is referencing the same trade reference.

3. Ask the counterparty to confirm the expected settlement date.

4. Keep the case under analyst review until the discrepancy is resolved.

---