# MAIA Settlement Mailbox Report - email_002.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Provide the missing trade details (Trade Date: 2026-03-19, Settlement Date: 2026-03-20, ISIN: CH0244767585) to the sender as requested to complete their records.
**Reason:** Sender asks for missing trade details to reconcile an incomplete post-settlement trade record. Single trade reference is identified in subject/body and attachment. No specific mismatch, missing confirmation, missing affirmation, or failed settlement claim is stated.

---

## 2. Email Summary

**Email ID:** email_002  
**Subject:** Outstanding Trade – Action Required – XJ02184853  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Santander

Sender reports the trade record is incomplete and requests missing details for reconciliation and archiving.

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
| trade_date | null | 2026-03-19 | missing_in_email | none |
| settlement_date | null | 2026-03-20 | missing_in_email | none |
| quantity | 29837 | 29837 | match | none |
| amount | 1666712.84 | 1666712.84 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | sell | match | none |
| counterparty_name | Santander | Santander | match | none |
| status | closed | closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] Trade successfully located using reference number XJ02184853.
- [x] All provided email facts (quantity, amount, currency, side, counterparty, security name) match the HOST record exactly.
- [x] Security ISIN (CH0244767585) and Counterparty LEI (5UMCZOEYKCVFAW8ZLO05) were verified via enrichment endpoints to match the names provided in the email.
- [ ] Provide the missing trade details (Trade Date: 2026-03-19, Settlement Date: 2026-03-20, ISIN: CH0244767585) to the sender as requested to complete their records.

---

## 7. Draft Analyst Response Template
```text
Dear Santander Settlement Team,

Thank you for your email regarding trade XJ02184853.

We have reviewed our records and can confirm the following missing details for your post-settlement audit:
- Trade Date: 2026-03-19
- Settlement Date: 2026-03-20
- ISIN: CH0244767585

All other details provided in your email (Sell 29,837 shares of UBS Group AG, Net Amount: EUR 1,666,712.84) match our records exactly, and the trade is marked as closed in our system.

Please let us know if you require any further information to complete your records.

Best regards,
Settlement Operations
```