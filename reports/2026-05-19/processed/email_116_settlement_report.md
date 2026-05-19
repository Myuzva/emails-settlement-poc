# MAIA Settlement Mailbox Report - email_116.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing of the sender's request for the final confirmation slip/trade advice; human review is not required based on HOST reconciliation.
**Reason:** Single clear trade reference available for HOST lookup. No attachment extraction failures or conflicting trade values found.

---

## 2. Email Summary

**Email ID:** email_116.eml  
**Subject:** Clarification Required: Trade XV75823317  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Commerzbank

The sender requests the final confirmation slip/trade advice or execution confirmation for a closed trade.

---

## 3. Classification
- **Primary Type:** confirmation_missing (originally confirmation_missing)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | XV75823317 | XV75823317 | match | none |
| security_name | Nestlé S.A. | Nestlé S.A. | match | none |
| isin | null | CH0038863350 | missing_in_email | none |
| trade_date | 2026-03-11 | 2026-03-11 | match | none |
| settlement_date | 2026-03-12 | 2026-03-12 | match | none |
| side | buy | Buy | match | none |
| quantity | 89669 | 89669 | match | none |
| amount | 437947.83 | 437947.83 | match | none |
| currency | CHF | CHF | match | none |
| counterparty_name | Commerzbank | Commerzbank | match | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- missing_confirmation_requested

---

## 6. Recommended Action
- [x] HOST trade was found and reconciles to the email facts. Proceed with standard processing of the sender's request for the final confirmation slip/trade advice; human review is not required based on HOST reconciliation.
- [ ] Provide the requested final confirmation slip/trade advice for trade XV75823317.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email. 

We can confirm that trade XV75823317 (Buy 89,669 shares of Nestlé S.A.) is marked as Closed in our system and all details match perfectly (Net Amount: CHF 437,947.83). 

Please find attached the requested final confirmation slip/trade advice for this trade.

Best regards,
Settlement Operations
```