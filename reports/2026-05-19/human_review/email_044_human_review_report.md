# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Low  

**Recommended Action:** Route to analyst review for manual processing.

**Reason:** The case requires human review due to an unsupported schema.

---

## 2. Email Summary

**Email ID:** email_044.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** ING Bank

The email requests confirmation of pre-settlement checks and funding for an open trade.

---

## 3. Classification
- **Primary Type:** settlement_status_request
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

*No HOST lookup was performed for this case.*

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | SH74049231 | N/A | N/A | N/A |
| security_isin | null | N/A | N/A | N/A |
| security_name | Tesla Inc. | N/A | N/A | N/A |
| settlement_date | 2026-03-06 | N/A | N/A | N/A |
| trade_date | 2026-03-05 | N/A | N/A | N/A |
| quantity | 14149 | N/A | N/A | N/A |
| amount | 927089.27 | N/A | N/A | N/A |
| currency | EUR | N/A | N/A | N/A |
| side | buy | N/A | N/A | N/A |
| counterparty_name | ING Bank | N/A | N/A | N/A |
| status | open | N/A | N/A | N/A |

### Discrepancy Flags
- None

---

## 6. Findings

The email was classified as a settlement status request with high confidence (0.95). However, the payload schema was marked as unsupported, triggering a mandatory human review. The extracted data indicates an open buy trade for Tesla Inc. with ING Bank.

**Evidence:** "We are conducting our standard pre-settlement review and note that trade SH74049231 remains open with a settlement date of 06-Mar-2026."

---

## 7. Next Steps

1. Analyst to manually review the email content and verify the extracted trade details.
2. Perform a manual HOST lookup for trade SH74049231 to confirm its status.
3. Respond to the counterparty regarding the pre-settlement review and funding status.
