# MAIA Settlement Mailbox Report - email_065.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing for the documentation_missing request. HOST trade matches the email facts; provide or route for retrieval of the requested archival settlement confirmation or trade advice according to internal document workflow.
**Reason:** Sender requests archival settlement confirmation or trade advice for a specific closed trade. Single trade reference and full lookup fields present.

---

## 2. Email Summary

**Email ID:** email_065  
**Subject:** Trade Inquiry – Reference IY82044718  
**Sender:** John Smith <j.smith@globalcapital.com>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** HSBC

The sender is requesting the archival documentation (settlement confirmation or trade advice) for trade IY82044718, which is recorded as closed.

---

## 3. Classification
- **Primary Type:** documentation_missing (originally instruction_or_document_update)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | IY82044718 | IY82044718 | match | none |
| security_name | JPMorgan Chase & Co. | JPMorgan Chase & Co. | match | none |
| isin | null | US46625H1005 | missing_in_email | none |
| trade_date | 2026-03-13 | 2026-03-13 | match | none |
| settlement_date | 2026-03-16 | 2026-03-16 | match | none |
| side | buy | Kauf | match | none |
| quantity | 43083 | 43083 | match | none |
| amount | 315787.63 | 315787.63 | match | none |
| currency | CHF | CHF | match | none |
| counterparty_name | HSBC | HSBC | match | none |
| counterparty_lei | null | MP6I5ZYZBEU3UXPYFY54 | missing_in_email | none |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade IY82044718 matches the email facts (closed, buy, 43,083 @ CHF 315,787.63, settlement 2026-03-16).
- [ ] Provide or route for retrieval of the requested archival settlement confirmation or trade advice according to internal document workflow.

---

## 7. Draft Analyst Response Template
```text
Dear John Smith,

Thank you for your inquiry regarding trade IY82044718.

We have verified the trade details in our system (Buy 43,083 shares of JPMorgan Chase & Co., Net Amount: CHF 315,787.63, Settlement Date: 2026-03-16). The trade is successfully closed. 

Please find attached the requested archival settlement confirmation/trade advice for your records.

Best regards,
Settlement Operations
```