# MAIA Settlement Mailbox Report - email_199.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Provide the requester with archival settlement documentation and confirmation that trade CP74965381 is closed.
**Reason:** Sender requests archival documentation for a specific trade recorded as closed.

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
| reference_number | CP74965381 | CP74965381 | match | none |
| security_isin | null | CH0012530207 | missing_in_email | none |
| security_name | ABB Ltd. | ABB Ltd. | match | none |
| settlement_date | 2026-03-11 | 2026-03-11 | match | none |
| trade_date | 2026-03-10 | 2026-03-10 | match | none |
| quantity | 57963 | 57963 | match | none |
| amount | 1308340.30 | 1308340.30 | match | none |
| currency | EUR | EUR | match | none |
| side | buy | Buy | match | none |
| counterparty_name | Goldman Sachs | Goldman Sachs | match | none |
| counterparty_lei | null | W22LROWP2IHZNBB6K528 | missing_in_email | low |
| status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] All key trade fields match host records. Provide the requester with archival settlement documentation and confirmation that trade CP74965381 is closed; include ISIN CH0012530207 and LEI W22LROWP2IHZNBB6K528 in the response for completeness.

---

## 7. Draft Analyst Response Template
```text
Dear Sarah Jensen,

Thank you for your email. 

We can confirm that trade CP74965381 (Buy 57,963 shares of ABB Ltd., ISIN CH0012530207) is closed in our system. All details match perfectly (Net Amount: EUR 1,308,340.30, Settlement Date: 2026-03-11).

Please find attached the requested archival settlement documentation for your records.

Best regards,
Settlement Operations
```