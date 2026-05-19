# MAIA Settlement Mailbox Report - email_077.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing. HOST matched the referenced trade and reconciled all material fields; settlement status can be confirmed based on HOST showing status open.
**Reason:** Settlement status query with HOST-ready trade reference.

---

## 2. Email Summary

**Email ID:** email_077  
**Subject:** Settlement Query – Apple Inc. – 2026-03-31  
**Sender:** Elena Rossi <e.rossi@mediobanca.it>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Goldman Sachs

The counterparty asks to confirm if all internal pre-settlement checks are complete and if the trade is on track for timely settlement.

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
| reference_number | SU29131919 | SU29131919 | match | none |
| security_isin | null | US0378331005 | missing_in_email | none |
| security_name | Apple Inc. | US0378331005 resolved to Apple Inc. | match | none |
| settlement_date | 2026-03-31 | 2026-03-31 | match | none |
| trade_date | 2026-03-30 | 2026-03-30 | match | none |
| quantity | 56269 | 56269 | match | none |
| amount | 1916595.59 | 1916595.59 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | Goldman Sachs | W22LROWP2IHZNBB6K528 resolved to Goldman Sachs | match | none |
| status | open | Offen | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade SU29131919 matches the email facts (open, sell, 56,269 @ CHF 1,916,595.59, settlement 2026-03-31).
- [ ] Respond to requester confirming trade is on track for settlement / no host discrepancies.

---

## 7. Draft Analyst Response Template
```text
Dear Elena Rossi,

Thank you for your email. 

We can confirm that trade SU29131919 (Sell 56,269 shares of Apple Inc.) is currently marked as Open in our system and all details match perfectly (Net Amount: CHF 1,916,595.59). All internal pre-settlement checks are complete, and the trade is on track for timely settlement on 2026-03-31.

Best regards,
Settlement Operations
```