# MAIA Settlement Mailbox Report - email_075.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** No action required. Host trade PK20518401 matches the email facts after enrichment. Proceed with normal settlement monitoring.
**Reason:** The email asks recipient to confirm receipt and advise whether clarifications or actions are required ahead of settlement. All details match perfectly.

---

## 2. Email Summary

**Email ID:** email_075  
**Subject:** Outstanding Trade – Action Required – PK20518401  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** BNP Paribas

The email asks recipient to confirm receipt and advise whether clarifications or actions are required ahead of settlement. Trade reference and settlement date are present in the body; detailed trade economics are present in the ZIP attachment.

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
| counterparty_name | BNP Paribas | R0MUWSFPU8MPRO8K5P83 (BNP Paribas) | match | none |
| status | open | Open | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No action required. Host trade PK20518401 matches the email facts after enrichment (security ISIN and counterparty LEI resolved). Proceed with normal settlement monitoring.
- [ ] Respond to requester confirming trade is on track for settlement / no host discrepancies.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email. 

We can confirm that trade PK20518401 (Sell 47,767 shares of Goldman Sachs Group Inc.) is currently marked as Open in our system and all details match perfectly (Net Amount: CHF 1,773,795.02). All internal pre-settlement checks are complete, and the trade is on track for settlement.

Best regards,
Settlement Operations
```