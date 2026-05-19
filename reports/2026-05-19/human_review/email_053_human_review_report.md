# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review for manual processing.

**Reason:** The case was routed to human review due to an unsupported schema validation error during processing, and a high-severity trade date mismatch was identified during HOST reconciliation.

---

## 2. Email Summary

**Email ID:** email_053.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Merrill Lynch

The sender explicitly mentions a settlement date inconsistency, claiming the trade should have settled on 2026-03-20, but the booking reflects a different date.

---

## 3. Classification
- **Primary Type:** settlement_date_mismatch
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | KR86473518 | KR86473518 | match | none |
| security_isin | null | US0378331005 | missing_in_email | none |
| security_name | Apple Inc. | Apple Inc. | match | none |
| settlement_date | 2026-03-20 | 2026-03-20 | match | none |
| trade_date | 2026-03-26 | 2026-03-19 | mismatch | high |
| quantity | 85772 | 85772 | match | none |
| amount | 1549075.48 | 1549075.48 | match | none |
| currency | EUR | EUR | match | none |
| side | buy | buy | match | none |
| counterparty_name | Merrill Lynch | Merrill Lynch | match | none |
| status | closed | closed | match | none |

### Discrepancy Flags
- trade_date_mismatch

---

## 6. Findings

The trade was found in HOST and most details match perfectly, including the settlement date (2026-03-20) which aligns with the sender's expected date. However, there is a high-severity mismatch in the trade date: the email and its attachment report 2026-03-26, whereas the HOST system shows 2026-03-19. 

Additionally, the case payload was flagged with an `unsupported_schema` routing reason, requiring manual validation.

---

## 7. Next Steps

1. Investigate the trade date discrepancy (2026-03-26 vs 2026-03-19) against internal trade booking records.
2. Confirm with the counterparty if the trade date in their records is correct, noting that the settlement date in HOST already matches their expectation (2026-03-20).
3. Validate the case payload structure to resolve the unsupported schema issue.
4. Keep the case under analyst review until the discrepancy is resolved.
