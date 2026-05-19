# MAIA Settlement Mailbox Report - email_109.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Standard  
**Recommended Action:** Proceed with standard processing for the missing confirmation request. HOST trade was found and reconciles to the email facts; provide or request the final trade confirmation or SWIFT confirmation according to the standard workflow.  
**Reason:** Email explicitly requests final trade confirmation or SWIFT confirmation for a settled trade. Single trade reference and complete trade details are present.

---

## 2. Email Summary

**Email ID:** email_109.eml  
**Subject:** Trade Exception – WB08756919  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** UBS

The sender requests final trade confirmation or SWIFT confirmation as settlement evidence for a closed settled trade.

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
| reference_number | WB08756919 | WB08756919 | match | none |
| security_isin | null | CH0012032048 | missing_in_email | none |
| security_name | Roche Holding AG | Roche Holding AG | match | none |
| settlement_date | 2026-03-04 | 2026-03-04 | match | none |
| trade_date | 2026-03-03 | 2026-03-03 | match | none |
| quantity | 79390 | 79390 | match | none |
| amount | 515644.54 | 515644.54 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty_name | UBS | UBS | match | none |
| counterparty_lei | null | BFM8T61CT2L1QCEMIK50 | missing_in_email | none |
| status | settled | Closed | match | none |

### Discrepancy Flags
- missing_confirmation_requested

---

## 6. Recommended Action
- [x] Proceed with standard processing for the missing confirmation request. HOST trade was found and reconciles to the email facts.
- [ ] Provide the final trade confirmation or SWIFT confirmation to the sender.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email regarding trade WB08756919.

We can confirm that the trade (Sale 79,390 shares of Roche Holding AG) is recorded as Closed/Settled in our system, matching your records. 

Please find attached the requested final trade confirmation / SWIFT confirmation for your reference.

Best regards,
Settlement Operations
```