# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Human review required before fully confirming the trade documentation request.

**Reason:** HOST counterparty is returned as an identifier while the email states the broker as Citigroup and counterparty enrichment was not completed.

---

## 2. Email Summary

**Email ID:** email_128.eml  
**Subject:** Reconciliation Query – FB01700321 – Roche Holding AG  
**Sender:** Claire Dubois <c.dubois@paribas-ops.fr>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Citigroup

The sender requests archival settlement confirmation or trade advice for a single closed trade.

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
| reference_number | FB01700321 | FB01700321 | match | none |
| security_isin | null | CH0012032048 | missing_in_email | none |
| security_name | Roche Holding AG | Roche Holding AG | match | none |
| settlement_date | 2026-03-30 | 2026-03-30 | match | none |
| trade_date | 2026-03-27 | 2026-03-27 | match | none |
| quantity | 68097 | 68097 | match | none |
| amount | 1394871.27 | 1394871.27 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | Citigroup | E57ODZWZ7FF32TWEFA76 | unknown | medium |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- counterparty_identifier_unresolved

---

## 6. Findings

HOST returned exactly one trade for reference number FB01700321. Reference number, settlement date, trade date, quantity, amount, currency, side, security, and status reconcile after safe normalization/enrichment. Security enrichment confirmed Roche Holding AG maps to HOST security identifier CH0012032048.

However, the counterparty cannot be confirmed from the available HOST response because HOST returned an identifier (E57ODZWZ7FF32TWEFA76) rather than the email's counterparty name (Citigroup).

---

## 7. Next Steps

1. Perform a counterparty lookup to prove equivalence between the identifier E57ODZWZ7FF32TWEFA76 and Citigroup.
2. Once the counterparty is verified, proceed with providing the requested archival documentation for trade FB01700321.
3. Keep the case under analyst review until the counterparty discrepancy is resolved.

---
