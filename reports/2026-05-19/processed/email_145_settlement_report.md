# MAIA Settlement Mailbox Report - email_145.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Reply to sender confirming final settlement: trade YN21200009 settled on 2026-03-23 (Status: Closed). Include quantity 77,982, amount EUR 1,301,274.03, counterparty Citigroup (LEI provided). Optionally attach official settlement confirmation or statement of settlement if available.
**Reason:** Sender explicitly requests final settlement confirmation for a named trade. Single trade reference and full lookup fields are provided. Request concerns post-settlement review documentation.

---

## 2. Email Summary

**Email ID:** email_145.eml  
**Subject:** Reconciliation Query – YN21200009 – BASF SE  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Citigroup

Sender requests final settlement confirmation and relevant documentation for post-settlement review.

---

## 3. Classification
- **Primary Type:** missing_confirmation (originally confirmation_missing)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | YN21200009 | YN21200009 | match | none |
| security_isin | null | DE000BASF111 | missing_in_email | none |
| security_name | BASF SE | null | missing_in_host | low |
| settlement_date | 2026-03-23 | 2026-03-23 | match | none |
| trade_date | 2026-03-20 | 2026-03-20 | match | none |
| quantity | 77982 | 77982 | match | none |
| amount | 1301274.03 | 1301274.03 | match | none |
| currency | EUR | EUR | match | none |
| side | buy | Buy | match | none |
| counterparty_name | Citigroup | Citigroup (LEI: E57ODZWZ7FF32TWEFA76) | match | none |
| status | unknown | Closed | mismatch | low |

### Discrepancy Flags
- missing_confirmation_requested
- security_isin_missing_in_email
- security_name_missing_in_host
- status_unknown_in_email_but_closed_in_host

---

## 6. Recommended Action
- [x] Reply to sender confirming final settlement: trade YN21200009 settled on 2026-03-23 (Status: Closed). Include quantity 77,982, amount EUR 1,301,274.03, counterparty Citigroup (LEI provided). Optionally attach official settlement confirmation or statement of settlement if available.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email.

We can confirm that trade YN21200009 (Buy 77,982 shares of BASF SE / ISIN DE000BASF111) is currently marked as Closed in our system. The trade successfully settled on 2026-03-23. All details match perfectly (Net Amount: EUR 1,301,274.03, Counterparty: Citigroup). 

Please find the final settlement confirmation attached for your post-settlement review.

Best regards,
Settlement Operations
```