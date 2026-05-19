# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required. Verify the correct security/ISIN and determine whether re-booking or correction is required.

**Reason:** HOST trade MB75276355 matches the economic details and counterparty, but HOST security identifier DE000BASF111 does not match the security enrichment for the email security name Swiss Re AG, which returned ISIN CH0126881561.

---

## 2. Email Summary

**Email ID:** email_104.eml  
**Subject:** Reconciliation Query – MB75276355 – Swiss Re AG  
**Sender:** James O'Brien <j.obrien@meridianfunds.co.uk>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Citigroup

The sender reports an instrument identifier/security discrepancy: their books show BASF SE while the trade notification references Swiss Re AG; asks to verify correct ISIN.

---

## 3. Classification
- **Primary Type:** security_mismatch (originally security_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | MB75276355 | MB75276355 | match | none |
| security_isin | null | DE000BASF111 | missing_in_email | none |
| security_name | Swiss Re AG | DE000BASF111 | mismatch | high |
| settlement_date | 2026-03-10 | 2026-03-10 | match | none |
| trade_date | 2026-03-09 | 2026-03-09 | match | none |
| quantity | 21635 | 21635 | match | none |
| amount | 1546104.19 | 1546104.19 | match | none |
| currency | USD | USD | match | none |
| side | buy | Buy | match | none |
| counterparty_name | Citigroup | E57ODZWZ7FF32TWEFA76 | match | none |
| status | unknown | Open | missing_in_email | none |

### Discrepancy Flags
- security_identifier_mismatch
- security_name_mismatch

---

## 6. Findings

HOST returned exactly one trade for reference MB75276355. Reference number, trade date, settlement date, side, quantity, amount, currency, and counterparty reconcile after safe normalization/enrichment. Counterparty enrichment maps Citigroup to the HOST counterparty LEI E57ODZWZ7FF32TWEFA76. 

Security comparison shows a material mismatch: email references Swiss Re AG while HOST security is DE000BASF111; security lookup for Swiss Re AG returned CH0126881561. The email itself reports a security discrepancy: sender says their books show BASF SE while the trade notification references Swiss Re AG.

---

## 7. Next Steps

1. Verify the correct security/ISIN (Swiss Re AG vs BASF SE) against internal trade booking records.

2. Determine whether re-booking or correction is required.

3. Contact the counterparty to confirm the correct security and resolve the discrepancy.

4. Keep the case under analyst review until the discrepancy is resolved.
