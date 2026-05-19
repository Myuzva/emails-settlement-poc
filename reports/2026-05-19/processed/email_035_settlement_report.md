# MAIA Settlement Mailbox Report - email_035.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Host trade found and key fields match. Request and attach the final trade confirmation or SWIFT message from Deutsche Bank per sender request. No immediate human review required; escalate to operations if confirmation cannot be provided.
**Reason:** Single exact trade match by reference number returned from HOST. All critical numeric and date fields match exactly or within tolerance.

---

## 2. Email Summary

**Email ID:** email_035  
**Subject:** Trade Exception – AH16220994  
**Sender:** Sarah Jensen <s.jensen@nordbank.com>  
**Received:** Tue, 28 Apr 2026 15:38:47 +0200  
**Counterparty:** Deutsche Bank

Sender requests final trade confirmation or SWIFT confirmation as settlement evidence for a settled closed trade.

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
| reference_number | AH16220994 | AH16220994 | match | none |
| security_isin | null | US5949181045 | missing_in_email | none |
| security_name | Microsoft Corp. | Microsoft Corp. | match | none |
| settlement_date | 2026-03-26 | 2026-03-26 | match | none |
| trade_date | 2026-03-25 | 2026-03-25 | match | none |
| quantity | 21668 | 21668 | match | none |
| amount | 1988835.46 | 1988835.46 | match | none |
| currency | USD | USD | match | none |
| side | sell | Sale | match | none |
| counterparty_name | Deutsche Bank | Deutsche Bank | match | none |
| status | settled | Closed | match | low |

### Discrepancy Flags
- missing_confirmation_requested
- security_isin_missing_in_email
- status_label_difference_closed_vs_settled

---

## 6. Recommended Action
- [x] Host trade found and key fields match. Request and attach the final trade confirmation or SWIFT message from Deutsche Bank per sender request.
- [ ] No immediate human review required; escalate to operations if confirmation cannot be provided.

---

## 7. Draft Analyst Response Template
```text
Dear Sarah Jensen,

Thank you for your email regarding trade AH16220994.

We have verified the trade details in our system and confirm that the trade is marked as Closed/Settled. As requested, please find attached the final trade confirmation / SWIFT confirmation for your records.

Best regards,
Settlement Operations
```