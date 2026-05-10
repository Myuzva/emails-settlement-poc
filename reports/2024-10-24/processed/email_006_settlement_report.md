# MAIA Settlement Mailbox Report - email_006.eml

- **Status**: standard_processed
- **Confidence Score**: 0.88 (Threshold: 0.72)
- **Routing Metadata**:
  - Future Folder: standard
  - Priority: low
  - Analyst Review Required: false

## Source Metadata
- **Email File**: email_006.eml
- **Primary Case Key**: trade_reference:BF92476064

## Classification
- **Primary Type**: missing_confirmation
- **Confidence**: 0.98
- **Reasons**: Email explicitly requests 'final confirmation slip' and 'copy of the trade advice or execution confirmation'

## Extracted Facts
- **Trade Reference**: BF92476064
- **Counterparty**: Société Générale
- **Security Name**: Tesla Inc.
- **Trade Date**: 2026-03-12
- **Settlement Date**: 2026-03-13
- **Side**: sell
- **Quantity**: 11303
- **Amount**: 999202.27
- **Currency**: EUR
- **Reported Status**: closed

## Evidence Snippets
- *"...require the final confirmation slip for trade BF92476064"* (Source: body)
- *"BF92476064  12-Mar-2026  Sale  Société Générale  999202.27   Tesla Inc.  EUR  13-Mar-2026  11303"* (Source: body)

## HOST Lookup Summary
- **Status**: matched
- **Lookup Strategy**: by_trade_reference
- **Host Response Count**: 1

### Side-by-Side Comparison
| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | BF92476064 | BF92476064 | match | none |
| isin | null | US88160R1014 | missing_in_email | low |
| security_name | Tesla Inc. | null | missing_in_host | low |
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| quantity | 11303 | 11303 | match | none |
| amount | 999202.27 | 999202.27 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty | Société Générale | O2RNE8IBXP4R0TD8PL25 | mismatch | medium |
| status | closed | Closed | match | none |

## Discrepancy Flags
- counterparty_mismatch
- security_name_missing_in_host
- security_identified_by_isin_only

## Recommended Action
Trade BF92476064 found on host and matches on reference, dates, quantity, amount, currency and side. Provide the requested final confirmation slip to the requester. Reconcile the host counterparty identifier (O2RNE8IBXP4R0TD8PL25) with 'Société Générale' by querying the host's counterparty mapping or operations before closing the case. Optionally update/augment host record with security name (ISIN US88160R1014 maps to Tesla Inc.).

## Draft Analyst Response Template
**Subject**: RE: Missing Confirmation Slip - Trade BF92476064

Hello,

Thank you for reaching out. Please find attached the final confirmation slip for trade BF92476064 (Tesla Inc., 11,303 shares, EUR 999,202.27) as requested. 

Let us know if you need any further assistance.

Best regards,
Settlements Team

## Audit Trail
- **Workflow Branch**: standard
- **Warnings**: 
  - Host counterparty is an identifier/code (O2RNE8IBXP4R0TD8PL25) rather than the expected name 'Société Générale'. Confirm mapping before relying on counterparty name.
  - Host response included ISIN but not a human-readable security name; security identified by ISIN US88160R1014 (Tesla).
  - No additional HOST endpoints (security or counterparty) were called because the preferred lookup by trade reference returned an unambiguous match.