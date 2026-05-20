# MAIA Settlement Mailbox Report - email_199.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Provide the requested archival settlement confirmation / trade advice to the requester.
**Reason:** Sender requests archival settlement confirmation or trade advice for a specific closed trade.

---

## 2. Email Summary

**Email ID:** email_199  
**Subject:** Clarification Required: Trade CP74965381  
**Sender:** Sarah Jensen <s.jensen@nordbank.com>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Goldman Sachs

The sender is requesting archival documentation (settlement confirmation or trade advice) for trade CP74965381, which is recorded as closed.

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
| reference_number | CP74965381 | CP74965381 | match | high |
| security_isin | null | CH0012530207 | missing_in_email | none |
| security_name | ABB Ltd. | ABB Ltd. | match | none |
| settlement_date | 2026-03-11 | 2026-03-11 | match | high |
| trade_date | 2026-03-10 | 2026-03-10 | match | medium |
| quantity | 57963 | 57963 | match | high |
| amount | 1308340.30 | 1308340.30 | match | high |
| currency | EUR | EUR | match | high |
| side | buy | Buy | match | medium |
| counterparty_name | Goldman Sachs | Goldman Sachs (LEI: W22LROWP2IHZNBB6K528) | match | medium |
| status | closed | Closed | match | low |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancies found. Host trade CP74965381 matches the email facts (closed, buy, 57,963 @ EUR 1,308,340.30, settlement 2026-03-11).
- [ ] Proceed to provide the requested archival settlement confirmation / trade advice to the requester.

---

## 7. Draft Analyst Response Template
```text
Dear Sarah Jensen,

Thank you for your email.

Please find attached the requested archival settlement confirmation / trade advice for trade CP74965381 (Buy 57,963 shares of ABB Ltd.). Our records confirm this trade successfully settled on 2026-03-11.

Let us know if you need any further assistance.

Best regards,
Settlement Operations
```