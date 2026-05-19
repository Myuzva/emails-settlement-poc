# MAIA Settlement Mailbox Report - email_036.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** The trade details provided in the email match the records in the HOST system. Proceed with providing the requested settlement confirmation or trade advice for trade UH78032934.
**Reason:** Sender requests archival settlement confirmation or trade advice for records.

---

## 2. Email Summary

**Email ID:** email_036  
**Subject:** Clarification Required: Trade UH78032934  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Raiffeisen Bank

The sender requests the archival documentation for trade UH78032934, which is recorded as closed in their system, and asks for a copy of the relevant settlement confirmation or trade advice.

---

## 3. Classification
- **Primary Type:** missing_confirmation
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | UH78032934 | UH78032934 | match | none |
| security_isin | null | CH0244767585 | missing_in_email | none |
| security_name | UBS Group AG | UBS Group AG | match | none |
| settlement_date | 2026-03-05 | 2026-03-05 | match | none |
| trade_date | 2026-03-04 | 2026-03-04 | match | none |
| quantity | 91177 | 91177 | match | none |
| amount | 235149.9 | 235149.9 | match | none |
| currency | USD | USD | match | none |
| side | sell | Sale | match | none |
| counterparty_name | Raiffeisen Bank | Raiffeisen Bank | match | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade UH78032934 matches the email facts (closed, sell, 91,177 @ USD 235,149.90, settlement 2026-03-05).
- [ ] Respond to requester providing the requested settlement confirmation or trade advice.

---

## 7. Draft Analyst Response Template
```text
Dear Raiffeisen Bank Settlement Team,

Thank you for your email.

As requested, please find attached the settlement confirmation / trade advice for trade UH78032934 (Sell 91,177 shares of UBS Group AG). The trade is recorded as Closed in our system, and all details match perfectly (Net Amount: USD 235,149.90, Settlement Date: 2026-03-05).

Best regards,
Settlement Operations
```