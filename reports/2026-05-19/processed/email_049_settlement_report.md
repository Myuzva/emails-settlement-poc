# MAIA Settlement Mailbox Report - email_049.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing. HOST trade matches the email facts; inform requester that HOST status is Offen/open for trade NB77500740 and follow normal settlement-status response workflow.
**Reason:** Settlement-related status/action request with HOST lookup-ready trade reference.

---

## 2. Email Summary

**Email ID:** email_049  
**Subject:** Trade Exception – NB77500740  
**Sender:** John Smith <j.smith@globalcapital.com>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Macquarie Group

The sender requests settlement status/action guidance for the trade due to settle on 2026-03-19.

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
| reference_number | NB77500740 | NB77500740 | match | none |
| security_name | Volkswagen AG | Volkswagen AG | match | none |
| isin | null | DE0007664005 | missing_in_email | none |
| trade_date | 2026-03-18 | 2026-03-18 | match | none |
| settlement_date | 2026-03-19 | 2026-03-19 | match | none |
| side | sell | Verkauf | match | none |
| quantity | 88419 | 88419 | match | none |
| amount | 731551.03 | 731551.03 | match | none |
| currency | CHF | CHF | match | none |
| counterparty_name | Macquarie Group | Macquarie Group | match | none |
| counterparty_lei | null | KG1ELAF8FBU2GBW60X80 | missing_in_email | none |
| status | unknown | Offen | missing_in_email | none |

### Discrepancy Flags
- status_requested_host_status_offen

---

## 6. Recommended Action
- [x] Proceed with standard processing. HOST trade matches the email facts; inform requester that HOST status is Offen/open for trade NB77500740 and follow normal settlement-status response workflow.
- [ ] Respond to requester confirming trade is on track for settlement / no host discrepancies.

---

## 7. Draft Analyst Response Template
```text
Dear John Smith,

Thank you for your email regarding trade NB77500740 in Volkswagen AG.

We can confirm that trade NB77500740 (Sell 88,419 shares of Volkswagen AG) is currently marked as Open (Offen) in our system. All economic details match perfectly (Net Amount: CHF 731,551.03, Settlement Date: 2026-03-19). 

Please let us know if you require any further action or information to facilitate settlement.

Best regards,
Settlement Operations
```