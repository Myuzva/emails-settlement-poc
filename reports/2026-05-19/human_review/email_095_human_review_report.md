# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review.

**Reason:** Subject indicates one additional trade and PDF contains two trade rows without trade references, so relation to OI96432964 is unclear. Attachment trade rows lack settlement dates and trade references.

---

## 2. Email Summary

**Email ID:** email_095  
**Subject:** Outstanding Trade – Action Required – OI96432964 (+ 1 more)  
**Sender:** Michael Hartmann <m.hartmann@eurofin.de>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Unknown

Sender reports incomplete documentation and requests missing complete trade details for settled transactions.

---

## 3. Classification
- **Primary Type:** instruction_or_document_update (originally documentation_missing)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** 
  - Commerzbank, Novartis AG, CHF 264227.02
  - Santander, Microsoft Corp., USD 903083.00

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | OI96432964 | N/A | N/A | none |
| security_isin | null | N/A | N/A | none |
| security_name | null | N/A | N/A | none |
| settlement_date | null | N/A | N/A | none |
| trade_date | null | N/A | N/A | none |
| quantity | null | N/A | N/A | none |
| amount | null | N/A | N/A | none |
| currency | null | N/A | N/A | none |
| side | unknown | N/A | N/A | none |
| counterparty_name | null | N/A | N/A | none |
| status | closed | N/A | N/A | none |

### Discrepancy Flags
- Documentation missing: Sender reports incomplete documentation on file; recorded as closed. Expected: complete trade details / missing information.

---

## 6. Findings

The email references trade OI96432964, which is recorded as closed but has incomplete documentation. The attachment contains two trade rows (Commerzbank and Santander) but lacks trade references and settlement dates, making it impossible to confidently map them to OI96432964.

---

## 7. Next Steps

1. Review the attached trade details and manually link them to the correct trade references.
2. Verify the documentation status for trade OI96432964.
3. Provide the missing complete trade details to the sender.
4. Keep the case under analyst review until the ambiguity is resolved.

---