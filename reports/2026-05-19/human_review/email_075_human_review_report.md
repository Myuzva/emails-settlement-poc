# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Low  

**Recommended Action:** Route to analyst review.

**Reason:** The email payload has an unsupported schema, requiring human review.

---

## 2. Email Summary

**Email ID:** email_075  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** BNP Paribas

The counterparty is following up regarding trade PK20518401, which is currently in open status with a forthcoming settlement date of 25-Mar-2026.

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

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | PK20518401 | N/A | not_performed | none |
| security_isin | null | N/A | not_performed | none |
| security_name | Goldman Sachs Group Inc. | N/A | not_performed | none |
| settlement_date | 2026-03-25 | N/A | not_performed | none |
| trade_date | 2026-03-24 | N/A | not_performed | none |
| quantity | 47767 | N/A | not_performed | none |
| amount | 1773795.02 | N/A | not_performed | none |
| currency | CHF | N/A | not_performed | none |
| side | sell | N/A | not_performed | none |
| counterparty_name | BNP Paribas | N/A | not_performed | none |
| status | open | N/A | not_performed | none |

### Discrepancy Flags
- None (HOST lookup not performed)

---

## 6. Findings

The email contains trade details for PK20518401, but the payload schema is unsupported (`unsupported_schema`), triggering a human review. HOST lookup was not performed.

---

## 7. Next Steps

1. Review the email and attachments manually.

2. Verify the trade details in the internal system.

3. Resolve the schema validation issue.

4. Keep the case under analyst review until the discrepancy is resolved.

---