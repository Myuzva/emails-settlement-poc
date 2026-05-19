# MAIA Settlement Mailbox Report - email_115.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Send the archival settlement confirmation / trade advice for KL96142296 to the requester. Attach the settlement confirmation referencing ISIN CH0012032048 and record counterparty LEI 9DJT3MQOBQGTCQ1MXC84.
**Reason:** Sender requests archival settlement confirmation or trade advice for a closed trade.

---

## 2. Email Summary

**Email ID:** email_115  
**Subject:** Outstanding Trade – Action Required – KL96142296  
**Sender:** John Smith <j.smith@globalcapital.com>  
**Received:** 2026-04-28 13:38 UTC  
**Counterparty:** Bank of America

The sender requests the archival documentation for trade KL96142296, which is recorded as closed in their system.

---

## 3. Classification
- **Primary Type:** instruction_or_document_update (originally documentation_missing)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | KL96142296 | KL96142296 | match | none |
| security_isin | null | CH0012032048 | missing_in_email | none |
| security_name | Roche Holding AG | Roche Holding AG | match | none |
| trade_date | 2026-03-05 | 2026-03-05 | match | none |
| settlement_date | 2026-03-06 | 2026-03-06 | match | none |
| quantity | 52525 | 52525 | match | none |
| amount | 1335818.94 | 1335818.94 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty_name | Bank of America | Bank of America | match | none |
| counterparty_lei | null | 9DJT3MQOBQGTCQ1MXC84 | missing_in_email | none |
| reported_status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] Send the archival settlement confirmation / trade advice for KL96142296 to the requester. Attach the settlement confirmation referencing ISIN CH0012032048 and record counterparty LEI 9DJT3MQOBQGTCQ1MXC84.

---

## 7. Draft Analyst Response Template
```text
Dear Bank of America Settlement Team,

Thank you for your email. 

As requested, please find attached the archival settlement confirmation for trade KL96142296 (Sell 52,525 shares of Roche Holding AG, ISIN CH0012032048). The trade is recorded as Closed in our system with a Net Amount of EUR 1,335,818.94 and settlement date 2026-03-06.

Please let us know if you require any further documentation.

Best regards,
Settlement Operations
```