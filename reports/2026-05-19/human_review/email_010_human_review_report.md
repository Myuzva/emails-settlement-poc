# Settlement Analyst Report: email_010.eml

| Field | Value |
| ----- | ----- |
| **Date** | 2026-05-19 |
| **Status** | Needs Human Review |
| **Confidence Score** | 86% |
| **Email File** | email_010.eml |
| **Trade Reference** | ZN64848506 |

## Executive Summary
The sender (Sarah Jensen) requests confirmation that internal pre-settlement checks are complete and the open trade is on track for timely settlement. While most trade economics match exactly between the email and the host system, the host counterparty identifier (`R0MUWSFPU8MPRO8K5P83`) could not be resolved to the email's counterparty ("BNP Paribas"). Human review is required to confirm this mapping before replying.

## Human Review Justification
- **Counterparty Unresolved**: The counterparty on the host is an internal identifier (`R0MUWSFPU8MPRO8K5P83`) that did not resolve via the `/counterparty` endpoint (404 Not Found). It cannot be automatically assumed to equal "BNP Paribas" without human confirmation.
- **Language Normalization**: Host-side 'Buy Sale' and 'Status' values were returned in German ('Verkauf', 'Offen') and have been normalized to 'sell' and 'open'.

## Trade Details Comparison

| Field | Email Value | Host Value | Status | Severity |
| ----- | ----------- | ---------- | ------ | -------- |
| **Reference Number** | ZN64848506 | ZN64848506 | Match | None |
| **Security Name** | JPMorgan Chase & Co. | JPMorgan Chase & Co. | Match | None |
| **ISIN** | *null* | US46625H1005 | Missing in Email | None |
| **Settlement Date** | 2026-03-18 | 2026-03-18 | Match | None |
| **Trade Date** | 2026-03-17 | 2026-03-17 | Match | None |
| **Quantity** | 23215 | 23215 | Match | None |
| **Amount** | 1977850.41 | 1977850.41 | Match | None |
| **Currency** | USD | USD | Match | None |
| **Side** | sell | Verkauf | Match | Low |
| **Counterparty** | BNP Paribas | R0MUWSFPU8MPRO8K5P83 | Mismatch | High |
| **Status** | open | Offen | Match | Low |

## Recommended Action
**Human review required**: Confirm mapping of host counterparty identifier `R0MUWSFPU8MPRO8K5P83` to the email counterparty 'BNP Paribas' before replying. All trade economics (amount, quantity, dates, currency, side) and reference number match; status is 'open' (host 'Offen') and settlement date matches. After counterparty confirmation, respond to requester confirming pre-settlement checks/status or update host record if mapping is incorrect.

## Evidence & Context
- **Body**: *"trade ZN64848506 is currently marked as open, scheduled for settlement on 2026-03-18"*
- **Body**: *"Could you please confirm if all internal pre-settlement checks are complete and if we are on track for a timely settlement?"*
- **Attachment (`trade_details.txt`)**: *"BNP Paribas 23215 2026-03-18 JPMorgan Chase & Co. 1977850.41 Verkauf USD 2026-03-17"*
