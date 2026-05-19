# MAIA Settlement Mailbox Report - email_077.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Operations: confirm whether internal pre-settlement checks for trade SU29131919 are complete and whether the trade is on track for timely settlement. Suggested reply to sender: confirm trade exists and is currently marked 'open' in the system (status matches), and advise expected next steps once Operations confirms pre-settlement checks.
**Reason:** The email asks for confirmation of pre-settlement checks and timely settlement, providing complete trade details for HOST lookup.

---

## 2. Email Summary

**Email ID:** email_077  
**Subject:** Settlement Query – Apple Inc. – 2026-03-31  
**Sender:** Elena Rossi <e.rossi@mediobanca.it>  
**Received:** 2026-04-28T15:38:48+02:00  
**Counterparty:** Goldman Sachs

The sender asks whether internal pre-settlement checks are complete and whether trade SU29131919 is on track for timely settlement while marked open.

---

## 3. Classification
- **Primary Type:** general_status_request (originally settlement_status_request)
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
| security_name | Apple Inc. | null | missing_in_host | low |
| settlement_date | 2026-03-31 | 2026-03-31 | match | none |
| trade_date | 2026-03-30 | 2026-03-30 | match | none |
| quantity | 56269 | 56269 | match | none |
| amount | 1916595.59 | 1916595.59 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | Goldman Sachs | Goldman Sachs | match | none |
| counterparty_lei | null | W22LROWP2IHZNBB6K528 | missing_in_email | none |
| status | open | Offen | match | none |

### Discrepancy Flags
- status_open
- security_name_missing_in_host
- security_isin_present_only_in_host
- operational_confirmation_required

---

## 6. Recommended Action
- [x] No critical reconciliation discrepancy found. Host trade SU29131919 matches the email facts (open, sell, 56,269 @ CHF 1,916,595.59, settlement 2026-03-31).
- [ ] Operations to confirm whether internal pre-settlement checks are complete.
- [ ] Respond to requester confirming trade exists and is currently marked 'open' in the system, and advise expected next steps once Operations confirms pre-settlement checks.

---

## 7. Draft Analyst Response Template
```text
Dear Elena Rossi,

Thank you for your email regarding trade SU29131919 (Apple Inc.).

We can confirm that the trade is currently marked as Open in our system and all details match perfectly (Sell 56,269 shares, Net Amount: CHF 1,916,595.59, Settlement Date: 2026-03-31). 

We are currently verifying with our Operations team if all internal pre-settlement checks are complete. We will provide you with an update on the timely settlement as soon as we receive confirmation.

Best regards,
Settlement Operations
```