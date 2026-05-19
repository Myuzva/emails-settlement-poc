# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Normal  

**Recommended Action:** Route to analyst review for manual processing.

**Reason:** Extracted security values conflict: Alphabet Inc. in sender books vs Microsoft Corp. in notification/attachment. Correct ISIN is requested but not present in the email or attachment.

---

## 2. Email Summary

**Email ID:** email_019.eml  
**Subject:** Unmatched Trade – Microsoft Corp. – QR20201268  
**Sender:** Thomas Müller <t.mueller@rheinasset.de>  
**Received:** Tue, 28 Apr 2026 15:38:47 +0200  
**Counterparty:** Deutsche Bank

The sender reports a discrepancy in the instrument identifier for trade QR20201268. Their books show Alphabet Inc., but the trade notification references Microsoft Corp. They request verification of the correct ISIN.

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

HOST lookup was not performed because the case was routed directly to human review due to a security mismatch and missing ISIN.

### Discrepancy Flags
- **security_mismatch**: Instrument identifier/security mismatch: sender books show Alphabet Inc., while trade notification and attachment reference Microsoft Corp.; correct ISIN requested.

---

## 6. Findings

The email explicitly states: "trade QR20201268 has flagged a discrepancy in the instrument identifier. We have Alphabet Inc. on our books, but the trade notification references Microsoft Corp."
The sender requests verification of the correct ISIN, but no ISIN is present in the email or attachment.
The PDF attachment `trade_details.pdf` provides trade details for Microsoft Corp. matching the notification.

---

## 7. Next Steps

1. Manually review the email and the attached `trade_details.pdf`.
2. Verify the correct security (Alphabet Inc. vs Microsoft Corp.) and the correct ISIN against internal trade booking records for trade QR20201268.
3. Advise the counterparty whether a re-booking is required prior to the value date.
4. Keep the case under analyst review until the security discrepancy is resolved.

---
