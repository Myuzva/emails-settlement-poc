# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required to verify whether email counterparty name Nordbank corresponds to HOST counterparty identifier W22LROWP2IHZNBB6K528.

**Reason:** Counterparty remains unresolved because HOST returned an identifier while email provided a name, and /counterparty lookup for Nordbank returned no match.

---

## 2. Email Summary

**Email ID:** email_097  
**Subject:** Follow-up: Sale of Novartis AG dated 2026-03-30 (+ 1 more)  
**Sender:** Sarah Jensen <s.jensen@nordbank.com>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Nordbank

The sender reports their record for the closed trade is incomplete and requests missing details for reconciliation and archiving.

---

## 3. Classification
- **Primary Type:** generic_trade_details_request (originally generic_trade_details_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** KY05031605 (Deutsche Bank AG, CHF 656475.65)

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | QZ85525941 | QZ85525941 | match | none |
| security_isin | null | CH0012221716 | missing_in_email | none |
| security_name | Novartis AG | Novartis AG | match | none |
| settlement_date | 2026-03-30 | 2026-03-30 | match | none |
| trade_date | 2026-03-27 | 2026-03-27 | match | none |
| quantity | 45458 | 45458 | match | none |
| amount | 1141321.88 | 1141321.88 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty_name | Nordbank | W22LROWP2IHZNBB6K528 | unknown | medium |
| status | closed | Closed | match | none |

### Discrepancy Flags
- counterparty_identifier_unresolved
- counterparty_enrichment_no_match

---

## 6. Findings

Primary trade was found by exact reference number QZ85525941 with a single HOST match. Settlement date, trade date, quantity, amount, currency, side, and status match after safe normalization. Email security name Novartis AG was enriched through /security and maps to HOST ISIN CH0012221716. Counterparty remains unresolved because HOST returned an identifier while email provided a name, and /counterparty lookup for Nordbank returned no match.

---

## 7. Next Steps

1. Verify whether email counterparty name Nordbank corresponds to HOST counterparty identifier W22LROWP2IHZNBB6K528.
2. Review the related trade KY05031605 if necessary, as it was not queried per PoC instructions.
3. Once counterparty is verified, provide the missing trade details to the sender for their reconciliation and archiving.
