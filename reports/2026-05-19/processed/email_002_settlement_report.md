# MAIA Settlement Mailbox Report - email_002.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Provide the missing trade details (ISIN, dates, and counterparty) to the sender as requested, as the HOST record matches all provided information.  
**Reason:** Email asks recipient to supply missing trade details so records can be reconciled and archived.

---

## 2. Email Summary

**Email ID:** email_002.eml  
**Subject:** Outstanding Trade – Action Required – XJ02184853  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Santander  

The sender states the trade record is incomplete and requests missing details for reconciliation/archive.

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
| security_isin | null | CH0244767585 | missing_in_email | none |
| security_name | UBS Group AG | UBS Group AG | match | none |
| settlement_date | null | 2026-03-20 | missing_in_email | none |
| trade_date | null | 2026-03-19 | missing_in_email | none |
| quantity | 29837 | 29837 | match | none |
| amount | 1666712.84 | 1666712.84 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | sell | match | none |
| counterparty_name | null | Santander | missing_in_email | none |
| status | closed | closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade XJ02184853 matches the email facts (closed, sell, 29,837 @ EUR 1,666,712.84).
- [x] Respond to requester providing the missing trade details (ISIN: CH0244767585, Trade Date: 2026-03-19, Settlement Date: 2026-03-20, Counterparty: Santander).

---

## 7. Draft Analyst Response Template
```text
Dear Sender,

Thank you for your email regarding trade XJ02184853.

We have reviewed our records and can confirm that the trade is marked as closed in our system. As requested for your post-settlement audit and archiving, please find the missing details below:
- ISIN: CH0244767585
- Trade Date: 2026-03-19
- Settlement Date: 2026-03-20
- Counterparty: Santander

Please let us know if you require any further information.

Best regards,
Settlement Operations
```