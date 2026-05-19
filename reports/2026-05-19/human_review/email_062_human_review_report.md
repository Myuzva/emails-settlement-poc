# Settlement Discrepancy Report: EP95329750 / email_062.eml

**Date Generated:** 2026-05-19
**Status:** Needs Human Review
**Confidence Score:** 12%
**Email File:** email_062.eml
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>
**Subject:** Trade Exception – EP95329750

---

## Executive Summary
The sender reported an unmatched trade (EP95329750) during period-end reconciliation. They have no internal record of this trade despite it appearing in external documentation as closed. Host system lookup for reference EP95329750 returned a 404 Not Found. Human review is required to investigate alternative booking references or erroneous settlement-file inclusion.

## Discrepancy Analysis

| Field | Email Value | Host Value | Status | Severity |
| :--- | :--- | :--- | :--- | :--- |
| **Trade Reference** | EP95329750 | *Not Found* | Missing in Host | High |
| **Security Name** | Novartis AG | *Not Found* | Missing in Host | Medium |
| **Settlement Date** | 2026-01-28 | *Not Found* | Missing in Host | High |
| **Trade Date** | 2026-01-27 | *Not Found* | Missing in Host | Medium |
| **Quantity** | 20,185 | *Not Found* | Missing in Host | High |
| **Amount** | 612,506.76 EUR | *Not Found* | Missing in Host | High |
| **Currency** | EUR | *Not Found* | Missing in Host | High |
| **Side** | Sell | *Not Found* | Missing in Host | Medium |
| **Counterparty** | Santander | *Not Found* | Missing in Host | Medium |

## Extracted Trade Details (Email)
* **Reference Number:** EP95329750
* **Counterparty:** Santander
* **Security:** Novartis AG
* **Trade Date:** 2026-01-27
* **Settlement Date:** 2026-01-28
* **Side:** Sell
* **Quantity:** 20,185
* **Amount:** 612,506.76 EUR
* **Reported Status:** Closed

## Host System Data
* **Lookup Strategy:** by_trade_reference
* **Host Status:** no_match (404 Not Found)
* **Notes:** Host returned 404 for trade reference EP95329750; treated as no_match per lookup rules. No trade data returned.

## Evidence & Quotes
* *"period-end reconciliation has flagged trade EP95329750 as unmatched — we have no record of this trade in our system despite it appearing in external documentation as closed"*
* *"Please advise whether this was booked under an alternative reference, or whether the trade was erroneously included in the settlement file."*
* *"Notional 612506.76; Security Novartis AG; Settlement Date 28-Jan-2026; Trd Side Sale; Broker Santander; Currency EUR; Exec Date 27-Jan-2026; Units 20185"*

## Recommended Actions
1. **Human review required.** Investigate alternative booking references.
2. Search other internal systems (trade blotter, booking apps, or legacy systems) for EP95329750 or matching trade attributes (28-Jan-2026, Novartis AG, 20,185 units, EUR 612,506.76).
3. Contact sender requesting any additional identifiers (internal booking reference, counterparty full legal name/LEI, broker reference) or attachments.