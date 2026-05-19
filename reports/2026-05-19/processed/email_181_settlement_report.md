# MAIA Settlement Mailbox Report - email_181.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Provide the requester with the archival settlement confirmation / trade advice for QQ86998552 (attach host copy), and include the ISIN CH0038863350 and counterparty LEI ANGGYXNX0JLX3X63W380 in the response for completeness.  
**Reason:** The sender explicitly requests a copy of the relevant settlement confirmation or trade advice for their records.

---

## 2. Email Summary

**Email ID:** email_181  
**Subject:** Trade Exception – QQ86998552  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Credit Suisse

Email requests archival documentation (settlement confirmation or trade advice) for a closed trade. Trade details extracted from attached text file.

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
| reference_number | QQ86998552 | QQ86998552 | match | none |
| security_isin | null | CH0038863350 | missing_in_email | none |
| security_name | Nestlé S.A. | Nestlé S.A. | match | none |
| settlement_date | 2026-03-30 | 2026-03-30 | match | none |
| trade_date | 2026-03-27 | 2026-03-27 | match | none |
| quantity | 87455 | 87455 | match | none |
| amount | 557959.98 | 557959.98 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | Credit Suisse | Credit Suisse (LEI: ANGGYXNX0JLX3X63W380) | match | none |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade QQ86998552 matches the email facts (closed, sell, 87,455 @ CHF 557,959.98, settlement 2026-03-30).
- [ ] Respond to requester providing the requested settlement confirmation or trade advice for their records.

---

## 7. Draft Analyst Response Template
```text
Dear Credit Suisse Settlement Team,

Thank you for your email. 

As requested, please find attached the settlement confirmation for trade QQ86998552 (Sell 87,455 shares of Nestlé S.A.). The trade was successfully closed and settled on 2026-03-30 for a net amount of CHF 557,959.98.

Please let us know if you need any further documentation.

Best regards,
Settlement Operations
```
