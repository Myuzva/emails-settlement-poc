# MAIA Settlement Mailbox Report - email_199.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing: HOST trade matches the email facts, and enrichment confirms the HOST security and counterparty identifiers correspond to the email names. No human review is required for trade-data reconciliation; handle the sender's request for archival settlement confirmation or trade advice according to the documentation workflow.
**Reason:** Single trade reference CP74965381 available for HOST lookup. Request concerns settlement/trade documentation.

---

## 2. Email Summary

**Email ID:** email_199.eml  
**Subject:** Clarification Required: Trade CP74965381  
**Sender:** Sarah Jensen <s.jensen@nordbank.com>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Goldman Sachs

The sender requests archival settlement confirmation or trade advice for a single identified closed trade.

---

## 3. Classification
- **Primary Type:** instruction_or_document_update
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | CP74965381 | CP74965381 | match | none |
| security_name | ABB Ltd. | ABB Ltd. | match | none |
| isin | null | CH0012530207 | missing_in_email | none |
| trade_date | 2026-03-10 | 2026-03-10 | match | none |
| settlement_date | 2026-03-11 | 2026-03-11 | match | none |
| side | buy | Buy | match | none |
| quantity | 57963 | 57963 | match | none |
| amount | 1308340.3 | 1308340.3 | match | none |
| currency | EUR | EUR | match | none |
| counterparty_name | Goldman Sachs | Goldman Sachs | match | none |
| counterparty_lei | null | W22LROWP2IHZNBB6K528 | missing_in_email | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- documentation_missing_request

---

## 6. Recommended Action
- [x] Proceed with standard processing: HOST trade matches the email facts, and enrichment confirms the HOST security and counterparty identifiers correspond to the email names. No human review is required for trade-data reconciliation; handle the sender's request for archival settlement confirmation or trade advice according to the documentation workflow.
- [ ] Provide the requested archival settlement confirmation or trade advice for trade CP74965381.

---

## 7. Draft Analyst Response Template
```text
Dear Sarah Jensen,

Thank you for your email.

Please find attached the requested archival settlement confirmation and trade advice for trade CP74965381 (Buy 57,963 shares of ABB Ltd.). As noted, the trade is recorded as Closed in our system with a settlement date of 2026-03-11.

If you require any further documentation or clarification, please let us know.

Best regards,
Settlement Operations
```