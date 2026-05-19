# MAIA Settlement Mailbox Report - email_197.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing for the missing confirmation request. HOST trade was found and reconciles to the email facts; provide or request generation of the final confirmation slip/trade advice for reference YZ85103017 without human review.
**Reason:** Email explicitly requests final confirmation slip/trade advice/execution confirmation for a single identified trade. Trade reference and core lookup fields are present in the body table.

---

## 2. Email Summary

**Email ID:** email_197.eml  
**Subject:** Outstanding Trade – Action Required – YZ85103017  
**Sender:** Claire Dubois <c.dubois@paribas-ops.fr>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Morgan Stanley

The sender requests the final confirmation slip or trade advice/execution confirmation for the closed trade YZ85103017.

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
| counterparty_lei | null | 9R7GPTSO7KV3UQJZQ078 | missing_in_email | none |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- missing_confirmation_requested

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade YZ85103017 matches the email facts (closed, buy, 87,805 @ CHF 932,975.05, settlement 2026-03-20).
- [ ] Provide or request generation of the final confirmation slip/trade advice for reference YZ85103017.
- [ ] Respond to requester with the requested confirmation slip.

---

## 7. Draft Analyst Response Template
```text
Dear Claire Dubois,

Thank you for your email regarding trade YZ85103017.

We have verified the trade details in our system (Buy 87,805 shares of Goldman Sachs Group Inc., Net Amount: CHF 932,975.05, Settlement Date: 2026-03-20). The trade is marked as closed and all details match perfectly. 

Please find attached the requested final confirmation slip / trade advice for your records.

Best regards,
Settlement Operations
```