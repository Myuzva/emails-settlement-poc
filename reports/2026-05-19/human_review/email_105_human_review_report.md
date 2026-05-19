# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review for manual processing and discrepancy resolution.

**Reason:** Human review is required because extracted values conflict inside the same email/thread (value date conflict).

---

## 2. Email Summary

**Email ID:** email_105.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Raiffeisen Bank

The counterparty reports a value date mismatch on trade MU50046625. Their internal booking reflects 05-Mar-2026, whereas the instruction indicates 19-Feb-2026.

---

## 3. Classification
- **Primary Type:** settlement_date_mismatch
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

HOST lookup was not performed because the case was routed directly to human review due to conflicting extracted values and a value date mismatch.

### Discrepancy Flags
- **settlement_date_mismatch**: Value date mismatch between internal booking and instruction. Sender value: 2026-03-05, Expected: 2026-02-19.

---

## 6. Findings

The email explicitly states: "We have identified a value date mismatch on trade MU50046625. Our internal booking reflects 05-Mar-2026, whereas the instruction received from your side indicates 19-Feb-2026."

The attachment `trade_details.zip` was successfully parsed and contains the following trade details: "Stlmt Date 19-Feb-2026 Net Amount 157516.59 Asset Microsoft Corp. Cpty Raiffeisen Bank Exec Date 04-Mar-2026 Trade Ref MU50046625 Face Amt 63414 Direction Verkauf Currency EUR".

The case requires human review due to conflicting settlement date values (value date conflict) inside the same email/thread.

---

## 7. Next Steps

1. Verify the correct settlement date against internal trade booking records for trade MU50046625.
2. Confirm whether the counterparty's internal booking date (05-Mar-2026) or the instruction date (19-Feb-2026) is correct.
3. Contact the counterparty to resolve the settlement date mismatch once internal records are verified.
4. Keep the case under analyst review until the discrepancy is resolved.

---
