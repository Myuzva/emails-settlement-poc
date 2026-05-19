# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review for manual processing.

**Reason:** The case requires human review due to an unsupported schema. The sender explicitly states a discrepancy in the instrument identifier, noting their records show Alphabet Inc. while the trade notification references Microsoft Corp.

---

## 2. Email Summary

**Email ID:** email_019.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Deutsche Bank

The sender reports a security mismatch for trade QR20201268. The sender has Alphabet Inc. on their books, but the trade notification references Microsoft Corp.

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

HOST lookup was not performed because the case was routed directly to human review due to an unsupported schema.

### Discrepancy Flags
- **wrong_security**: Sender has Alphabet Inc. on their books, but trade notification references Microsoft Corp.

---

## 6. Findings

The email explicitly states: "Our pre-settlement check for trade QR20201268 has flagged a discrepancy in the instrument identifier. We have Alphabet Inc. on our books, but the trade notification references Microsoft Corp.."
The case was routed to human review due to an unsupported schema.

---

## 7. Next Steps

1. Manually review the email and the attached `trade_details.pdf`.
2. Verify the correct security (Alphabet Inc. vs Microsoft Corp.) against internal trade booking records for trade QR20201268.
3. Contact the counterparty to resolve the security mismatch once internal records are verified.
4. Keep the case under analyst review until the discrepancy is resolved.
