# MAIA Human-in-the-Loop (HITL) Report: email_050.eml

## 1. Case Overview
* **Date Processed:** 2026-05-19
* **Email File:** email_050.eml
* **Sender:** James O'Brien <j.obrien@meridianfunds.co.uk>
* **Subject:** Trade Inquiry – Reference OA38238234
* **Primary Classification:** documentation_missing
* **Confidence Score:** 0.82
* **Status:** `needs_human_review`

## 2. Reason for Human Review
Human review is recommended before responding because the HOST trade was found and key economic fields match, but the counterparty could not be reconciled. The email shows "Meridian Funds" while HOST shows identifier "ANGGYXNX0JLX3X63W380", and counterparty enrichment by name returned no match.

## 3. Extracted Trade Facts
| Field | Extracted Value | Confidence |
| :--- | :--- | :--- |
| **Reference Number** | OA38238234 | 0.98 |
| **Counterparty** | Meridian Funds | 0.72 |
| **Trade Date** | 2026-03-13 | 0.95 |
| **Settlement Date** | 2026-03-16 | 0.95 |
| **Quantity** | 51993 | 0.95 |
| **Amount** | 1915019.39 | 0.95 |
| **Currency** | CHF | 0.95 |
| **Side** | unknown | 0.00 |

## 4. HOST Reconciliation Summary
* **HOST Lookup Status:** matched
* **HOST Reference:** OA38238234
* **HOST Counterparty:** ANGGYXNX0JLX3X63W380
* **HOST Security:** US0378331005 (Apple Inc.)
* **HOST Status:** Open

## 5. Discrepancies & Claims
| Field | Email Value | HOST Value | Status | Severity |
| :--- | :--- | :--- | :--- | :--- |
| **Counterparty** | Meridian Funds | ANGGYXNX0JLX3X63W380 | unknown | medium |
| **Side** | unknown | Sale | missing_in_email | low |
| **Security ISIN** | null | US0378331005 | missing_in_email | none |
| **Security Name** | null | Apple Inc. | missing_in_email | none |
| **Status** | unknown | Open | missing_in_email | none |

*Note: The sender reports that documentation is incomplete and asks for full trade details to proceed with pre-settlement checks. Missing fields in the email are expected.*

## 6. Recommended Action
If accepted after review, respond with the complete HOST trade details requested for pre-settlement checks.