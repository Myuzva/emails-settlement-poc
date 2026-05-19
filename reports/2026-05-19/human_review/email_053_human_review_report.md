# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Route to human review.

**Reason:** HOST settlement date matches the email's expected settlement date, but the email trade date differs materially from HOST transaction date; verify whether the extracted trade date is correct and whether any amendment is actually required.

---

## 2. Email Summary

**Email ID:** email_053.eml  
**Subject:** Trade Status Update Request – KR86473518  
**Sender:** Claire Dubois <c.dubois@paribas-ops.fr>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Merrill Lynch

The sender reports a settlement date inconsistency on trade KR86473518 and asks how to correct it, expecting settlement on 2026-03-20.

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
| reference_number | KR86473518 | KR86473518 | match | none |
| security_isin | null | US0378331005 | missing_in_email | none |
| security_name | Apple Inc. | Apple Inc. | match | none |
| settlement_date | 2026-03-20 | 2026-03-20 | match | none |
| trade_date | 2026-03-26 | 2026-03-19 | mismatch | high |
| quantity | 85772 | 85772 | match | none |
| amount | 1549075.48 | 1549075.48 | match | none |
| currency | EUR | EUR | match | none |
| side | buy | Kauf | match | none |
| counterparty_name | Merrill Lynch | Merrill Lynch | match | none |
| counterparty_lei | null | FAK6QKWT97JDDAHS3S03 | missing_in_email | none |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- trade_date_mismatch
- reported_settlement_date_matches_host
- security_identifier_resolved_by_enrichment
- counterparty_identifier_resolved_by_enrichment

---

## 6. Findings

The trade was found in HOST by exact reference number. Core economic fields (settlement date, quantity, amount, currency, side, security, counterparty, and status) reconcile after safe enrichment and translation.

However, the email trade date (2026-03-26) materially differs from the HOST transaction date (2026-03-19). Additionally, the attachment trade date (2026-03-26) is later than the settlement date (2026-03-20), which is highly unusual and likely an error in the source document.

---

## 7. Next Steps

1. Verify the correct trade date against internal trade booking records and the original source document.
2. Confirm whether the counterparty's expected settlement date (2026-03-20) is already correctly reflected in HOST, meaning no amendment may be necessary.
3. Clarify the trade date discrepancy with the counterparty if needed.
4. Keep the case under analyst review until the discrepancy is resolved.

---