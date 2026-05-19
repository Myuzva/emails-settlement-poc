# MAIA Settlement Mailbox Report - email_200.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Proceed with status confirmation.
**Reason:** Trade found by reference number ET58646605. All critical fields (quantity, amount, dates, currency) match exactly.

---

## 2. Email Summary

**Email ID:** email_200.eml  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Deutsche Bank

Email requests settlement status for trade ET58646605. Attachment contains trade details.

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
| reference_number | ET58646605 | ET58646605 | match | none |
| security_isin | null | US38141G1040 | missing_in_email | none |
| security_name | Goldman Sachs Group Inc. | Goldman Sachs Group Inc. | match | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| quantity | 13513 | 13513 | match | none |
| amount | 1175985.38 | 1175985.38 | match | none |
| currency | USD | USD | match | none |
| side | buy | buy | match | none |
| counterparty_name | Deutsche Bank | Deutsche Bank | match | none |
| status | open | open | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade ET58646605 matches the email facts (open, buy, 13,513 @ USD 1,175,985.38, settlement 2026-03-13).
- [ ] Respond to requester confirming trade is on track for settlement / no host discrepancies.

---

## 7. Draft Analyst Response Template
```text
Dear Deutsche Bank Settlement Team,

Thank you for your email. 

We can confirm that trade ET58646605 (Buy 13,513 shares of Goldman Sachs Group Inc.) is currently marked as open in our system and all details match perfectly (Net Amount: USD 1,175,985.38). All internal pre-settlement checks are complete, and the trade is on track for timely settlement on 2026-03-13.

Best regards,
Settlement Operations
```