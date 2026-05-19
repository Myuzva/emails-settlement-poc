# MAIA Settlement Mailbox Report - email_120.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** No host/data discrepancies requiring human review. Provide the requested final trade confirmation / SWIFT confirmation to the sender referencing trade WE09006039.
**Reason:** Sender requests final trade confirmation or SWIFT confirmation for a trade recorded as settled.

---

## 2. Email Summary

**Email ID:** email_120  
**Subject:** Trade Confirmation Request – WE09006039  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** 2026-04-28 15:38:48 +0200  
**Counterparty:** Nomura Securities

The sender requests the final trade confirmation or SWIFT confirmation for trade WE09006039, which is recorded as settled.

---

## 3. Classification
- **Primary Type:** missing_confirmation (originally confirmation_missing)
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
| security_isin | null | CH0011075394 | missing_in_email | none |
| security_name | Zurich Insurance Group AG | Zurich Insurance Group AG | match | none |
| settlement_date | 2026-03-17 | 2026-03-17 | match | none |
| trade_date | 2026-03-16 | 2026-03-16 | match | none |
| quantity | 59280 | 59280 | match | none |
| amount | 955284.68 | 955284.68 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty_name | Nomura Securities | YFSWKL48C7RRQDP89D10 | match | none |
| status | settled | Closed | match | low |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No host/data discrepancies requiring human review. Provide the requested final trade confirmation / SWIFT confirmation to the sender referencing trade WE09006039.
- [ ] Respond to requester providing the final trade confirmation or SWIFT confirmation.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email. 

We can confirm that trade WE09006039 (Sell 59,280 shares of Zurich Insurance Group AG) is recorded as Closed in our system and all details match perfectly (Net Amount: EUR 955,284.68). Please find attached the requested final trade confirmation / SWIFT confirmation for this transaction.

Best regards,
Settlement Operations
```