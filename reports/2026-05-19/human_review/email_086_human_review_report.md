# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Low  

**Recommended Action:** Route to analyst review for manual processing.

**Reason:** Human in the loop is required due to an unsupported schema.

---

## 2. Email Summary

**Email ID:** email_086.eml  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Nomura Securities

The counterparty is following up on trade SB50634868 in Apple Inc., due to settle on 2026-03-17.

---

## 3. Classification
- **Primary Type:** general_status_request (originally settlement_status_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** SB50634868 (Nomura Securities, USD 813,715.21)

---

## 5. HOST Lookup Comparison

*HOST lookup was not performed for this case due to the unsupported schema requiring human review.*

### Discrepancy Flags
- None

---

## 6. Findings

The email contains trade details for reference SB50634868, but the case was flagged for human review due to an unsupported schema. The extraction confidence is high (0.99), but manual validation is required to ensure the data aligns with internal systems.

---

## 7. Next Steps

1. Analyst to manually review the email and attachment (`trade_details.txt`).
2. Verify the trade details (Quantity: 49,362, Amount: 813,715.21 USD) against internal records.
3. Process the settlement status request manually.
