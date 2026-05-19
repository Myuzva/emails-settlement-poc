# MAIA Settlement Mailbox Report - email_194.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing. HOST trade was found and reconciles to the email facts; provide or retrieve the requested final settlement confirmation/documentation for trade IN04953005.
**Reason:** Email explicitly requests final settlement confirmation for a single referenced trade. Attached PDF provides complete trade details for HOST lookup.

---

## 2. Email Summary

**Email ID:** email_194.eml  
**Subject:** Trade Confirmation Request – IN04953005  
**Sender:** James O'Brien <j.obrien@meridianfunds.co.uk>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Deutsche Bank

The sender requests final settlement confirmation/documentation for post-settlement review for trade IN04953005.

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
| reference_number | IN04953005 | IN04953005 | match | none |
| security_name | Amazon.com Inc. | Amazon.com Inc. | match | none |
| isin | null | US0231351067 | missing_in_email | none |
| trade_date | 2026-03-10 | 2026-03-10 | match | none |
| settlement_date | 2026-03-11 | 2026-03-11 | match | none |
| side | sell | Verkauf | match | none |
| quantity | 19725 | 19725 | match | none |
| amount | 933595.17 | 933595.17 | match | none |
| currency | CHF | CHF | match | none |
| counterparty_name | Deutsche Bank | Deutsche Bank | match | none |
| counterparty_lei | null | 7LTWFZYICNSX8D621K86 | missing_in_email | none |
| status | unknown | Geschlossen | missing_in_email | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] Proceed with standard processing. HOST trade was found and reconciles to the email facts; provide or retrieve the requested final settlement confirmation/documentation for trade IN04953005.
- [ ] Respond to requester providing the final settlement confirmation for trade IN04953005.

---

## 7. Draft Analyst Response Template
```text
Dear James O'Brien,

Thank you for your email.

We can confirm that trade IN04953005 (Sell 19,725 shares of Amazon.com Inc.) is currently marked as Geschlossen (Closed) in our system and all details match perfectly (Net Amount: CHF 933,595.17). 

Please find attached the final settlement confirmation for trade IN04953005 as requested.

Best regards,
Settlement Operations
```