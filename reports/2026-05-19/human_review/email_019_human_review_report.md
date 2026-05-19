# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review to verify the correct ISIN and resolve the instrument conflict.

**Reason:** Instrument values conflict inside the email: Alphabet Inc. on sender books vs Microsoft Corp. in notification/attachment. Sender requests verification of the correct ISIN and whether re-booking is required.

---

## 2. Email Summary

**Email ID:** email_019  
**Subject:** Unmatched Trade – Microsoft Corp. – QR20201268  
**Sender:** Unknown (Message ID: <177738352767.31976.18357420564104303561@Arek.yallo.box>)  
**Received:** Unknown  
**Counterparty:** Deutsche Bank

The sender reports a discrepancy in the instrument identifier for trade QR20201268, noting Alphabet Inc. on their books but Microsoft Corp. in the trade notification and attachment.

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

*Note: HOST lookup was not performed as the case requires human review due to internal email conflicts.*

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | QR20201268 | N/A | N/A | N/A |
| security_isin | null | N/A | N/A | N/A |
| security_name | Microsoft Corp. (Alphabet Inc. claimed) | N/A | N/A | N/A |
| settlement_date | 2026-03-10 | N/A | N/A | N/A |
| trade_date | 2026-03-09 | N/A | N/A | N/A |
| quantity | 75634 | N/A | N/A | N/A |
| amount | 605945.09 | N/A | N/A | N/A |
| currency | EUR | N/A | N/A | N/A |
| side | buy | N/A | N/A | N/A |
| counterparty_name | Deutsche Bank | N/A | N/A | N/A |
| status | unknown | N/A | N/A | N/A |

### Discrepancy Flags
- **security_mismatch**: Sender states their books show Alphabet Inc. while the trade notification and attached trade details reference Microsoft Corp.; requests correct ISIN verification.

---

## 6. Findings

The email contains conflicting instrument information. The sender's books show "Alphabet Inc.", but the trade notification and the attached PDF ("trade_details.pdf") reference "Microsoft Corp." for trade QR20201268.

The likely cause of the settlement break is a security mismatch. The case should be reviewed before any re-booking or correction is performed.

---

## 7. Next Steps

1. Verify the correct ISIN and instrument name against internal trade booking records for trade QR20201268.
2. Confirm whether re-booking is required based on the correct instrument.
3. Communicate the correct instrument details to the counterparty.
4. Keep the case under analyst review until the discrepancy is resolved.

---