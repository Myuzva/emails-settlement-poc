# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review.

**Reason:** The case requires human review due to an unsupported schema (missing confirmation for a closed trade).

---

## 2. Email Summary

**Email ID:** email_197  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Morgan Stanley

The sender requires the final confirmation slip / trade advice for audit purposes for a closed trade.

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

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | YZ85103017 | N/A | N/A | none |
| security_isin | null | N/A | N/A | none |
| security_name | Goldman Sachs Group Inc. | N/A | N/A | none |
| settlement_date | 2026-03-20 | N/A | N/A | none |
| trade_date | 2026-03-19 | N/A | N/A | none |
| quantity | 87805 | N/A | N/A | none |
| amount | 932975.05 | N/A | N/A | none |
| currency | CHF | N/A | N/A | none |
| side | buy | N/A | N/A | none |
| counterparty_name | Morgan Stanley | N/A | N/A | none |
| status | closed | N/A | N/A | none |

### Discrepancy Flags
- missing_confirmation: Sender requires the final confirmation slip / trade advice for audit purposes.

---

## 6. Findings

The email requests a final confirmation slip for trade YZ85103017 for audit purposes. The trade is reported as closed. The case requires human review due to an unsupported schema.

---

## 7. Next Steps

1. Review the request for the confirmation slip.
2. Verify the trade status and details internally.
3. Provide the requested trade advice/execution confirmation to the counterparty.
4. Keep the case under analyst review until the request is fulfilled.

---