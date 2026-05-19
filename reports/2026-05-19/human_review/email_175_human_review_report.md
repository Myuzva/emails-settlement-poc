# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review for manual processing.

**Reason:** The case requires human review due to an unsupported schema.

---

## 2. Email Summary

**Email ID:** email_175.eml  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Société Générale

The counterparty reports a settlement issue for a securities transaction and asks for confirmation of the expected settlement details.

---

## 3. Classification
- **Primary Type:** general_status_request (originally settlement_status_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

*No HOST lookup was performed as the case was routed to human review prior to HOST reconciliation.*

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | CS49526624 | N/A | N/A | N/A |
| security_isin | null | N/A | N/A | N/A |
| security_name | Microsoft Corp. | N/A | N/A | N/A |
| settlement_date | 2026-03-06 | N/A | N/A | N/A |
| trade_date | 2026-03-05 | N/A | N/A | N/A |
| quantity | 46524 | N/A | N/A | N/A |
| amount | 1861098.31 | N/A | N/A | N/A |
| currency | CHF | N/A | N/A | N/A |
| side | sell | N/A | N/A | N/A |
| counterparty_name | Société Générale | N/A | N/A | N/A |
| status | open | N/A | N/A | N/A |

### Discrepancy Flags
- None

---

## 6. Findings

The email was successfully classified as a settlement status request, and trade details were extracted with high confidence (0.99). However, the case was routed to human review due to an unsupported schema.

---

## 7. Next Steps

1. Analyst to review the email content and extracted trade details.
2. Manually verify the trade status in the HOST system.
3. Respond to the counterparty with the appropriate settlement status.
