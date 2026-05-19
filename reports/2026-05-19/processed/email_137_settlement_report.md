# MAIA Settlement Mailbox Report - email_137.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Confirm that HOST trade SL99789329 is booked with settlement date 2026-03-19, while the email/attachment instruction states 2026-04-27. All other reconciled fields match after safe enrichment and normalization. Because the email is explicitly requesting confirmation of the settlement date, handle through standard confirmation workflow rather than human-in-the-loop escalation.
**Reason:** Single clear trade reference is available for HOST lookup. Primary issue is a settlement date mismatch requiring standard reconciliation processing.

---

## 2. Email Summary

**Email ID:** email_137  
**Subject:** Reconciliation Query – SL99789329 – Apple Inc.  
**Sender:** John Smith <j.smith@globalcapital.com>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** JP Morgan

The sender reports a value date mismatch on trade SL99789329. Their internal booking reflects 19-Mar-2026, whereas the instruction received indicates 27-Apr-2026, and requests confirmation of the correct settlement date.

---

## 3. Classification
- **Primary Type:** settlement_date_mismatch (originally settlement_date_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | SL99789329 | SL99789329 | match | none |
| security_name | Apple Inc. | Apple Inc. | match | none |
| isin | null | US0378331005 | missing_in_email | none |
| trade_date | 2026-03-18 | 2026-03-18 | match | none |
| settlement_date | 2026-04-27 | 2026-03-19 | mismatch | high |
| side | sell | Verkauf | match | none |
| quantity | 84028 | 84028 | match | none |
| amount | 1795415.75 | 1795415.75 | match | none |
| currency | CHF | CHF | match | none |
| counterparty_name | JP Morgan | JP Morgan | match | none |
| counterparty_lei | null | 8I5DZWZKVSZI1NUHU748 | missing_in_email | low |
| status | unknown | Offen | missing_in_email | none |

### Discrepancy Flags
- settlement_date_mismatch
- host_settlement_date_matches_sender_internal_booking_date
- email_instruction_settlement_date_differs_from_host

---

## 6. Recommended Action
- [x] Confirm that HOST trade SL99789329 is booked with settlement date 2026-03-19, while the email/attachment instruction states 2026-04-27. All other reconciled fields match after safe enrichment and normalization. Because the email is explicitly requesting confirmation of the settlement date, handle through standard confirmation workflow rather than human-in-the-loop escalation.
- [ ] Respond to requester confirming the correct settlement date.

---

## 7. Draft Analyst Response Template
```text
Dear John Smith,

Thank you for your email regarding trade SL99789329 (Apple Inc.).

We have reviewed the details and can confirm that our internal booking reflects a settlement date of 2026-03-19, which matches your internal booking. The instruction indicating 2026-04-27 appears to be incorrect. All other trade details (Sell 84,028 shares, Net Amount: CHF 1,795,415.75) match perfectly.

Please let us know if you need any further clarification or if we should amend the instruction.

Best regards,
Settlement Operations
```