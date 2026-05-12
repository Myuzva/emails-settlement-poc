# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Investigate settlement date discrepancy. Host confirms 2026-03-05, which matches the sender's internal booking but contradicts the instruction date 2026-02-19.

**Reason:** The sender explicitly states a value date mismatch, with their internal booking reflecting 05-Mar-2026 and the instruction indicating 19-Feb-2026.

---

## 2. Email Summary

**Email ID:** email_105.eml  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Raiffeisen Bank

Email reports a settlement date mismatch for trade MU50046625. Trade details extracted from attached ZIP containing a PDF.

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
| reference_number | MU50046625 | MU50046625 | match | none |
| security_isin | null | US5949181045 | missing_in_email | none |
| security_name | Microsoft Corp. | Microsoft Corp. | match | none |
| settlement_date | 2026-02-19 | 2026-03-05 | mismatch | high |
| trade_date | 2026-03-04 | 2026-03-04 | match | none |
| quantity | 63414 | 63414 | match | none |
| amount | 157516.59 | 157516.59 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | sell | match | none |
| counterparty_name | Raiffeisen Bank | Raiffeisen Bank | match | none |
| status | pending | pending | match | none |

### Discrepancy Flags
- settlement_date_mismatch

---

## 6. Findings

The trade was found in HOST, but the settlement date differs from the instruction date in the email.

The likely cause of the settlement break is a settlement date mismatch. Host confirms 2026-03-05, which matches the sender's internal booking but contradicts the instruction date 2026-02-19. The case should be reviewed before any confirmation is sent externally.

---

## 7. Next Steps

1. Verify the correct settlement date against internal trade booking records.

2. Confirm whether the counterparty is referencing the same trade reference.

3. Ask the counterparty to confirm the expected settlement date.

4. Keep the case under analyst review until the discrepancy is resolved.

---