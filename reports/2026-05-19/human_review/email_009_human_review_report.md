# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Request clarification from counterparty and route to analyst review.

**Reason:** Conflicting settlement date values are stated in the email: internal booking 2026-03-23 versus instruction/table value 2026-04-23.

---

## 2. Email Summary

**Email ID:** email_009.eml  
**Subject:** Trade Confirmation Request – BP86251923  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** HSBC

The sender reports a value date mismatch and requests confirmation of the correct settlement date.

---

## 3. Classification
- **Primary Type:** wrong_date (originally settlement_date_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

*HOST lookup was not performed for this case.*

### Discrepancy Flags
- **settlement_date_mismatch**: Sender reports a value date mismatch and requests confirmation of the correct settlement date. Sender value: 2026-03-23, Expected/Requested value: 2026-04-23.

---

## 5. Findings

The email contains two settlement date values due to the reported mismatch; extracted settlement_date uses the instruction/table value. Conflicting settlement date values require human review.

---

## 6. Next Steps

1. Verify the correct settlement date against internal trade booking records.

2. Confirm whether the counterparty is referencing the same trade reference.

3. Ask the counterparty to confirm the expected settlement date.

4. Keep the case under analyst review until the discrepancy is resolved.

---