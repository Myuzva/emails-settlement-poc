# MAIA Settlement Mailbox Report - email_002.eml

- **Status**: standard_processed
- **Confidence Score**: 0.88 (Threshold: 0.72)
- **Routing Metadata**:
  - Future Folder: standard
  - Priority: low
  - Analyst Review Required: false
- **Source Metadata**:
  - Email File: email_002.eml
  - Message ID: null
- **Classification**: generic_trade_details_request (Confidence: 0.95)

## Extracted Facts
- **Trade Reference**: XJ02184853
- **Counterparty**: Santander
- **Security Name**: UBS Group AG
- **ISIN**: null
- **Trade Date**: null
- **Settlement Date**: null
- **Side**: sell
- **Quantity**: 29837
- **Amount**: 1666712.84
- **Currency**: EUR
- **Reported Status**: closed

## Evidence Snippets
- **Body**: "Our post-settlement audit of trade XJ02184853 has revealed that the trade record is incomplete in our system, despite the trade being marked as closed." (Confidence: 0.98)
- **Attachment (trade_details.txt)**: "Side Verkauf\nTrade Ref XJ02184853\nQuantity 29837\nAsset UBS Group AG\nCurrency EUR\nNet Amount 1666712.84" (Confidence: 0.99)

## Attachment Extraction Status
- **Count**: 1 (All processed: true)
- **Items**:
  - `trade_details.txt` (text/plain) - Status: parsed. Contains trade data.

## HOST Lookup Summary
- **Status**: matched
- **Lookup Strategy**: by_trade_reference
- **Endpoint**: /trades

## Side-by-Side Comparison
| Field | Email Value | HOST Value | Status | Severity |
|---|---|---|---|---|
| reference_number | XJ02184853 | XJ02184853 | match | none |
| security_isin | null | CH0244767585 | missing_in_email | low |
| instrument/security_name | UBS Group AG | null | missing_in_host | low |
| settlement_date | null | 2026-03-20 | missing_in_email | medium |
| trade_date | null | 2026-03-19 | missing_in_email | medium |
| quantity | 29837 | 29837 | match | none |
| amount | 1666712.84 | 1666712.84 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Verkauf (sell) | match | none |
| counterparty | Santander | 5UMCZOEYKCVFAW8ZLO05 | mismatch | medium |
| reported_status | closed | Geschlossen (closed) | match | none |

## Discrepancy Flags
- missing_trade_date_in_email
- missing_settlement_date_in_email
- security_name_missing_in_host_response
- counterparty_identifier_mismatch

## Recommended Action
Populate the internal trade record using host values: set trade_date=2026-03-19, settlement_date=2026-03-20 and security ISIN=CH0244767585. Verify and map the host counterparty identifier (5UMCZOEYKCVFAW8ZLO05) to the known name 'Santander' in the counterparty master before updating; if mapping is not found, escalate to operations for manual verification. Enrich the security name from the security master using the ISIN if required. No full human review required if counterparty mapping can be confirmed.

## Draft Analyst Response Template
Dear Santander Operations,

Thank you for reaching out regarding trade XJ02184853. We have reviewed our systems and can confirm the trade is closed. We have updated our records with the missing trade date (2026-03-19) and settlement date (2026-03-20) as per our internal systems. 

Please let us know if you need any further details.

Best regards,
Settlements Team

## Audit Trail
- **Workflow Branch**: standard
- **APIs Called**: HOST /trades (by reference_number)
- **Warnings**: 
  - Email missing critical fields trade_date and settlement_date; host provided these values recommended for update.
  - Host returned a counterparty identifier rather than a human-readable name; confirm mapping before automatic update.
  - Host did not return a human-readable security name (only ISIN); consider enriching from security master.