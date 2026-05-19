# MAIA Settlement Mailbox Report - email_006.eml

- **Status:** standard_processed
- **Confidence Score:** 0.90
- **Confidence Threshold:** 0.72
- **Report generated (UTC):** 2026-05-10

## Routing Metadata

| Field | Value |
|---|---|
| Workflow branch | standard |
| Next workflow action | standard_processing |
| future_folder | standard |
| priority | low |
| analyst_review_required | false |
| should_query_host | true |
| recommended_report_type | standard_case |

## Source Metadata

| Field | Value |
|---|---|
| email_file | email_006.eml |
| source path | emails/email_006.eml |
| message_id | Not provided |
| sha256 | Not provided |
| schema_version | maia.structured_case_input.v1 |

## Classification

| Field | Value |
|---|---|
| Primary type | missing_confirmation |
| Original primary type | confirmation_missing |
| Secondary types | None |
| Settlement-related | true |
| Multi-type | false |
| Classification confidence | 0.98 |
| Confidence threshold | 0.72 |
| Needs human review | false |
| Human review reasons | None |

**Classification rationale:** Email explicitly requests a “final confirmation slip” and a “copy of the trade advice or execution confirmation.”

## Extracted Facts

| Field | Email Value |
|---|---|
| Reference number | BF92476064 |
| Counterparty name | Société Générale |
| Counterparty LEI | Not provided |
| Security name | Tesla Inc. |
| ISIN | Not provided |
| Trade date | 2026-03-12 |
| Settlement date | 2026-03-13 |
| Side | sell |
| Quantity | 11,303 |
| Amount | 999,202.27 |
| Currency | EUR |
| Reported status | closed |

### Trade Candidates

| Role | Trade Reference | Counterparty | Security | Trade Date | Settlement Date | Side | Quantity | Amount | Currency | Reported Status |
|---|---:|---|---|---|---|---|---:|---:|---|---|
| primary | BF92476064 | Société Générale | Tesla Inc. | 2026-03-12 | 2026-03-13 | sell | 11,303 | 999,202.27 | EUR | closed |

## Multi-Trade Notes

The email contains one trade candidate only. No multi-trade ambiguity was detected.

## Evidence Snippets

| ID | Source | Related Trade Reference | Supports | Snippet |
|---|---|---|---|---|
| ev_001 | body | BF92476064 | classification.primary_type | “require the final confirmation slip for trade BF92476064” |
| ev_002 | body | BF92476064 | extracted_data.trades[0].quantity; extracted_data.trades[0].net_amount | “BF92476064  12-Mar-2026  Sale  Société Générale  999202.27   Tesla Inc.  EUR  13-Mar-2026  11303” |

## Attachment Extraction Status

| Field | Value |
|---|---|
| Attachment count | 0 |
| All processed | true |
| Items | None |
| Notes | None |

## HOST Lookup Summary

| Field | Value |
|---|---|
| HOST lookup performed | true |
| Lookup status | matched |
| Lookup endpoint / mode | /trades / by_trade_reference |
| Preferred lookup strategy | by_trade_reference |
| Lookup key | trade_reference = BF92476064 |
| HOST response count | 1 |
| Reconciliation confidence | 0.90 |

**HOST reconciliation summary:** HOST returned a single matching trade for reference `BF92476064`. The reference number, trade date, settlement date, quantity, amount, currency, side, and closed status all match the email. The HOST counterparty value is `O2RNE8IBXP4R0TD8PL25`, which appears to be an internal identifier rather than the human-readable counterparty name in the email.

## Side-by-Side Comparison

| Field | Email Value | HOST Value | Status | Severity |
|---|---|---|---|---|
| reference_number | BF92476064 | BF92476064 | match | none |
| security_isin | Not provided | US88160R1014 | missing_in_email | low |
| security_name | Tesla Inc. | Not provided | missing_in_host | low |
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| quantity | 11,303 | 11,303 | match | none |
| amount | 999,202.27 | 999,202.27 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty | Société Générale | O2RNE8IBXP4R0TD8PL25 | mismatch | medium |
| reported_status | closed | Closed | match | none |

## Discrepancy Flags

- `counterparty_mismatch`

### Discrepancy Details

- The email identifies the counterparty as **Société Générale**.
- HOST identifies the counterparty field as **O2RNE8IBXP4R0TD8PL25**.
- The HOST value appears to be an internal identifier. No counterparty enrichment or master-data mapping was performed in this workflow.
- HOST provided the security as ISIN **US88160R1014** while the email provided the security name **Tesla Inc.**; HOST did not return a human-readable security name.

## Recommended Action

Host returned a single matching trade (`BF92476064`) with matching trade date, settlement date, quantity, amount, currency, side, and closed status. Recommended next steps:

1. Run counterparty enrichment or consult counterparty master data to confirm that `O2RNE8IBXP4R0TD8PL25` maps to **Société Générale**.
2. If the mapping confirms Société Générale, treat the missing-confirmation request as satisfied from a trade-existence/status perspective and provide the final confirmation slip or trade advice through the approved channel.
3. If the mapping does not confirm Société Générale, escalate to operations to resolve the counterparty discrepancy before sending any confirmation or closure notice.

## Draft Analyst Response Template

```text
Subject: Re: Final confirmation slip request - Trade BF92476064

Dear Client,

Thank you for your request.

We have located trade BF92476064 in our records. The trade is recorded as closed with the following details:

- Trade reference: BF92476064
- Trade date: 12-Mar-2026
- Settlement date: 13-Mar-2026
- Side: Sale
- Security: Tesla Inc.
- Quantity: 11,303
- Net amount: EUR 999,202.27
- Counterparty: Société Générale

We will provide the final confirmation slip / trade advice via the approved confirmation delivery channel. If you require it to be resent to a specific authorized recipient or mailbox, please confirm the delivery details.

Kind regards,
Settlements Team
```

**Analyst note before sending:** Confirm the HOST counterparty identifier `O2RNE8IBXP4R0TD8PL25` maps to Société Générale, or resolve the counterparty discrepancy, before sending any final confirmation or trade advice.

## Audit Trail

| Item | Details |
|---|---|
| Workflow branch | standard |
| APIs called | HOST lookup was performed before report generation according to provided HOST reconciliation; no HOST APIs were called during report writing. GitHub repository tools were used to persist this Markdown report. |
| HOST lookup plan | `/trades` by trade reference |
| Case key | trade_reference:BF92476064 |
| All required lookup fields present | true |
| Missing critical fields | None |
| Validation errors | None |
| Extraction confidence | 0.98 |
| Classification confidence | 0.98 |

### Warnings

- Host provided Security as ISIN (`US88160R1014`) while the email provided security name `Tesla Inc.`; no human-readable security name was returned from HOST.
- Host counterparty value appears to be an internal code; no counterparty enrichment was performed in this lookup.
- If counterparty mapping is critical, run a counterparty lookup or consult the master data service.
