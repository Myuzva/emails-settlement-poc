# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review for manual trade linkage and clarification.

**Reason:** Several trades are present and the primary trade linkage for attachment rows is unclear. Additional trade has no trade reference. Fallback lookup fields are incomplete for attachment rows because settlement date and ISIN are missing.

---

## 2. Email Summary

**Email ID:** email_095  
**Subject:** Outstanding Trade – Action Required – OI96432964 (+ 1 more)  
**Sender:** Michael Hartmann <m.hartmann@eurofin.de>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Unknown

The sender reports incomplete documentation for trade OI96432964 and requests complete trade details to update audit records. The attachment contains multiple unreferenced trades.

---

## 3. Classification
- **Primary Type:** instruction_or_document_update (originally documentation_missing)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** OI96432964 (Primary), Unreferenced Trade 1 (Commerzbank, Novartis AG, CHF 264227.02), Unreferenced Trade 2 (Santander, Microsoft Corp., USD 903083.00)

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | OI96432964 | N/A | not_looked_up | none |
| security_isin | null | N/A | not_looked_up | none |
| security_name | null | N/A | not_looked_up | none |
| settlement_date | null | N/A | not_looked_up | none |
| trade_date | null | N/A | not_looked_up | none |
| quantity | null | N/A | not_looked_up | none |
| amount | null | N/A | not_looked_up | none |
| currency | null | N/A | not_looked_up | none |
| side | unknown | N/A | not_looked_up | none |
| counterparty_name | null | N/A | not_looked_up | none |
| status | closed | N/A | not_looked_up | none |

### Discrepancy Flags
- Sender reports incomplete documentation on file and requests complete trade details.

---

## 6. Findings

The email references trade OI96432964 with incomplete documentation. The attachment contains two trade-detail rows without trade references, settlement dates, or ISINs. It is unclear how the attachment rows link to the primary trade OI96432964. No HOST lookup was performed due to missing critical fields and ambiguity.

---

## 7. Next Steps

1. Review the attachment to manually identify the trades.
2. Clarify with the sender which trade details correspond to OI96432964.
3. Update the documentation for the relevant trades once identified.

---