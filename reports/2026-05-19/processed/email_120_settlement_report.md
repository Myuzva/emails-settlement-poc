# MAIA Settlement Mailbox Report - email_120.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing: HOST trade was found and reconciles to the email facts. Provide or request generation of the final trade confirmation or SWIFT confirmation for trade WE09006039 as requested.
**Reason:** Trade reference WE09006039 is available for HOST lookup. Settlement-related confirmation request with sufficient lookup data.

---

## 2. Email Summary

**Email ID:** email_120  
**Subject:** Trade Confirmation Request – WE09006039  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Nomura Securities

Sender requests final trade confirmation or SWIFT confirmation for the settled trade as quarter-end audit evidence.

---

## 3. Classification
- **Primary Type:** confirmation_missing (originally confirmation_missing)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | WE09006039 | WE09006039 | match | none |
| security_name | Zurich Insurance Group AG | Zurich Insurance Group AG | match | none |
| isin | null | CH0011075394 | missing_in_email | none |
| settlement_date | 2026-03-17 | 2026-03-17 | match | none |
| trade_date | 2026-03-16 | 2026-03-16 | match | none |
| quantity | 59280 | 59280 | match | none |
| amount | 955284.68 | 955284.68 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty_name | Nomura Securities | Nomura Securities | match | none |
| counterparty_lei | null | YFSWKL48C7RRQDP89D10 | missing_in_email | none |
| status | settled | Closed | match | none |

### Discrepancy Flags
- missing_confirmation_requested

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade WE09006039 matches the email facts (Closed, Sale, 59,280 @ EUR 955,284.68, settlement 2026-03-17).
- [ ] Provide or request generation of the final trade confirmation or SWIFT confirmation for trade WE09006039.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email. 

We can confirm that trade WE09006039 (Sale 59,280 shares of Zurich Insurance Group AG) is recorded as Closed in our system and all details match perfectly (Net Amount: EUR 955,284.68). 

Please find attached the requested final trade confirmation / SWIFT confirmation for your records.

Best regards,
Settlement Operations
```