# MAIA Settlement Mailbox Report - email_027.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing: HOST trade matches the email facts. Provide or route the requested final confirmation slip, trade advice, or execution confirmation for trade WV50025113.
**Reason:** Email explicitly requests final confirmation slip/trade advice/execution confirmation for one trade. Single trade reference and complete lookup facts are present in the body table.

---

## 2. Email Summary

**Email ID:** email_027  
**Subject:** Reconciliation Query – WV50025113 – BASF SE  
**Sender:** Michael Hartmann <m.hartmann@eurofin.de>  
**Received:** Tue, 28 Apr 2026 15:38:47 +0200  
**Counterparty:** HSBC

The sender requests the final confirmation slip, trade advice, or execution confirmation for the closed trade WV50025113.

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
| reference_number | WV50025113 | WV50025113 | match | none |
| security_name | BASF SE | BASF SE | match | none |
| isin | null | DE000BASF111 | missing_in_email | none |
| trade_date | 2026-03-20 | 2026-03-20 | match | none |
| settlement_date | 2026-03-23 | 2026-03-23 | match | none |
| side | sell | Sale | match | none |
| quantity | 95759 | 95759 | match | none |
| amount | 1126263.19 | 1126263.19 | match | none |
| currency | EUR | EUR | match | none |
| counterparty_name | HSBC | HSBC | match | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- missing_confirmation_requested

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade WV50025113 matches the email facts (closed, sell, 95,759 @ EUR 1,126,263.19, settlement 2026-03-23).
- [ ] Provide or route the requested final confirmation slip, trade advice, or execution confirmation for trade WV50025113.

---

## 7. Draft Analyst Response Template
```text
Dear Michael Hartmann,

Thank you for your email. 

We can confirm that trade WV50025113 (Sell 95,759 shares of BASF SE) is currently marked as Closed in our system and all details match perfectly (Net Amount: EUR 1,126,263.19). As requested, please find attached the final confirmation slip / trade advice / execution confirmation for this trade.

Best regards,
Settlement Operations
```