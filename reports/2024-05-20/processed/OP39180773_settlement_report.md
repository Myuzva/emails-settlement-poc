# MAIA Settlement Mailbox Report - OP39180773

- **Status**: standard_processed
- **Confidence Score**: 0.95 (Threshold: 0.72)
- **Routing Metadata**:
  - Future Folder: standard
  - Priority: Normal
  - Analyst Review Required: false
- **Source Metadata**:
  - Email File: Unknown (Reference: OP39180773)
- **Classification**: missing_confirmation

## Extracted Facts
- **Reference Number**: OP39180773
- **Counterparty**: JP Morgan
- **Security**: Deutsche Bank AG
- **Trade Date**: 2026-03-10
- **Settlement Date**: 2026-03-11
- **Side**: buy
- **Quantity**: 68390
- **Amount**: 1436398.52
- **Currency**: CHF

## Evidence Snippets
- **trade_reference**: "obtain the final settlement confirmation for trade OP39180773"
- **counterparty**: "Dealer: JP Morgan"
- **trade_date**: "Trade Date: 10-Mar-2026"
- **settlement_date**: "Stlmt Date: 11-Mar-2026"
- **currency**: "Trade Ccy: CHF"
- **net_amount**: "Net Amt: 1 436 398.52"
- **quantity**: "Quantity: 68 390"
- **side**: "Buy/Sell: Buy"
- **instrument**: "Instrument: Deutsche Bank AG"
- **notes**: "All trade details extracted from attached trade_details.jpg screenshot."

## Attachment Extraction Status
- **trade_details.jpg**: processed (Contains trade data: true)

## HOST Lookup Summary
- **Status**: matched
- **Lookup Plan**: Endpoint `/trades`, Mode `reference_number`
- **Host Response Count**: 1

## Side-by-Side Comparison
| Field | Email Value | HOST Value | Status | Severity |
|---|---|---|---|---|
| reference_number | OP39180773 | OP39180773 | match | none |
| security | Deutsche Bank AG | DE0005140008 | match | none |
| trade_date | 2026-03-10 | 2026-03-10 | match | none |
| settlement_date | 2026-03-11 | 2026-03-11 | match | none |
| quantity | 68390 | 68390 | match | none |
| amount | 1436398.52 | 1436398.52 | match | none |
| currency | CHF | CHF | match | none |
| side | buy | Buy | match | none |
| counterparty | JP Morgan | 8I5DZWZKVSZI1NUHU748 | mismatch | low |

## Discrepancy Flags
- counterparty_identifier_mismatch

## Recommended Action
Resolve counterparty identifier to human-readable name (counterparty lookup) and confirm mapping with internal reference; if confirmed, close reconciliation. If mismatch persists, escalate to operations.

## Draft Analyst Response Template
Dear Counterparty,

Thank you for your email. We have successfully matched trade OP39180773 in our system. We are currently resolving a minor discrepancy regarding the counterparty identifier and will provide the final settlement confirmation shortly.

Best regards,
Settlements Team

## Audit Trail
- **Workflow Branch**: standard
- **APIs Called**: email_analysis_tool, host_reconciliation (/trades)
- **Warnings**: Host returned counterparty as an internal identifier rather than a human-readable name; perform counterparty enrichment lookup before final confirmation
