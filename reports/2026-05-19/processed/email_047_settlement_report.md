# MAIA Settlement Mailbox Report - email_047.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Provide the counterparty with the requested archival documentation (settlement confirmation / trade advice) for TN29591110. Attach the hosted trade record (including ISIN US0231351067) and confirm counterparty identity (Citigroup, LEI E57ODZWZ7FF32TWEFA76). No human review required.
**Reason:** The email requests archival documentation for a specific trade, and all trade details match perfectly with the HOST system.

---

## 2. Email Summary

**Email ID:** email_047  
**Subject:** Unmatched Trade – Amazon.com Inc. – TN29591110  
**Sender:** Claire Dubois <c.dubois@paribas-ops.fr>  
**Received:** Unknown  
**Counterparty:** Citigroup

The counterparty requests a copy of the relevant settlement confirmation or trade advice for archival records for trade TN29591110, which is recorded as closed.

---

## 3. Classification
- **Primary Type:** instruction_or_document_update (originally instruction_or_document_update)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | TN29591110 | TN29591110 | match | high |
| security_name | Amazon.com Inc. | Amazon.com Inc. | match | none |
| security_isin | null | US0231351067 | missing_in_email | none |
| settlement_date | 2026-03-30 | 2026-03-30 | match | none |
| trade_date | 2026-03-27 | 2026-03-27 | match | none |
| side | buy | Buy | match | none |
| quantity | 43183 | 43183 | match | high |
| amount | 1786042.27 | 1786042.27 | match | high |
| currency | EUR | EUR | match | none |
| counterparty_name | Citigroup | Citigroup | match | medium |
| counterparty_lei | null | E57ODZWZ7FF32TWEFA76 | missing_in_email | none |
| reported_status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation differences found. Host trade TN29591110 matches the email facts perfectly.
- [x] Provide the counterparty with the requested archival documentation (settlement confirmation / trade advice) for TN29591110.
- [x] Attach the hosted trade record (including ISIN US0231351067) and confirm counterparty identity (Citigroup, LEI E57ODZWZ7FF32TWEFA76).
- [ ] No human review required.

---

## 7. Draft Analyst Response Template
```text
Dear Claire Dubois,

Thank you for your email.

Please find attached the requested archival documentation (settlement confirmation / trade advice) for trade TN29591110 (Buy 43,183 shares of Amazon.com Inc., ISIN US0231351067). 

As requested, we confirm the trade is recorded as Closed in our system with a Net Amount of EUR 1,786,042.27 and Settlement Date of 2026-03-30.

Please let us know if you need any further assistance.

Best regards,
Settlement Operations
```