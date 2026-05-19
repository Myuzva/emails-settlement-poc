# MAIA Settlement Mailbox Report - email_109.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Provide the requested final trade confirmation / SWIFT confirmation to the counterparty (WB08756919). If unable to locate the confirmation, escalate to operations/back-office for retrieval and provide evidence to the sender.
**Reason:** Sender requests final trade confirmation or SWIFT confirmation as settlement evidence for a settled closed trade.

---

## 2. Email Summary

**Email ID:** email_109.eml  
**Subject:** Trade Exception – WB08756919  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** UBS

Counterparty requests final trade confirmation or SWIFT confirmation for quarter-end settlement evidence.

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
| security | Roche Holding AG | CH0012032048 | match | none |
| trade_date | 2026-03-03 | 2026-03-03 | match | none |
| settlement_date | 2026-03-04 | 2026-03-04 | match | none |
| side | sell | Sale | match | none |
| quantity | 79390 | 79390 | match | none |
| amount | 515644.54 | 515644.54 | match | none |
| currency | EUR | EUR | match | none |
| counterparty | UBS | BFM8T61CT2L1QCEMIK50 (resolved to UBS) | match | none |
| status | settled | Closed | match | low |

### Discrepancy Flags
- missing_confirmation
- security_identifier_type_difference
- status_label_difference

---

## 6. Recommended Action
- [x] Provide the requested final trade confirmation / SWIFT confirmation to the counterparty (WB08756919).
- [ ] If unable to locate the confirmation, escalate to operations/back-office for retrieval and provide evidence to the sender.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email regarding trade WB08756919.

We confirm that the trade for 79,390 shares of Roche Holding AG (Net Amount: EUR 515,644.54) is recorded as Closed/Settled in our system. 

Please find attached the requested final trade confirmation / SWIFT confirmation for your audit evidence.

Best regards,
Settlement Operations
```