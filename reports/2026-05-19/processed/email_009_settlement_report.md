# MAIA Settlement Mailbox Report - email_009.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** High  
**Recommended Action:** Proceed with standard settlement-date discrepancy handling.
**Reason:** The email explicitly states a value date mismatch for one trade reference and asks to confirm correct settlement date.

---

## 2. Email Summary

**Email ID:** email_009  
**Subject:** Trade Confirmation Request – BP86251923  
**Sender:** Elena Rossi <e.rossi@mediobanca.it>  
**Received:** 2026-04-28 13:38 UTC  
**Counterparty:** HSBC

Sender reports value date mismatch: internal booking shows 23.03.2026 while instruction from recipient side shows 23.04.2026; asks to confirm correct settlement date.

---

## 3. Classification
- **Primary Type:** settlement_date_mismatch (originally settlement_date_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | BP86251923 | BP86251923 | match | none |
| security_isin | null | DE0007236101 | missing_in_email | none |
| security_name | Siemens AG | Siemens AG | match | none |
| trade_date | 2026-03-20 | 2026-03-20 | match | none |
| settlement_date | 2026-04-23 | 2026-03-23 | mismatch | high |
| quantity | 67180 | 67180 | match | none |
| amount | 313757.36 | 313757.36 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | HSBC | HSBC | match | none |
| counterparty_lei | null | MP6I5ZYZBEU3UXPYFY54 | missing_in_email | low |
| status | null | Offen | missing_in_email | none |

### Discrepancy Flags
- settlement_date_mismatch

---

## 6. Recommended Action
- [x] Proceed with standard settlement-date discrepancy handling. HOST trade matches the email on reference, trade date, quantity, amount, currency, side, security after enrichment, and counterparty after enrichment. 
- [x] HOST settlement date is 2026-03-23, while the email table/instruction value is 2026-04-23; this aligns with the sender's stated internal booking date and should be used to confirm the correct HOST-recorded settlement date.
- [ ] Respond to requester confirming the correct settlement date.

---

## 7. Draft Analyst Response Template
```text
Dear Elena Rossi,

Thank you for your email regarding trade BP86251923.

We have reviewed the trade details in our system. We can confirm that our internal records show the settlement date as 23.03.2026, which aligns with your internal booking. All other trade details (Sell 67,180 shares of Siemens AG, Net Amount: EUR 313,757.36) match perfectly.

Please let us know if you need any further assistance to amend the instruction on your side.

Best regards,
Settlement Operations
```