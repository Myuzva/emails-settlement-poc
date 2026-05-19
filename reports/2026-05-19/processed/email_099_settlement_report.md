# MAIA Settlement Mailbox Report - email_099.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Proceed with standard processing: HOST trade was matched and economics, dates, side, security, and counterparty reconcile. The sender is requesting final trade confirmation or SWIFT confirmation for audit evidence; provide or route for documentation issuance according to internal process.
**Reason:** Sender requests final trade confirmation or SWIFT confirmation for a settled closed trade. Single trade reference and supporting trade details are present.

---

## 2. Email Summary

**Email ID:** email_099  
**Subject:** Outstanding Trade – Action Required – QQ15669741  
**Sender:** James O'Brien <j.obrien@meridianfunds.co.uk>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Société Générale

The sender requests final trade confirmation or SWIFT confirmation for audit evidence for a settled trade.

---

## 3. Classification
- **Primary Type:** confirmation_missing
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | QQ15669741 | QQ15669741 | match | none |
| security_isin | null | US30303M1027 | missing_in_email | none |
| security_name | Meta Platforms Inc. | Meta Platforms Inc. | match | none |
| settlement_date | 2026-03-18 | 2026-03-18 | match | none |
| trade_date | 2026-03-17 | 2026-03-17 | match | none |
| quantity | 34657 | 34657 | match | none |
| amount | 1773667.56 | 1773667.56 | match | none |
| currency | USD | USD | match | none |
| side | buy | Buy | match | none |
| counterparty_name | Société Générale | Société Générale | match | none |
| status | settled | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade QQ15669741 matches the email facts (Closed, Buy, 34,657 @ USD 1,773,667.56, settlement 2026-03-18).
- [ ] Respond to requester providing the final trade confirmation or SWIFT confirmation as requested.

---

## 7. Draft Analyst Response Template
```text
Dear James O'Brien,

Thank you for your email. 

We can confirm that trade QQ15669741 (Buy 34,657 shares of Meta Platforms Inc.) is currently marked as Closed in our system and all details match perfectly (Net Amount: USD 1,773,667.56). 

Please find attached the requested final trade confirmation / SWIFT confirmation for your audit evidence.

Best regards,
Settlement Operations
```