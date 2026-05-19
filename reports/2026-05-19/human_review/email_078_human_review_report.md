# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review for manual processing.

**Reason:** Critical attachment extraction failed (`trade_details.jpg` inside ZIP could not be OCR'd) and multiple critical fields are missing. Security values conflict between sender records and confirmation.

---

## 2. Email Summary

**Email ID:** email_078.eml  
**Subject:** Clarification Required: Trade DY52987070  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Unknown  

The email reports a security mismatch for trade DY52987070. The sender booked Nestlé S.A., but the confirmation references Alphabet Inc. The sender requests clarification of the correct instrument before settlement.

---

## 3. Classification
- **Primary Type:** wrong_security (originally security_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

HOST lookup was not performed because the case was routed directly to human review due to attachment extraction failure and missing critical fields.

### Discrepancy Flags
- **wrong_security**: Sender booked Nestlé S.A., but confirmation references Alphabet Inc.

---

## 6. Findings

The email explicitly states: "Regarding trade DY52987070, our records indicate the traded security is Nestlé S.A.. However, the confirmation we received references Alphabet Inc."
The attachment `trade_details.zip` contained an image `trade_details.jpg` that failed OCR extraction, resulting in missing critical fields: counterparty, trade_date, settlement_date, quantity, currency, and net_amount.

---

## 7. Next Steps

1. Manually review the email and attempt to read the contents of `trade_details.jpg`.
2. Verify the correct security (Nestlé S.A. vs Alphabet Inc.) against internal trade booking records for trade DY52987070.
3. Confirm the missing trade details (counterparty, date, quantity, currency, amount).
4. Contact the counterparty to resolve the security mismatch once internal records are verified.

---
