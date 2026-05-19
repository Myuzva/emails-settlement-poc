# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Route to analyst review for manual inspection of the unparsed attachment and resolution of the amount discrepancy.

**Reason:** Human review is required because a nested image attachment (`trade_details.jpg` inside `trade_details.zip`) could not be OCR-extracted and may contain trade-critical data. Additionally, there is a reported amount mismatch (Sender: CHF 1,946,833.17 vs Documentation: CHF 1,049,328.73).

---

## 2. Email Summary

**Email ID:** email_173  
**Subject:** Outstanding Trade – Action Required – VO00624838  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** 2026-04-28 13:38 UTC  
**Counterparty:** Unknown  

The sender reports a discrepancy in the trade amount for trade VO00624838, stating their records indicate CHF 1,946,833.17 while the received documentation states CHF 1,049,328.73.

---

## 3. Classification
- **Primary Type:** amount_mismatch (originally amount_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

*Note: HOST lookup was not performed as the case was routed directly to human review due to critical attachment extraction failure.*

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | VO00624838 | N/A | missing_in_host | none |
| security_isin | null | N/A | missing_in_email | none |
| security_name | null | N/A | missing_in_email | none |
| settlement_date | null | N/A | missing_in_email | none |
| trade_date | null | N/A | missing_in_email | none |
| quantity | null | N/A | missing_in_email | none |
| amount | 1946833.17 | N/A | missing_in_host | none |
| currency | CHF | N/A | missing_in_host | none |
| side | unknown | N/A | missing_in_host | none |
| counterparty_name | null | N/A | missing_in_email | none |
| status | unknown | N/A | missing_in_host | none |

### Discrepancy Flags
- **Amount Mismatch:** Sender reports CHF 1,946,833.17, but documentation states CHF 1,049,328.73.

---

## 5. Findings

The email highlights a significant amount discrepancy for trade VO00624838. The sender's records show CHF 1,946,833.17, whereas the documentation they received states CHF 1,049,328.73. Furthermore, a nested image attachment (`trade_details.jpg` inside `trade_details.zip`) failed OCR extraction, meaning critical evidence regarding the discrepancy could not be automatically parsed.

---

## 6. Next Steps

1. Manually review the unparsed attachment (`trade_details.jpg`) to extract the correct trade details and documentation values.
2. Perform a manual HOST lookup using trade reference VO00624838 to verify the correct settlement amount.
3. Investigate the root cause of the CHF 1,946,833.17 vs CHF 1,049,328.73 discrepancy.
4. Contact the sender (Anna Kowalski) to clarify the correct amount and resolve the mismatch.

---