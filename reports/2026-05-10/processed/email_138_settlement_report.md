# MAIA Settlement Mailbox Report - email_138.eml

**Status:** standard_processed
**Confidence Score:** 0.85 (Threshold: 0.72)

## Routing Metadata
- **Future Folder:** standard
- **Priority:** medium
- **Analyst Review Required:** true

## Source Metadata
- **Email File:** email_138.eml
- **Path:** emails/email_138.eml

## Classification
- **Primary Type:** missing_confirmation
- **Secondary Types:** generic_trade_details_request

## Extracted Facts
- **Primary Trade Reference:** BY50062766
- **Counterparty:** Citigroup
- **Security:** Siemens AG
- **Trade Date:** 2026-03-12
- **Settlement Date:** 2026-03-13
- **Side:** sell
- **Quantity:** 18,856
- **Amount:** 1,163,259.25 CHF
- **Reported Status:** closed

## Multi-Trade Notes
This email contains multiple trades. 
- **Primary Trade:** BY50062766 (Siemens AG, Sell, 18,856)
- **Related Trade:** VI67093486 (Apple Inc., Buy, 68,644)

## Evidence Snippets
- **Body:** "we are requesting the archival documentation for trade BY50062766, which is recorded as closed in our system." (Supports: classification.primary_type, extracted_data.reported_status)
- **Attachment (trade_details.pdf):** "CHF 03/13/2026 1,163,259.25 Siemens AG 18,856 Citigroup Sale BY50062766 03/12/2026" (Supports: quantity, net_amount)

## Attachment Extraction Status
- **File:** trade_details.pdf
- **Status:** parsed (pdf_text)
- **Contains Trade Data:** Yes
- **Contains Multiple Trades:** Yes

## HOST Lookup Summary
- **Status:** not_called
- **Lookup Plan:** 
  - `/trades` by_trade_reference (BY50062766)
  - `/trades` by_trade_reference (VI67093486)

## Side-by-Side Comparison
| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| trade_reference | BY50062766 | null | unknown | high |
| security_name | Siemens AG | null | unknown | medium |
| isin | null | null | unknown | low |
| settlement_date | 2026-03-13 | null | unknown | high |
| trade_date | 2026-03-12 | null | unknown | medium |
| quantity | 18856 | null | unknown | medium |
| amount | 1163259.25 | null | unknown | high |
| currency | CHF | null | unknown | medium |
| side | sell | null | unknown | low |
| counterparty | Citigroup | null | unknown | medium |

## Discrepancy Flags
- host_lookup_not_performed
- multi_trade_email
- requires_human_review

## Recommended Action
Perform manual host verification for primary trade BY50062766 (and related trade VI67093486 if needed). Query host endpoint /trades?reference=BY50062766 and confirm settlement_date=2026-03-13, quantity=18,856, amount=1,163,259.25 CHF, instrument=Siemens AG, counterparty=Citigroup. If automated host access is available, run lookups by trade reference and then reconcile any mismatches; otherwise attach host evidence obtained manually to this case and complete human review.

## Draft Analyst Response Template
```text
Dear Citigroup,

Thank you for your inquiry. Please find attached the requested archival documentation and settlement confirmation for trade BY50062766 (Siemens AG), which successfully settled on our end on 2026-03-13. 

If you also require documentation for the related trade VI67093486, please let us know.

Best regards,
Settlements Team
```

## Audit Trail
- **Workflow Branch:** standard
- **APIs Called:** None (HOST lookup not performed)
- **Warnings:** 
  - HOST queries were not executed (no live host access in this environment).
  - Attachment contains multiple trades; ensure reviewer selects correct trade when querying the host.
  - If host records use different identifiers (ISIN/sedol/other), run security and counterparty lookups as needed during manual review.