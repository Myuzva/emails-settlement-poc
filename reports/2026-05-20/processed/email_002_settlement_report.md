# MAIA Settlement Mailbox Report - email_002.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Record from HOST can be used to update internal trade record: populate ISIN (CH0244767585), settlement date (2026-03-20) and trade date (2026-03-19), and store counterparty LEI. No obvious substantive mismatches. Because the email is a request for missing information, reply to counterparty confirming the HOST values and ask them to confirm any further details if needed.
**Reason:** Email asks counterparty to supply missing trade details for reconciliation/archive.

---

## 2. Email Summary

**Email ID:** email_002  
**Subject:** Outstanding Trade – Action Required – XJ02184853  
**Sender:** John Smith <j.smith@globalcapital.com>  
**Received:** 2026-04-28T15:38:47+02:00  
**Counterparty:** Santander

Sender states the trade record is incomplete and requests missing details for reconciliation and archiving.

---

## 3. Classification
- **Primary Type:** generic_trade_details_request
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
| counterparty_name | Santander | Santander (LEI: 5UMCZOEYKCVFAW8ZLO05) | match | none |
| counterparty_lei | null | 5UMCZOEYKCVFAW8ZLO05 | missing_in_email | none |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- missing_settlement_date_in_email
- missing_trade_date_in_email
- missing_isin_in_email
- host_uses_LEI_for_counterparty
- language_label_difference_host_vs_email

---

## 6. Recommended Action
- [x] Record from HOST can be used to update internal trade record: populate ISIN (CH0244767585), settlement date (2026-03-20) and trade date (2026-03-19), and store counterparty LEI.
- [x] No obvious substantive mismatches.
- [x] Because the email is a request for missing information, reply to counterparty confirming the HOST values and ask them to confirm any further details if needed.

---

## 7. Draft Analyst Response Template
```text
Dear John Smith,

Thank you for your email regarding trade XJ02184853.

We can confirm the following missing details from our records to assist with your reconciliation:
- ISIN: CH0244767585
- Trade Date: 2026-03-19
- Settlement Date: 2026-03-20
- Counterparty LEI: 5UMCZOEYKCVFAW8ZLO05

Please let us know if you need any further information to complete your archiving.

Best regards,
Settlement Operations
```