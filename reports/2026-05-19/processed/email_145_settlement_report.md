# MAIA Settlement Mailbox Report - email_145.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Proceed with standard processing and provide the requested final settlement confirmation for trade YN21200009. No human review is required based on HOST reconciliation.
**Reason:** Sender requests final settlement confirmation for a specific trade reference and provides complete trade details.

---

## 2. Email Summary

**Email ID:** email_145  
**Subject:** Reconciliation Query – YN21200009 – BASF SE  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Citigroup  

The sender requests final settlement confirmation/documentation for post-settlement review for trade YN21200009.

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
| security_name | BASF SE | BASF SE | match | none |
| settlement_date | 2026-03-23 | 2026-03-23 | match | none |
| trade_date | 2026-03-20 | 2026-03-20 | match | none |
| quantity | 77982 | 77982 | match | none |
| amount | 1301274.03 | 1301274.03 | match | none |
| currency | EUR | EUR | match | none |
| side | buy | Buy | match | none |
| counterparty_name | Citigroup | Citigroup | match | none |
| counterparty_lei | null | E57ODZWZ7FF32TWEFA76 | missing_in_email | none |
| status | settled | Closed | match | low |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade YN21200009 matches the email facts (Closed, Buy, 77,982 @ EUR 1,301,274.03, settlement 2026-03-23).
- [x] Respond to requester providing the final settlement confirmation for trade YN21200009.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email.

We can confirm that trade YN21200009 (Buy 77,982 shares of BASF SE) has successfully settled on 2026-03-23. All details match our records (Net Amount: EUR 1,301,274.03). Please find the final settlement confirmation attached as requested.

Best regards,
Settlement Operations
```