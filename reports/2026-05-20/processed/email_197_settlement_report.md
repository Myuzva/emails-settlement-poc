# MAIA Settlement Mailbox Report - email_197.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Provide the requested confirmation to Morgan Stanley for trade YZ85103017: attach and send the trade advice / execution confirmation. No human review required for trade data reconciliation.
**Reason:** The email asks for the final confirmation slip/trade advice/execution confirmation for a specific trade.

---

## 2. Email Summary

**Email ID:** email_197.eml  
**Subject:** Outstanding Trade – Action Required – YZ85103017  
**Sender:** Claire Dubois <c.dubois@paribas-ops.fr>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Morgan Stanley

The counterparty requests the final confirmation slip or trade advice/execution confirmation for a closed trade.

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
| reference_number | YZ85103017 | YZ85103017 | match | none |
| security_isin | null | US38141G1040 | missing_in_email | none |
| security_name | Goldman Sachs Group Inc. | Goldman Sachs Group Inc. | match | none |
| settlement_date | 2026-03-20 | 2026-03-20 | match | none |
| trade_date | 2026-03-19 | 2026-03-19 | match | none |
| quantity | 87805 | 87805 | match | none |
| amount | 932975.05 | 932975.05 | match | none |
| currency | CHF | CHF | match | none |
| side | buy | Kauf | match | none |
| counterparty_name | Morgan Stanley | Morgan Stanley | match | none |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- missing_confirmation_requested

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade YZ85103017 matches the email facts (closed, buy, 87,805 @ CHF 932,975.05, settlement 2026-03-20).
- [ ] Provide the requested confirmation to Morgan Stanley for trade YZ85103017: attach and send the trade advice / execution confirmation.

---

## 7. Draft Analyst Response Template
```text
Dear Claire Dubois,

Thank you for your email.

Please find attached the requested final confirmation slip / execution confirmation for trade YZ85103017 (Buy 87,805 shares of Goldman Sachs Group Inc.). 

Best regards,
Settlement Operations
```