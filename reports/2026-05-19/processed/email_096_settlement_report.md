# MAIA Settlement Mailbox Report - email_096.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** proceed_with_settlement_details_provision
**Reason:** Sender explicitly requests full trade details due to incomplete documentation.

---

## 2. Email Summary

**Email ID:** email_096  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Morgan Stanley

The sender explicitly requests full trade details due to incomplete documentation so they can proceed with pre-settlement checks.

---

## 3. Classification
- **Primary Type:** generic_trade_details_request
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | UF76998758 | UF76998758 | match | none |
| security_isin | null | CH0012530207 | missing_in_email | none |
| security_name | ABB Ltd. | ABB Ltd. | match | none |
| settlement_date | 2026-03-10 | 2026-03-10 | match | none |
| trade_date | null | 2026-03-09 | missing_in_email | none |
| quantity | 29748 | 29748 | match | none |
| amount | 1837445.57 | 1837445.57 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | sell | match | none |
| counterparty_name | Morgan Stanley | Morgan Stanley | match | none |
| status | unknown | Offen | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade UF76998758 matches the email facts (Offen, sell, 29,748 @ CHF 1,837,445.57, settlement 2026-03-10).
- [ ] Respond to requester providing the full trade details as requested.

---

## 7. Draft Analyst Response Template
```text
Dear Morgan Stanley Settlement Team,

Thank you for your email.

As requested, please find the full trade details for reference UF76998758 below:
- Security: ABB Ltd. (ISIN: CH0012530207)
- Trade Date: 2026-03-09
- Settlement Date: 2026-03-10
- Side: Sell
- Quantity: 29,748
- Net Amount: CHF 1,837,445.57

Our internal pre-settlement checks are complete, and the trade is currently marked as Open in our system. Please let us know if you need any further information to proceed with your checks.

Best regards,
Settlement Operations
```