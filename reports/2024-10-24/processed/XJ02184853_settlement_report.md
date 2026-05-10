# MAIA Settlement Mailbox Report - XJ02184853

- **Status**: standard_processed
- **Confidence Score**: 0.95 (Threshold: 0.72)
- **Routing metadata**: 
  - Future Folder: standard
  - Priority: Normal
  - Analyst Review Required: false
- **Source metadata**: 
  - Email File: unknown_email
- **Classification**: missing_confirmation

## Extracted Facts
- **Reference Number**: XJ02184853
- **Counterparty**: Santander
- **Security Name**: UBS Group AG
- **Side**: sell
- **Quantity**: 29837
- **Amount**: 1666712.84
- **Currency**: EUR

## Evidence Snippets
- Trade Ref XJ02184853 (Source: evidence.trade_reference)
- Quantity 29837 (Source: evidence.quantity)
- Asset UBS Group AG (Source: evidence.security_name)
- Currency EUR (Source: evidence.currency)
- Net Amount 1666712.84 (Source: evidence.net_amount)
- Executing Broker Santander (Source: evidence.counterparty)
- Side 'Verkauf' translated to 'Sell'. (Source: evidence.side)

## Attachment Extraction Status
- **trade_details.txt**: attempted (Contains trade data: true)

## HOST Lookup Summary
- **Status**: matched
- **Lookup Plan**: Endpoint `/trades`, Mode `reference_number`
- **Matches Found**: 1

## Side-by-Side Comparison
| Field | Email Value | HOST Value | Status | Severity |
|---|---|---|---|---|
| reference_number | XJ02184853 | XJ02184853 | match | none |
| quantity | 29837 | 29837 | match | none |
| amount | 1666712.84 | 1666712.84 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Verkauf | match | none |
| security_name | UBS Group AG | null | missing_in_host | low |
| isin | null | CH0244767585 | missing_in_email | low |
| settlement_date | null | 2026-03-20 | missing_in_email | low |
| trade_date | null | 2026-03-19 | missing_in_email | low |
| counterparty | Santander | 5UMCZOEYKCVFAW8ZLO05 | unknown | low |

## Discrepancy Flags
- None

## Recommended Action
- **Action**: affirm
- **Reasons**: HOST reference match found, Single unambiguous trade returned, Quantity, amount and currency match exactly

## Draft Analyst Response Template
Dear Santander,

Thank you for your email. We have successfully located the trade reference XJ02184853 in our system. All critical trade details (Quantity: 29837, Amount: 1666712.84 EUR) match our records. We are proceeding with the affirmation.

Best regards,
Settlements Team

## Audit Trail
- **Workflow Branch**: standard
- **APIs Called**: email_analysis_tool
- **Warnings**: None
