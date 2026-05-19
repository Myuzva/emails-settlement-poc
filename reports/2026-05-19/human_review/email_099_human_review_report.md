# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Unknown (Schema Validation Failed)

**Priority:** High  

**Recommended Action:** Route to analyst review for manual processing.

**Reason:** The payload schema `maia.email_case_payload.v1` is not supported for canonicalization in workflow 1. The case could not be processed automatically.

---

## 2. Email Summary

**Email ID:** email_099.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Unknown (Raw payload indicates Société Générale)

The email could not be processed due to an unsupported schema version. Raw payload data suggests a request for final trade confirmation or SWIFT confirmation for trade QQ15669741 (Meta Platforms Inc., Buy, 34,657 @ USD 1,773,667.56).

---

## 3. Classification
- **Primary Type:** unsupported_schema
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

HOST lookup was not performed because the case was routed directly to human review due to an unsupported input schema.

### Discrepancy Flags
- **unsupported_schema**: payload schema maia.email_case_payload.v1 is not supported for canonicalization in workflow 1.

---

## 6. Findings

The automated workflow failed to canonicalize the input payload because the schema version (`maia.email_case_payload.v1`) is not supported in workflow 1. As a result, no structured facts were extracted into the canonical format, and no HOST lookup was performed.

---

## 7. Next Steps

1. Manually review the email `email_099.eml` and its attachments (`trade_details.zip`).
2. Verify the trade details (QQ15669741) against internal trade booking records.
3. Provide the requested final trade confirmation or SWIFT confirmation to the counterparty if the trade is found and settled.
4. Investigate the upstream system generating the unsupported schema version `maia.email_case_payload.v1` to ensure compatibility with workflow 1.

---
