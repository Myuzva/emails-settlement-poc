# MAIA Settlement Mailbox Report - email_047.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Proceed with standard processing. Provide or route the requested archival settlement confirmation or trade advice according to normal workflow.
**Reason:** The email requests archival settlement confirmation or trade advice for a specific closed trade and provides trade reference plus settlement details.

---

## 2. Email Summary

**Email ID:** email_047  
**Subject:** Unmatched Trade – Amazon.com Inc. – TN29591110  
**Sender:** Claire Dubois <c.dubois@paribas-ops.fr>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Citigroup

The sender requests archival documentation: relevant settlement confirmation or trade advice for records for trade TN29591110, which is recorded as closed.

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
| reference_number | TN29591110 | TN29591110 | match | none |
| security_isin | null | US0231351067 | missing_in_email | none |
| security_name | Amazon.com Inc. | Amazon.com Inc. | match | none |
| trade_date | 2026-03-27 | 2026-03-27 | match | none |
| settlement_date | 2026-03-30 | 2026-03-30 | match | none |
| side | buy | Buy | match | none |
| quantity | 43183 | 43183 | match | none |
| amount | 1786042.27 | 1786042.27 | match | none |
| currency | EUR | EUR | match | none |
| counterparty_name | Citigroup | Citigroup | match | none |
| counterparty_lei | null | E57ODZWZ7FF32TWEFA76 | missing_in_email | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade TN29591110 matches the email facts (Closed, Buy, 43,183 @ EUR 1,786,042.27, settlement 2026-03-30).
- [ ] Respond to requester providing the requested archival settlement confirmation or trade advice.

---

## 7. Draft Analyst Response Template
```text
Dear Claire Dubois,

Thank you for your email. 

We can confirm that trade TN29591110 (Buy 43,183 shares of Amazon.com Inc.) is recorded as Closed in our system and all details match perfectly (Net Amount: EUR 1,786,042.27). 

As requested, please find attached the archival settlement confirmation / trade advice for your records.

Best regards,
Settlement Operations
```