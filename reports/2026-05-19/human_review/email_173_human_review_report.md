# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Route to analyst review for manual verification.

**Reason:** Critical attachment extraction failed (OCR returned no text for trade_details.jpg) and there are conflicting amount values within the same email body.

---

## 2. Email Summary

**Email ID:** email_173.eml  
**Subject:** Outstanding Trade – Action Required – VO00624838  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Unknown

The sender reports a trade amount variance between internal records and received documentation for trade VO00624838.

---

## 3. Classification
- **Primary Type:** wrong_amount (originally amount_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

*Note: HOST lookup was not performed as this case requires human review due to extraction failures and data conflicts.*

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | VO00624838 | N/A | N/A | none |
| security_isin | null | N/A | N/A | none |
| security_name | null | N/A | N/A | none |
| settlement_date | null | N/A | N/A | none |
| trade_date | null | N/A | N/A | none |
| quantity | null | N/A | N/A | none |
| amount | 1946833.17 / 1049328.73 | N/A | N/A | none |
| currency | CHF | N/A | N/A | none |
| side | unknown | N/A | N/A | none |
| counterparty_name | null | N/A | N/A | none |
| status | open | N/A | N/A | none |

### Discrepancy Flags
- **Amount Mismatch:** Sender records indicate 1,946,833.17 CHF, but received documentation states 1,049,328.73 CHF.

---

## 5. Findings

The email contains conflicting amount values (1,946,833.17 CHF vs 1,049,328.73 CHF) for trade VO00624838. Additionally, a critical attachment (`trade_details.zip/trade_details.jpg`) could not be processed due to OCR failure, meaning crucial trade details might be missing from the extracted facts.

---

## 6. Next Steps

1. Manually review the attached `trade_details.jpg` to extract the correct trade details.

2. Verify the correct settlement amount against internal trade booking records for trade VO00624838.

3. Contact the sender to clarify the discrepancy between their records and the documentation.

4. Keep the case under analyst review until the correct amount is confirmed and the discrepancy is resolved.

---