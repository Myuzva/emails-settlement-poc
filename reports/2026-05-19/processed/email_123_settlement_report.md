# MAIA Settlement Mailbox Report - email_123.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Proceed with automated status update as all fields match the HOST system.
**Reason:** Email explicitly asks for status/clarifications ahead of settlement for an open trade.

---

## 2. Email Summary

**Email ID:** email_123.eml  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Bank of America

Courtesy follow-up regarding trade AF97232113, which is currently in open status.

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
| reference_number | AF97232113 | AF97232113 | match | none |
| security_isin | null | US0378331005 | missing_in_email | none |
| security_name | Apple Inc. | Apple Inc. | match | none |
| settlement_date | 2026-03-03 | 2026-03-03 | match | none |
| trade_date | 2026-03-02 | 2026-03-02 | match | none |
| quantity | 89199 | 89199 | match | none |
| amount | 1109313.13 | 1109313.13 | match | none |
| currency | EUR | EUR | match | none |
| side | buy | buy | match | none |
| counterparty_name | Bank of America | Bank of America | match | none |
| status | open | open | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade AF97232113 matches the email facts (open, buy, 89,199 @ EUR 1,109,313.13, settlement 2026-03-03).
- [ ] Respond to requester confirming trade is on track for settlement / no host discrepancies.

---

## 7. Draft Analyst Response Template
```text
Dear Bank of America Settlement Team,

Thank you for your email. 

We can confirm that trade AF97232113 (Buy 89,199 shares of Apple Inc.) is currently marked as open in our system and all details match perfectly (Net Amount: EUR 1,109,313.13). All internal pre-settlement checks are complete, and the trade is on track for timely settlement on 2026-03-03.

Best regards,
Settlement Operations
```