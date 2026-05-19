# Settlement Discrepancy Report: QZ85525941 - Action Required

| Field | Value |
| :--- | :--- |
| **Date** | 2026-05-19 |
| **Case ID** | email_097.eml |
| **Status** | Needs Human Review |
| **Priority** | High |
| **Assignee** | Settlement Operations Team |

## Executive Summary
A post-settlement audit request was received from Sarah Jensen (s.jensen@nordbank.com) regarding trade `QZ85525941`. The sender states that the trade record is incomplete in their system despite being marked as closed. While the core trade economics (quantity, amount, dates) match our host system, critical discrepancies exist regarding counterparty identification and security naming conventions that require human verification.

## Discrepancy Analysis

| Field | Email Value | Host Value | Status | Severity |
| :--- | :--- | :--- | :--- | :--- |
| **Reference Number** | QZ85525941 | QZ85525941 | Match | None |
| **Counterparty** | Nordbank | W22LROWP2IHZNBB6K528 | Mismatch | High |
| **Security** | Novartis AG | CH0012221716 | Mismatch | Low |
| **Trade Date** | 2026-03-27 | 2026-03-27 | Match | None |
| **Settlement Date**| 2026-03-30 | 2026-03-30 | Match | None |
| **Side** | sell | Sale | Match | None |
| **Quantity** | 45,458 | 45,458 | Match | None |
| **Amount** | 1,141,321.88 EUR | 1,141,321.88 EUR | Match | None |
| **Status** | closed | Closed | Match | None |

## Root Cause Analysis
1. **Counterparty Identification Failure**: The email references the counterparty as "Nordbank", but our host system uses the identifier `W22LROWP2IHZNBB6K528`. An automated lookup for "Nordbank" returned a 404 Not Found, meaning we cannot programmatically confirm this mapping.
2. **Security Naming Convention**: The host system tracks the security via ISIN (`CH0012221716`), whereas the email provides the company name ("Novartis AG"). 
3. **Multi-Trade Ambiguity**: The attached PDF contains an additional trade (`KY05031605`), though the email body explicitly identifies `QZ85525941` as the primary trade needing action.

## Recommended Actions
1. **Verify Counterparty Mapping**: Manually confirm that the host identifier `W22LROWP2IHZNBB6K528` corresponds to "Nordbank".
2. **Verify Security Mapping**: Confirm that ISIN `CH0012221716` corresponds to "Novartis AG".
3. **Update Host Records**: Once verified, update the host system to link the human-readable names with their respective identifiers to prevent future lookup failures.
4. **Respond to Counterparty**: Provide the missing details requested by Sarah Jensen to close their audit gap.

## Audit Trail
* **Source**: `email_097.eml`
* **Message ID**: `<177738352859.31976.9751081404812316314@Arek.yallo.box>`
* **Evidence**:
  * *Body*: "post-settlement audit of trade QZ85525941 has revealed that the trade record is incomplete in our system, despite the trade being marked as closed"
  * *Attachment (trade_details.pdf)*: "QZ85525941 45458 30.03.2026 Sale Novartis AG 1141321.88 27.03.2026 EUR"