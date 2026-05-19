# MAIA Settlement Mailbox Report - email_194.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** No human review required. Confirm settlement to sender for trade IN04953005 (settled on 2026-03-11) and attach final settlement confirmation. Consider updating/enriching internal mapping so host counterparty ID 7LTWFZYICNSX8D621K86 is linked to 'Deutsche Bank' and record security ISIN US0231351067 against the trade.
**Reason:** Email explicitly requests final settlement confirmation for a single trade reference. Attached PDF provides matching trade details for the same reference.

---

## 2. Email Summary

**Email ID:** email_194  
**Subject:** Trade Confirmation Request – IN04953005  
**Sender:** James O'Brien <j.obrien@meridianfunds.co.uk>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Deutsche Bank

Sender requests final settlement confirmation/documentation for trade IN04953005.

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
| security | Amazon.com Inc. | US0231351067 | missing_in_email | none |
| settlement_date | 2026-03-11 | 2026-03-11 | match | none |
| trade_date | 2026-03-10 | 2026-03-10 | match | none |
| quantity | 19725 | 19725 | match | none |
| amount | 933595.17 | 933595.17 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | Deutsche Bank | 7LTWFZYICNSX8D621K86 | missing_in_host | medium |
| status | unknown | Geschlossen | missing_in_email | none |

### Discrepancy Flags
- security_isin_missing_in_email
- counterparty_name_missing_in_host_record
- host_uses_counterparty_identifier_not_name
- host_fields_in_german_language

---

## 6. Recommended Action
- [x] No human review required. Confirm settlement to sender for trade IN04953005 (settled on 2026-03-11) and attach final settlement confirmation.
- [ ] Consider updating/enriching internal mapping so host counterparty ID 7LTWFZYICNSX8D621K86 is linked to 'Deutsche Bank' and record security ISIN US0231351067 against the trade.

---

## 7. Draft Analyst Response Template
```text
Dear James O'Brien,

Thank you for your email. 

We can confirm that trade IN04953005 (Sell 19,725 shares of Amazon.com Inc.) has successfully settled on 2026-03-11. Please find the final settlement confirmation attached as requested.

Best regards,
Settlement Operations
```