# Human-in-the-Loop (HITL) Resolution Report

## Case Overview
- **Case ID:** VE93513959
- **Date Processed:** 2026-05-19
- **Status:** `needs_human_review`
- **Primary Issue:** Amount Mismatch
- **Confidence Score:** 0.91

## Discrepancy Details
- **Reported Amount (Email):** CHF 2158002.39
- **Expected Amount (Sender Claim):** CHF 1662949.54
- **Host Amount:** CHF 1662949.54
- **Description:** Sender reports correct amount CHF 1662949.54 but settlement was processed at CHF 2158002.39. The email facts/table show CHF 2158002.39 as the processed amount, while the HOST amount is CHF 1662949.54.

## Host System Data
- **Trade Reference:** VE93513959
- **Security:** CH0012530207 (ABB Ltd.)
- **Counterparty:** 3TK20IVIUJ8J3ZU0QE75 (ING Bank)
- **Trade Date:** 2026-03-03
- **Settlement Date:** 2026-03-04
- **Quantity:** 46388
- **Currency:** CHF
- **Side:** Kauf (buy)
- **Status:** Geschlossen

## Recommended Action
Route to human review for settlement amount discrepancy: email/table amount is CHF 2158002.39 while HOST amount is CHF 1662949.54. Security and counterparty identifiers were reconciled through enrichment lookups.