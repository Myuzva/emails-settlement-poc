# MAIA Settlement Mailbox Report - email_138.eml

**Status:** standard_processed
**Confidence Score:** 0.45 (Threshold: 0.72)

## Routing Metadata
- **Future Folder:** standard
- **Priority:** medium
- **Analyst Review Required:** true

## Source Metadata
- **Email File:** email_138.eml
- **Classification:** missing_confirmation (Secondary: generic_trade_details_request)

## Extracted Facts (Primary Trade)
- **Reference Number:** BY50062766
- **Counterparty:** Citigroup
- **Trade Date:** 2026-03-12
- **Settlement Date:** 2026-03-13
- **Quantity:** 18,856
- **Amount:** 1,163,259.25 CHF
- **Security:** Siemens AG
- **Side:** sell
- **Reported Status:** closed

## Multi-Trade Notes
This email contains multiple trades. 
- **Primary Trade:** BY50062766
- **Related Trade:** VI67093486 (Apple Inc., Buy, 68,644 EUR 1,575,378.23, Trade Date: 2026-03-17, Settlement Date: 2026-03-18)

## Evidence Snippets
- **Body:** "we are requesting the archival documentation for trade BY50062766, which is recorded as closed in our system." (Confidence: 0.99)
- **Attachment (trade_details.pdf):** "CHF 03/13/2026 1,163,259.25 Siemens AG 18,856 Citigroup Sale BY50062766 03/12/2026" (Confidence: 0.99)

## Attachment Extraction Status
- **trade_details.pdf:** parsed (Contains trade data: true, Contains multiple trades: true)

## HOST Lookup Summary
- **Status:** not_called
- **Planned Lookups:** 
  - GET /trades?reference_number=BY50062766
  - GET /trades?reference_number=VI67093486

## Side-by-Side Comparison
| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | BY50062766 | null | missing_in_host | high |
| security_name | Siemens AG | null | missing_in_host | medium |
| isin | null | null | unknown | low |
| trade_date | 2026-03-12 | null | missing_in_host | medium |
| settlement_date | 2026-03-13 | null | missing_in_host | medium |
| quantity | 18856 | null | missing_in_host | medium |
| amount | 1163259.25 | null | missing_in_host | medium |
| currency | CHF | null | missing_in_host | low |
| side | sell | null | missing_in_host | low |
| counterparty | Citigroup | null | missing_in_host | medium |
| reported_status | closed | null | missing_in_host | medium |

## Discrepancy Flags
- host_lookup_skipped
- requires_human_review
- multi_trade_email

## Recommended Action
- [ ] Approve and run the planned host lookups (GET /trades?reference_number=BY50062766 and optionally VI67093486)
- [ ] Include the parsed attachment (trade_details.pdf) when reconciling
- [ ] Verify archival/settlement documentation
- [ ] Request counterparty/security identifier lookups to reconcile naming if needed
- [ ] Document results and attach host responses to the case

## Draft Analyst Response Template
```text
Dear Citigroup,

Thank you for your message regarding trade BY50062766. 

We are currently retrieving the requested archival documentation and settlement confirmation for this closed trade from our systems. We have also noted the details for trade VI67093486 provided in the attachment.

We will provide the requested documentation to you shortly.

Best regards,
Settlement Operations
```

## Audit Trail
- **Workflow Branch:** standard
- **APIs Called:** None (Host lookup skipped)
- **Warnings:** 
  - Host lookup not executed; host_response_summary.count == 0.
  - Email references multiple trades (BY50062766 primary, VI67093486 related); ensure reviewer considers both.
  - ISIN missing from email/attachment — reviewer may need host security lookup to reconcile security identifiers.