# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Low  

**Recommended Action:** Route to analyst review due to unsupported schema.

**Reason:** The case requires human review because of an unsupported schema.

---

## 2. Email Summary

**Email ID:** email_176.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Morgan Stanley

The counterparty is following up on trade ME19312140 in Roche Holding AG, due to settle on 17.03.2026.

---

## 3. Classification
- **Primary Type:** settlement_status_request
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

*Note: No HOST lookup was performed as per instructions.*

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | ME19312140 | N/A | N/A | none |
| security_isin | null | N/A | N/A | none |
| security_name | Roche Holding AG | N/A | N/A | none |
| settlement_date | 2026-03-17 | N/A | N/A | none |
| trade_date | 2026-03-16 | N/A | N/A | none |
| quantity | 88389 | N/A | N/A | none |
| amount | 1212017.91 | N/A | N/A | none |
| currency | EUR | N/A | N/A | none |
| side | sell | N/A | N/A | none |
| counterparty_name | Morgan Stanley | N/A | N/A | none |
| status | unknown | N/A | N/A | none |

### Discrepancy Flags
- None

---

## 5. Findings

The case was routed to human review due to an unsupported schema. Trade details were successfully extracted from the email body and the attached image (`trade_details.jpg`), but the payload structure requires manual validation.

---

## 6. Next Steps

1. Review the extracted trade details against the original email and attachment.
2. Validate the schema and ensure all required fields are correctly mapped.
3. Proceed with standard processing once the schema issue is resolved.

---