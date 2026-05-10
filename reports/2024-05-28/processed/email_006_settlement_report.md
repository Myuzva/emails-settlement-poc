# MAIA Settlement Mailbox Report - email_006.eml

- **Status**: standard_processed
- **Confidence Score**: 0.96 (Threshold: 0.72)
- **Routing Metadata**:
  - Future Folder: standard
  - Priority: low
  - Analyst Review Required: false
- **Source Metadata**:
  - Email File: email_006.eml
  - Path: emails/email_006.eml
- **Classification**: missing_confirmation (Confidence: 0.98)

## Extracted Facts
- **Trade Reference**: BF92476064
- **Counterparty**: Société Générale
- **Security**: Tesla Inc.
- **Trade Date**: 2026-03-12
- **Settlement Date**: 2026-03-13
- **Side**: sell
- **Quantity**: 11303
- **Amount**: 999202.27 EUR
- **Reported Status**: closed

## Attachment Extraction Status
- **Count**: 0
- **All Processed**: true

## Evidence Snippets
- "require the final confirmation slip for trade BF92476064" (Source: body)
- "BF92476064  12-Mar-2026  Sale  Société Générale  999202.27   Tesla Inc.  EUR  13-Mar-2026  11303" (Source: body)

## HOST Lookup Summary
- **Status**: matched
- **Lookup Strategy**: by_trade_reference
- **Host Records Found**: 1

### Side-by-Side Comparison
| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | BF92476064 | BF92476064 | match | none |
| security_isin | null | US88160R1014 | missing_in_email | low |
| security_name | Tesla Inc. | Tesla Inc. | match | none |
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| quantity | 11303 | 11303 | match | none |
| amount | 999202.27 | 999202.27 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty | Société Générale | Société Générale | match | none |
| reported_status | closed | Closed | match | none |

## Discrepancy Flags
- None (ISIN missing in email but enriched from HOST).

## Recommended Action
Host trade BF92476064 found and matches the email details. Provide the final confirmation slip to the requester and record that confirmation has been sent. Close or update the missing-confirmation workflow item per internal process.

## Draft Analyst Response
**Subject:** RE: Missing Confirmation - Trade BF92476064

Hello,

Please find attached the final confirmation slip for trade BF92476064 (Tesla Inc., 11,303 shares, settling 13-Mar-2026) as requested. 

Let us know if you need any further assistance.

Best regards,
Settlements Team

## Audit Trail
- **Workflow Branch**: standard
- **Warnings**: 
  - ISIN was not present in the email and was enriched from host data.
  - Host trades endpoint returned counterparty as LEI; counterparty enrichment resolved to a readable name.