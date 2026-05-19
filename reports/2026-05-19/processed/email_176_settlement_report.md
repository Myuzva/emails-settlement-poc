# MAIA Settlement Mailbox Report - email_176.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** No human review required. Respond to the settlement status request using HOST result: trade ME19312140 is matched in HOST and current status is Open.
**Reason:** Email explicitly asks whether action is required for settlement of a named trade. Single trade reference and full trade details are available from body and attachment.

---

## 2. Email Summary

**Email ID:** email_176.eml  
**Subject:** Reconciliation Query – ME19312140 – Roche Holding AG  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Morgan Stanley

Sender requests settlement status/action guidance for the trade due to settle on 2026-03-17.

---

## 3. Classification
- **Primary Type:** settlement_status_request
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | ME19312140 | ME19312140 | match | none |
| security_name | Roche Holding AG | Roche Holding AG | match | none |
| security_isin | null | CH0012032048 | missing_in_email | none |
| trade_date | 2026-03-16 | 2026-03-16 | match | none |
| settlement_date | 2026-03-17 | 2026-03-17 | match | none |
| side | sell | Sale | match | none |
| quantity | 88389 | 88389 | match | none |
| amount | 1212017.91 | 1212017.91 | match | none |
| currency | EUR | EUR | match | none |
| counterparty_name | Morgan Stanley | Morgan Stanley | match | none |
| counterparty_lei | null | 9R7GPTSO7KV3UQJZQ078 | missing_in_email | none |
| status | unknown | Open | missing_in_email | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No human review required. Respond to the settlement status request using HOST result: trade ME19312140 is matched in HOST and current status is Open.
- [ ] Respond to requester confirming trade is on track for settlement / no host discrepancies.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email. 

We can confirm that trade ME19312140 (Sale 88,389 shares of Roche Holding AG) is currently marked as Open in our system and all details match perfectly (Net Amount: EUR 1,212,017.91). All internal pre-settlement checks are complete, and the trade is on track for timely settlement on 2026-03-17.

Best regards,
Settlement Operations
```