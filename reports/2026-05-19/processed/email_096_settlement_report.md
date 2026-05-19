# MAIA Settlement Mailbox Report - email_096.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing. HOST trade was found by reference and material extracted fields match after safe enrichment; use HOST values to complete the requested trade details/documentation resubmission.
**Reason:** Settlement-related documentation update request with clear trade reference for HOST lookup.

---

## 2. Email Summary

**Email ID:** email_096  
**Subject:** Trade Status Update Request – UF76998758  
**Sender:** Elena Rossi <e.rossi@mediobanca.it>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Morgan Stanley

Counterparty reports incomplete documentation and requests resubmission of full trade details for pre-settlement checks.

---

## 3. Classification
- **Primary Type:** instruction_or_document_update
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
| security_name | ABB Ltd. | ABB Ltd. | match | none |
| isin | null | CH0012530207 | missing_in_email | none |
| settlement_date | 2026-03-10 | 2026-03-10 | match | none |
| trade_date | null | 2026-03-09 | missing_in_email | low |
| quantity | 29748 | 29748 | match | none |
| amount | 1837445.57 | 1837445.57 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | Morgan Stanley | Morgan Stanley | match | none |
| counterparty_lei | null | 9R7GPTSO7KV3UQJZQ078 | missing_in_email | low |
| status | null | Offen | missing_in_email | none |

### Discrepancy Flags
- email_claims_incomplete_documentation
- trade_date_missing_in_email
- counterparty_lei_missing_in_email

---

## 6. Recommended Action
- [x] Proceed with standard processing. HOST trade was found by reference and material extracted fields match after safe enrichment; use HOST values to complete the requested trade details/documentation resubmission.
- [ ] Respond to requester providing the full trade details as requested.

---

## 7. Draft Analyst Response Template
```text
Dear Elena Rossi,

Thank you for your email regarding trade UF76998758.

As requested, please find the full trade details below to complete your documentation:
- Reference Number: UF76998758
- Security: ABB Ltd. (ISIN: CH0012530207)
- Trade Date: 2026-03-09
- Settlement Date: 2026-03-10
- Quantity: 29,748
- Net Amount: CHF 1,837,445.57
- Side: Sell
- Counterparty LEI: 9R7GPTSO7KV3UQJZQ078

Please let us know if you require any further information to proceed with the settlement.

Best regards,
Settlement Operations
```