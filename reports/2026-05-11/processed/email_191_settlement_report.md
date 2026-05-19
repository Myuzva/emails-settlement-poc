# MAIA Settlement Mailbox Report - email_191.eml

- **Status:** standard_processed
- **Confidence Score:** 0.95
- **Classification Confidence:** 0.98
- **Confidence Threshold:** 0.72
- **Generated UTC Date:** 2026-05-11

## Routing Metadata

| Field | Value |
|---|---|
| Workflow branch | standard |
| Next workflow action | standard_processing |
| Future folder | standard |
| Priority | low |
| Analyst review required | false |
| Should query HOST | true |
| Recommended report type | standard_case |

## Source Metadata

| Field | Value |
|---|---|
| Email file | email_191.eml |
| Source path | emails/email_191.eml |
| Message ID | Not provided |
| SHA-256 | Not provided |
| Schema version | maia.structured_case_input.v1 |
| Original payload schema | maia.email_case_payload.v1 |

## Classification

| Field | Value |
|---|---|
| Primary type | general_status_request |
| Original primary type | settlement_status_request |
| Settlement related | true |
| Secondary types | None |
| Multi-type | false |
| Needs human review | false |

**Classification rationale:**

- Email explicitly asks to confirm if pre-settlement checks are complete and if on track for timely settlement.

## Extracted Facts

| Field | Extracted value |
|---|---|
| Reference number | JB51584684 |
| Counterparty name | UniCredit |
| Counterparty LEI | Not provided in email |
| Security name | JPMorgan Chase & Co. |
| ISIN | Not provided in email |
| Trade date | 2026-03-18 |
| Settlement date | 2026-03-19 |
| Side | sell |
| Quantity | 70,135 |
| Amount | 1,022,523.28 |
| Currency | CHF |
| Reported status | open |

### Trade Candidates

| Role | Trade reference | Counterparty | Security | ISIN | Trade date | Settlement date | Side | Quantity | Amount | Currency | Reported status |
|---|---|---|---|---|---|---|---|---:|---:|---|---|
| primary | JB51584684 | UniCredit | JPMorgan Chase & Co. | Not provided | 2026-03-18 | 2026-03-19 | sell | 70,135 | 1,022,523.28 | CHF | open |

### Field Confidence

| Field | Confidence |
|---|---:|
| Trade reference | 0.99 |
| Counterparty | 0.90 |
| Trade date | 0.99 |
| Settlement date | 0.99 |
| Quantity | 0.99 |
| Currency | 0.99 |
| Net amount | 0.99 |
| Instrument | 0.99 |
| Side | 0.99 |

## Multi-Trade Notes

- The email contains **one** trade candidate.
- `multi_trade_email`: false.
- Primary case key: `trade_reference:JB51584684`.
- No conflicting fields or missing critical fields were identified.

## Evidence Snippets

| ID | Source | Related trade | Supports | Snippet |
|---|---|---|---|---|
| ev_001 | body | JB51584684 | classification.primary_type; extracted_data.trade_reference; extracted_data.reported_status | “trade JB51584684 is currently marked as open... Could you please confirm if all internal pre-settlement checks are complete” |
| ev_002 | attachment:trade_details.pdf | JB51584684 | quantity; net amount; currency; instrument; side; trade date; settlement date | “Net Amt 1022523.28 Security JPMorgan Chase & Co. Nom 70135 Direction Sale Trd Ccy CHF Val Dt 19-Mar-2026 Broker UniCredit Trade Date 18-Mar-2026” |

**Evidence notes:** Extracted trade reference and status from email body. Extracted trade details from attached PDF.

## Attachment Extraction Status

| Filename | Content type | Extraction status | Extraction method | Contains trade data | Contains multiple trades | Related trade references | Warnings |
|---|---|---|---|---|---|---|---|
| trade_details.pdf | application/pdf | parsed | pdf_text | true | false | JB51584684 | None |

- Attachment count: 1
- All attachments processed: true
- Unsupported or failed attachments: none

## HOST Lookup Summary

HOST reconciliation was provided for this standard branch case. No HOST APIs were called during report generation.

| Field | Value |
|---|---|
| Lookup status | matched |
| Host response count | 1 |
| Preferred lookup strategy | by_trade_reference |
| Lookup key | JB51584684 |
| Host confidence score | 0.95 |

### HOST Lookup Plan

| Endpoint | Mode |
|---|---|
| /trades | by_reference |
| /security | by_name |
| /counterparty | by_name |

### HOST Confidence Reasons

- Exact match on unique trade reference JB51584684 returned a single host trade (1 result).
- Numeric fields (quantity and amount) match exactly within allowed tolerances.
- Dates match exactly after normalization.
- Security name and counterparty name were confirmed via security and counterparty lookups; ISIN and LEI were enriched from HOST.
- No ambiguous or conflicting HOST results.

## Side-by-Side Comparison

| Field | Email value | HOST value | Status | Severity |
|---|---|---|---|---|
| Reference number | JB51584684 | JB51584684 | match | none |
| Security name | JPMorgan Chase & Co. | JPMorgan Chase & Co. | match | none |
| ISIN | Not provided | US46625H1005 | missing_in_email | low |
| Trade date | 2026-03-18 | 2026-03-18 | match | none |
| Settlement date | 2026-03-19 | 2026-03-19 | match | none |
| Quantity | 70,135 | 70,135 | match | none |
| Amount | 1,022,523.28 | 1,022,523.28 | match | none |
| Currency | CHF | CHF | match | none |
| Side | sell | Sale | match | none |
| Counterparty | UniCredit | UniCredit (LEI: F1T87K3OQ2OV1UORLH26) | match | none |
| Reported status | open | Open | match | none |

## Discrepancy Flags

- No reconciliation discrepancy flags were reported.
- Low-severity enrichment note: email did not include ISIN; HOST supplied ISIN `US46625H1005`.
- Low-severity enrichment note: HOST supplied counterparty LEI `F1T87K3OQ2OV1UORLH26` for UniCredit.

## Recommended Action

- [ ] Proceed with standard processing for trade `JB51584684`.
- [ ] Confirm to the requester that the trade is recorded as **OPEN** and on track for settlement on **2026-03-19**.
- [ ] Include HOST enrichment details internally: ISIN `US46625H1005`; counterparty LEI `F1T87K3OQ2OV1UORLH26`.
- [ ] No analyst escalation required unless new information is received from the requester or settlement status changes.

**System recommendation:** No reconciliation discrepancies found. Proceed with standard processing and confirm to requester that trade JB51584684 is recorded as OPEN and on track for settlement on 2026-03-19. Note: ISIN and counterparty LEI were added from HOST enrichment.

## Draft Analyst Response Template

Subject: Re: Settlement status for trade JB51584684

Hello,

Thank you for your message.

We have completed the internal pre-settlement reconciliation checks for trade **JB51584684** against our records. The trade is recorded as **OPEN** and the key details match our records:

- Counterparty: **UniCredit**
- Security: **JPMorgan Chase & Co.**
- Side: **Sale**
- Quantity: **70,135**
- Net amount: **CHF 1,022,523.28**
- Trade date: **18-Mar-2026**
- Settlement date: **19-Mar-2026**

No reconciliation discrepancies were identified. Based on the current status, the trade remains on track for timely settlement on **19-Mar-2026**.

Best regards,
Settlement Operations

## Quality and Validation

| Field | Value |
|---|---|
| All required lookup fields present | true |
| Missing critical fields | None |
| Validation errors | None |
| Extraction confidence | 0.98 |
| Classification confidence | 0.98 |
| Parser warnings | None |
| OCR warnings | None |

## Audit Trail

| Item | Details |
|---|---|
| Workflow branch | standard |
| Report status | standard_processed |
| HOST lookup performed before report generation | Yes, provided as `host_reconciliation` input |
| HOST APIs called during report generation | None |
| Other external/HOST APIs called during report generation | None |
| GitHub repository tools used | repository tree lookup; code search; branch list; set active branch; create branch; create file |
| Code Executor usage | Used only to determine current UTC date |
| `/answers` called | No |
| Report persisted to GitHub | `reports/2026-05-11/processed/email_191_settlement_report.md` |

## Warnings

- Email did not include ISIN; HOST trade stored security as ISIN `US46625H1005`. Security lookup was performed before report generation to confirm name match.
- HOST counterparty was provided as LEI; counterparty lookup was performed before report generation to confirm name match to UniCredit.
