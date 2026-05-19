# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review for manual processing.

**Reason:** The case requires human review due to an unsupported schema and multi-trade ambiguity.

---

## 2. Email Summary

**Email ID:** email_067.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** HSBC

The sender flagged a potential amount mismatch on trade KV78386940. The figure in their system is 588,790.65 CHF, whereas the counterparty notification reflects 394,329.00 CHF.

---

## 3. Classification
- **Primary Type:** wrong_amount (originally amount_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** Unreferenced trade (BNP Paribas, Nestlé S.A., CHF 1,310,952.25)

---

## 5. HOST Lookup Comparison

HOST lookup was not performed because the case was routed directly to human review due to unsupported schema and multi-trade ambiguity.

### Discrepancy Flags
- **amount_mismatch**: Sender value 588,790.65 CHF, expected or requested value 394,329.00 CHF.

---

## 6. Findings

The email explicitly states: "We have flagged a potential amount mismatch on trade KV78386940. The figure in our system is 588 790.65 CHF, whereas the counterparty notification reflects 394 329.00 CHF."
The attachment `trade_details.pdf` contains multiple trades, including a secondary trade for BNP Paribas (Nestlé S.A., CHF 1,310,952.25). The case was flagged for human review due to an unsupported schema.

---

## 7. Next Steps

1. Manually review the email and the attached `trade_details.pdf`.
2. Verify the correct settlement amount for trade KV78386940 against internal trade booking records.
3. Investigate the secondary trade (BNP Paribas) to determine if any action is required.
4. Contact the counterparty to resolve the amount mismatch once internal records are verified.

---
