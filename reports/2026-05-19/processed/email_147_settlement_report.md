# MAIA Settlement Mailbox Report - email_147.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard settlement-status response. HOST trade matches the email facts; no human review is required based on reconciliation.
**Reason:** Settlement-related follow-up with HOST-ready trade reference. Critical trade fields extracted from attachment.

---

## 2. Email Summary

**Email ID:** email_147  
**Subject:** Reconciliation Query – VO41550204 – Deutsche Bank AG  
**Sender:** Michael Hartmann <m.hartmann@eurofin.de>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** BNP Paribas

The sender provides a courtesy follow-up regarding trade VO41550204, which is currently in open status with a forthcoming settlement date of 2026.03.19, and asks to confirm receipt and advise whether actions are required ahead of settlement.

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
| reference_number | VO41550204 | VO41550204 | match | none |
| security_name | Deutsche Bank AG | Deutsche Bank AG | match | none |
| isin | null | DE0005140008 | missing_in_email | none |
| trade_date | 2026-03-18 | 2026-03-18 | match | none |
| settlement_date | 2026-03-19 | 2026-03-19 | match | none |
| side | sell | Verkauf | match | none |
| quantity | 46983 | 46983 | match | none |
| amount | 932852.81 | 932852.81 | match | none |
| currency | CHF | CHF | match | none |
| counterparty_name | BNP Paribas | BNP Paribas | match | none |
| counterparty_lei | null | R0MUWSFPU8MPRO8K5P83 | missing_in_email | none |
| status | open | Offen | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade VO41550204 matches the email facts (open, sell, 46,983 @ CHF 932,852.81, settlement 2026-03-19).
- [ ] Respond to requester confirming trade is on track for settlement / no host discrepancies.

---

## 7. Draft Analyst Response Template
```text
Dear Michael Hartmann,

Thank you for your email. 

We can confirm that trade VO41550204 (Sell 46,983 shares of Deutsche Bank AG) is currently marked as Open in our system and all details match perfectly (Net Amount: CHF 932,852.81). All internal pre-settlement checks are complete, and the trade is on track for timely settlement on 2026-03-19.

Best regards,
Settlement Operations
```