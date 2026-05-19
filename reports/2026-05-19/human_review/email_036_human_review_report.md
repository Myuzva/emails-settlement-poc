# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Low  

**Recommended Action:** Route to analyst review for manual processing.

**Reason:** The case requires human review due to an unsupported schema validation issue.

---

## 2. Email Summary

**Email ID:** email_036.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Raiffeisen Bank

The sender is requesting archival documentation/settlement confirmation for a closed trade. Trade details were extracted from the attached image.

---

## 3. Classification
- **Primary Type:** missing_confirmation (originally confirmation_missing)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

HOST lookup was not performed because the case was routed directly to human review due to an unsupported schema validation issue.

### Discrepancy Flags
- None

---

## 6. Findings

The email explicitly states: "we are requesting the archival documentation for trade UH78032934, which is recorded as closed in our system."
The attachment `trade_details.jpg` was successfully parsed and contains the trade details: Quantity: 91177, Notional: 235149.90, Counterpart: Raiffeisen Bank, Trans Dt: 03/04/2026, Settlement Date: 03/05/2026, Asset: UBS Group AG, Buy Sale: Sale, Currency: USD.
However, the case was flagged for human review due to `unsupported_schema`.

---

## 7. Next Steps

1. Manually review the email and the extracted trade details.
2. Verify the trade UH78032934 against internal trade booking records.
3. Confirm the trade details (date, quantity, currency, amount, side) match the internal records.
4. Provide the requested archival documentation/settlement confirmation to the counterparty once internal records are verified.
