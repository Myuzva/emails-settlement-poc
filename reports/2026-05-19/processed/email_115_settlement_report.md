# MAIA Settlement Mailbox Report - email_115.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Proceed with standard processing for the documentation request.
**Reason:** Settlement-related document request with HOST-ready trade reference.

---

## 2. Email Summary

**Email ID:** email_115  
**Subject:** Outstanding Trade – Action Required – KL96142296  
**Sender:** John Smith <j.smith@globalcapital.com>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Bank of America

The sender requests archival settlement confirmation or trade advice for a closed trade (KL96142296).

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
| reference_number | KL96142296 | KL96142296 | match | none |
| security_isin | null | CH0012032048 | missing_in_email | none |
| security_name | Roche Holding AG | Roche Holding AG | match | none |
| settlement_date | 2026-03-06 | 2026-03-06 | match | none |
| trade_date | 2026-03-05 | 2026-03-05 | match | none |
| quantity | 52525 | 52525 | match | none |
| amount | 1335818.94 | 1335818.94 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty_name | Bank of America | Bank of America | match | none |
| counterparty_lei | null | 9DJT3MQOBQGTCQ1MXC84 | missing_in_email | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] Proceed with standard processing for the documentation request. HOST trade details match the email facts after safe normalization and enrichment; no human review is required for reconciliation.
- [ ] Provide the requested archival settlement confirmation or trade advice for trade KL96142296.

---

## 7. Draft Analyst Response Template
```text
Dear John Smith,

Thank you for your email.

Please find attached the requested archival settlement confirmation and trade advice for trade KL96142296 (Sale 52,525 shares of Roche Holding AG). As noted, this trade is recorded as Closed in our system with a settlement date of 2026-03-06.

Please let us know if you require any further documentation.

Best regards,
Settlement Operations
```