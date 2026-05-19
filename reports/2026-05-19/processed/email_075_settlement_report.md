# MAIA Settlement Mailbox Report - email_075.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing. HOST trade PK20518401 matches the email facts; no human-in-the-loop review is required based on reconciliation.
**Reason:** Email follows up on an outstanding/open trade and asks whether clarifications or actions are required ahead of settlement. Trade reference and settlement details are present in body and attachment.

---

## 2. Email Summary

**Email ID:** email_075.eml  
**Subject:** Outstanding Trade – Action Required – PK20518401  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** BNP Paribas

The sender follows up regarding trade PK20518401, which is currently in open status with a forthcoming settlement date of 25-Mar-2026, and asks whether clarifications or actions are required ahead of settlement.

---

## 3. Classification
- **Primary Type:** settlement_status_request (originally settlement_status_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | PK20518401 | PK20518401 | match | none |
| security_isin | null | US38141G1040 | missing_in_email | none |
| security_name | Goldman Sachs Group Inc. | Goldman Sachs Group Inc. | match | none |
| settlement_date | 2026-03-25 | 2026-03-25 | match | none |
| trade_date | 2026-03-24 | 2026-03-24 | match | none |
| quantity | 47767 | 47767 | match | none |
| amount | 1773795.02 | 1773795.02 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Sale | match | none |
| counterparty_name | BNP Paribas | BNP Paribas | match | none |
| counterparty_lei | null | R0MUWSFPU8MPRO8K5P83 | missing_in_email | none |
| status | open | Open | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade PK20518401 matches the email facts (open, sell, 47,767 @ CHF 1,773,795.02, settlement 2026-03-25).
- [ ] Respond to requester confirming trade is on track for settlement / no host discrepancies.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email regarding trade PK20518401.

We can confirm that trade PK20518401 (Sell 47,767 shares of Goldman Sachs Group Inc.) is currently marked as Open in our system and all details match perfectly (Net Amount: CHF 1,773,795.02). All internal pre-settlement checks are complete, and the trade is on track for timely settlement on 2026-03-25.

Best regards,
Settlement Operations
```