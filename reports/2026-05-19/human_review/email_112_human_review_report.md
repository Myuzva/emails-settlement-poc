# Human-in-the-Loop (HITL) Resolution Report

## Case Overview
- **Email File:** `email_112.eml`
- **Date Processed:** 2026-05-19
- **Status:** `needs_human_review`
- **Confidence Score:** 0.25
- **Primary Issue:** `reference_not_found_on_host`

## Reason for HITL Routing
- **Missing HOST Data:** Primary lookup by reference_number (RR29571843) returned 404 - no matching trade on HOST.
- **Sender Request:** Sender explicitly requests confirmation that the reference is missing in their system; human verification is appropriate.
- **Automated Reconciliation Failed:** Because the sender requests confirmation of a missing reference and the host returned no match, manual investigation is required.

## Extracted Trade Details
| Field | Extracted Value |
| :--- | :--- |
| **Trade Reference** | RR29571843 |
| **Counterparty** | Goldman Sachs |
| **Security** | Novartis AG |
| **Trade Date** | 2026-03-04 |
| **Settlement Date** | 2026-03-05 |
| **Side** | buy |
| **Quantity** | 94226 |
| **Amount** | 755047.19 |
| **Currency** | USD |

## Host Reconciliation Status
- **Lookup Strategy:** `by_trade_reference`
- **Host Status:** `no_match` (404 Not Found)
- **Discrepancies:**
  - `reference_number`: Missing in HOST (High Severity)
  - `security_name`: Missing in HOST (Medium Severity)
  - `quantity`: Missing in HOST (High Severity)
  - `amount`: Missing in HOST (High Severity)

## Recommended Analyst Action
Human review required: confirm with sender whether RR29571843 is the correct reference. If confirmed, instruct back-office to search HOST using alternative keys (trade date, settlement date, counterparty, amount, quantity). If not, request corrected reference or additional booking identifiers. Log as unresolved until manual investigation completes.

## Evidence & Context
- **Subject:** "Trade Confirmation Request – RR29571843"
- **Body:** "unable to match trade reference RR29571843 to any record in our booking system. Please confirm whether the reference number is correct"
- **Body:** "USD | Goldman Sachs | RR29571843 | 2026-03-04 | 2026-03-05 | Novartis AG | 94226 | 755047.19 | Kauf"