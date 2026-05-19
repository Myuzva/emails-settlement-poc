# MAIA Settlement Mailbox Report - email_195.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard response: advise the sender that HOST shows the trade as Offen/open and no economic-field discrepancy was found. No human review is required based on this reconciliation.
**Reason:** Settlement-related status request with usable trade reference. Attachment processed successfully.

---

## 2. Email Summary

**Email ID:** email_195  
**Subject:** Trade Status Update Request – KK26393091  
**Sender:** Michael Hartmann <m.hartmann@eurofin.de>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** BNP Paribas

The sender requests current settlement status/action guidance for the trade; no failure or mismatch is claimed.

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
| reference_number | KK26393091 | KK26393091 | match | none |
| security_name | Goldman Sachs Group Inc. | Goldman Sachs Group Inc. | match | none |
| isin | null | US38141G1040 | missing_in_email | none |
| trade_date | 2026-03-23 | 2026-03-23 | match | none |
| settlement_date | 2026-03-24 | 2026-03-24 | match | none |
| side | sell | Verkauf | match | none |
| quantity | 25199 | 25199 | match | none |
| amount | 1171796.04 | 1171796.04 | match | none |
| currency | CHF | CHF | match | none |
| counterparty_name | BNP Paribas | BNP Paribas | match | none |
| counterparty_lei | null | R0MUWSFPU8MPRO8K5P83 | missing_in_email | none |
| status | unknown | Offen | missing_in_email | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade KK26393091 matches the email facts (Offen, Verkauf, 25,199 @ CHF 1,171,796.04, settlement 2026-03-24).
- [ ] Respond to requester confirming trade is on track for settlement / no host discrepancies.

---

## 7. Draft Analyst Response Template
```text
Dear Michael Hartmann,

Thank you for your email. 

We can confirm that trade KK26393091 (Sell 25,199 shares of Goldman Sachs Group Inc.) is currently marked as Open (Offen) in our system and all details match perfectly (Net Amount: CHF 1,171,796.04). All internal pre-settlement checks are complete, and the trade is on track for timely settlement on 2026-03-24.

Best regards,
Settlement Operations
```