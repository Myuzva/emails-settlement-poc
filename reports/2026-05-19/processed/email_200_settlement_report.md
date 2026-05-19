# MAIA Settlement Mailbox Report - email_200.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard status-response workflow confirming the referenced trade details are consistent in HOST.
**Reason:** Single settlement-related status request with clear trade reference ET58646605.

---

## 2. Email Summary

**Email ID:** email_200  
**Subject:** Reconciliation Query – ET58646605 – Goldman Sachs Group Inc.  
**Sender:** Elena Rossi <e.rossi@mediobanca.it>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Deutsche Bank

Sender requests confirmation that pre-settlement checks are complete and timely settlement remains on track for an open trade.

---

## 3. Classification
- **Primary Type:** settlement_status_request (originally settlement_status_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | ET58646605 | ET58646605 | match | none |
| security_name | Goldman Sachs Group Inc. | Goldman Sachs Group Inc. | match | none |
| isin | null | US38141G1040 | missing_in_email | none |
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| side | buy | Kauf | match | none |
| quantity | 13513 | 13513 | match | none |
| amount | 1175985.38 | 1175985.38 | match | none |
| currency | USD | USD | match | none |
| counterparty_name | Deutsche Bank | Deutsche Bank | match | none |
| counterparty_lei | null | 7LTWFZYICNSX8D621K86 | missing_in_email | none |
| status | open | Offen | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No human review required for reconciliation. HOST trade matches the email facts after safe normalization and enrichment. Proceed with standard status-response workflow confirming the referenced trade details are consistent in HOST.
- [ ] Respond to requester confirming trade is on track for settlement / no host discrepancies.

---

## 7. Draft Analyst Response Template
```text
Dear Elena Rossi,

Thank you for your email. 

We can confirm that trade ET58646605 (Buy 13,513 shares of Goldman Sachs Group Inc.) is currently marked as Open in our system and all details match perfectly (Net Amount: USD 1,175,985.38). All internal pre-settlement checks are complete, and the trade is on track for timely settlement on 2026-03-13.

Best regards,
Settlement Operations
```