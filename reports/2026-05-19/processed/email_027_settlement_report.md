# MAIA Settlement Mailbox Report - email_027.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Record confirms host trade matches email details. Provide requester with the executed trade confirmation / trade advice from records (attach the stored confirmation). No human escalation required.
**Reason:** Sender requests final confirmation slip/trade advice/execution confirmation for a specific trade. Single trade reference and full trade details are provided.

---

## 2. Email Summary

**Email ID:** email_027  
**Subject:** Reconciliation Query – WV50025113 – BASF SE  
**Sender:** Michael Hartmann <m.hartmann@eurofin.de>  
**Received:** 2026-04-28 15:38:47 +0200  
**Counterparty:** HSBC

The counterparty requests the final confirmation slip/trade advice or execution confirmation for audit records regarding trade WV50025113.

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
| security_isin | null | DE000BASF111 | missing_in_email | none |
| security_name | BASF SE | BASF SE | match | none |
| settlement_date | 2026-03-23 | 2026-03-23 | match | none |
| trade_date | 2026-03-20 | 2026-03-20 | match | none |
| quantity | 95759 | 95759 | match | none |
| amount | 1126263.19 | 1126263.19 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty_name | HSBC | HSBC (MP6I5ZYZBEU3UXPYFY54) | match | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] Record confirms host trade matches email details. Provide requester with the executed trade confirmation / trade advice from records (attach the stored confirmation). No human escalation required.
- [ ] Respond to requester with the requested confirmation slip.

---

## 7. Draft Analyst Response Template
```text
Dear Michael Hartmann,

Thank you for your email.

Please find attached the final confirmation slip / trade advice for trade WV50025113 (Sell 95,759 shares of BASF SE) as requested for your audit records. All details match our records (Net Amount: EUR 1,126,263.19, Settlement Date: 2026-03-23).

Best regards,
Settlement Operations
```