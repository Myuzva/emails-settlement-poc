# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review.

**Reason:** Human review required due to unsupported schema.

---

## 2. Email Summary

**Email ID:** email_137.eml  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** JP Morgan

The counterparty reports a settlement date mismatch. Internal booking reflects 19-Mar-2026, whereas the instruction received indicates 27-Apr-2026.

---

## 3. Classification
- **Primary Type:** settlement_date_mismatch
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** SL99789329 (JP Morgan, Apple Inc., CHF 1795415.75)

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | SL99789329 | N/A | N/A | N/A |
| security_isin | null | N/A | N/A | N/A |
| security_name | Apple Inc. | N/A | N/A | N/A |
| settlement_date | 2026-04-27 | N/A | N/A | N/A |
| trade_date | 2026-03-18 | N/A | N/A | N/A |
| quantity | 84028 | N/A | N/A | N/A |
| amount | 1795415.75 | N/A | N/A | N/A |
| currency | CHF | N/A | N/A | N/A |
| side | sell | N/A | N/A | N/A |
| counterparty_name | JP Morgan | N/A | N/A | N/A |
| status | unknown | N/A | N/A | N/A |

### Discrepancy Flags
- Settlement date mismatch: Sender value 2026-03-19 vs Expected 2026-04-27.

---

## 6. Findings

The email explicitly states a value date mismatch on trade SL99789329. The internal booking reflects 19-Mar-2026, whereas the instruction received indicates 27-Apr-2026. The case requires human review due to an unsupported schema.

---

## 7. Next Steps

1. Review the unsupported schema issue.
2. Verify the correct settlement date against internal trade booking records.
3. Confirm the expected settlement date with the counterparty.
4. Keep the case under analyst review until the discrepancy is resolved.

---
