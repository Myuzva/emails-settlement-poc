# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Human review required: confirm mapping between email counterparty 'Morgan Stanley' and host counterparty id '9R7GPTSO7KV3UQJZQ078' and resolve security name 'ABB Ltd.' to host identifier CH0012530207. Run /counterparty and /security enrichment lookups (or ask originator to provide ISIN and trade date) and confirm trade date (host shows 2026-03-09). If enrichment confirms equivalence, close the documentation gap; otherwise request corrected trade details from sender.

**Reason:** Unresolved mapping for security name and counterparty reduces automated confidence and requires human confirmation. Trade date is missing in the email.

---

## 2. Email Summary

**Email ID:** email_096  
**Subject:** Trade Status Update Request – UF76998758  
**Sender:** Elena Rossi <e.rossi@mediobanca.it>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Morgan Stanley

The sender reports that documentation/key fields for the trade are incomplete and requests resubmission of full trade details for pre-settlement checks.

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
| security_isin | null | CH0012530207 | missing_in_email | none |
| security_name | ABB Ltd. | CH0012530207 | mismatch | medium |
| settlement_date | 2026-03-10 | 2026-03-10 | match | none |
| trade_date | null | 2026-03-09 | missing_in_email | medium |
| quantity | 29748 | 29748 | match | none |
| amount | 1837445.57 | 1837445.57 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | Morgan Stanley | 9R7GPTSO7KV3UQJZQ078 | mismatch | medium |
| status | unknown | Offen | missing_in_email | none |

### Discrepancy Flags
- security_name_needs_resolution_to_host_identifier
- counterparty_name_not_matched_to_host_counterparty_id
- trade_date_missing_in_email

---

## 6. Findings

The trade was found in HOST with matching reference number, settlement date, quantity, amount, and currency. However, the security name ("ABB Ltd.") and counterparty ("Morgan Stanley") from the email could not be automatically resolved to the HOST identifiers ("CH0012530207" and "9R7GPTSO7KV3UQJZQ078"). Additionally, the trade date is missing in the email but present in HOST (2026-03-09).

---

## 7. Next Steps

1. Confirm mapping between email counterparty 'Morgan Stanley' and host counterparty id '9R7GPTSO7KV3UQJZQ078'.

2. Resolve security name 'ABB Ltd.' to host identifier CH0012530207.

3. Confirm trade date (host shows 2026-03-09) with the originator.

4. If enrichment confirms equivalence, close the documentation gap; otherwise request corrected trade details from sender.

---