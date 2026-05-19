# MAIA Settlement Mailbox Report - email_181.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Proceed with standard processing: HOST trade matches the email facts. Provide the requested settlement confirmation or trade advice for reference QQ86998552.
**Reason:** Sender requests a copy of the relevant settlement confirmation or trade advice for archival records.

---

## 2. Email Summary

**Email ID:** email_181.eml  
**Subject:** Trade Exception – QQ86998552  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Credit Suisse

The sender requests archival documentation (settlement confirmation or trade advice) for trade QQ86998552, which is recorded as closed.

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
| reference_number | QQ86998552 | QQ86998552 | match | none |
| security_name | Nestlé S.A. | Nestlé S.A. | match | none |
| isin | null | CH0038863350 | missing_in_email | none |
| settlement_date | 2026-03-30 | 2026-03-30 | match | none |
| trade_date | 2026-03-27 | 2026-03-27 | match | none |
| quantity | 87455 | 87455 | match | none |
| amount | 557959.98 | 557959.98 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | Credit Suisse | Credit Suisse | match | none |
| counterparty_lei | null | ANGGYXNX0JLX3X63W380 | missing_in_email | none |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- documentation_missing_request

---

## 6. Recommended Action
- [x] Proceed with standard processing: HOST trade matches the email facts. Provide the requested settlement confirmation or trade advice for reference QQ86998552 if available through the normal documentation workflow; no human review is required for reconciliation.
- [ ] Send the requested settlement confirmation or trade advice to the sender.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email.

As requested, please find attached the settlement confirmation / trade advice for trade QQ86998552 (Sell 87,455 shares of Nestlé S.A., Net Amount: CHF 557,959.98). The trade is recorded as closed in our system.

Best regards,
Settlement Operations
```