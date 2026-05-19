# MAIA Settlement Mailbox Report - email_002.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing. HOST contains a single matching trade for reference XJ02184853; provided economics, side, security, counterparty, currency, quantity, amount, and status reconcile after safe normalization/enrichment. Missing email trade date, settlement date, ISIN, and counterparty LEI can be supplied from HOST if needed for the trade-details request.
**Reason:** Single trade reference is available for HOST lookup. Body requests missing trade details for a post-settlement audit and attachment provides a single trade reference with trade economics.

---

## 2. Email Summary

**Email ID:** email_002.eml  
**Subject:** Outstanding Trade – Action Required – XJ02184853  
**Sender:** John Smith <j.smith@globalcapital.com>  
**Received:** Tue, 28 Apr 2026 15:38:47 +0200  
**Counterparty:** Santander  

Sender states the post-settlement audit found the trade record incomplete and requests missing details to reconcile and archive records.

---

## 3. Classification
- **Primary Type:** generic_trade_details_request (originally generic_trade_details_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | XJ02184853 | XJ02184853 | match | none |
| security_name | UBS Group AG | UBS Group AG | match | none |
| isin | null | CH0244767585 | missing_in_email | none |
| settlement_date | null | 2026-03-20 | missing_in_email | low |
| trade_date | null | 2026-03-19 | missing_in_email | low |
| side | sell | Verkauf | match | none |
| quantity | 29837 | 29837 | match | none |
| amount | 1666712.84 | 1666712.84 | match | none |
| currency | EUR | EUR | match | none |
| counterparty_name | Santander | Santander | match | none |
| counterparty_lei | null | 5UMCZOEYKCVFAW8ZLO05 | missing_in_email | low |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade XJ02184853 matches the email facts (closed, sell, 29,837 @ EUR 1,666,712.84).
- [ ] Respond to requester providing the missing trade details (ISIN: CH0244767585, Trade Date: 2026-03-19, Settlement Date: 2026-03-20, Counterparty LEI: 5UMCZOEYKCVFAW8ZLO05) to complete their post-settlement audit.

---

## 7. Draft Analyst Response Template
```text
Dear John Smith,

Thank you for your email regarding the post-settlement audit for trade XJ02184853.

We can confirm that the trade is marked as Closed in our system and the economics match your records (Sell 29,837 shares of UBS Group AG, Net Amount: EUR 1,666,712.84). 

To assist with completing your trade record, please find the missing details below:
- ISIN: CH0244767585
- Trade Date: 2026-03-19
- Settlement Date: 2026-03-20
- Counterparty LEI: 5UMCZOEYKCVFAW8ZLO05

Please let us know if you require any further information to reconcile and archive your records.

Best regards,
Settlement Operations
```