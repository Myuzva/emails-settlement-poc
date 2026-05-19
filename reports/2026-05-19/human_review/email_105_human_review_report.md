# Human Review Required: Settlement Date Mismatch - MU50046625

## Case Overview
- **Email File:** email_105.eml
- **Message ID:** `<177738352875.31976.1179565069528118348@Arek.yallo.box>`
- **Date:** Tue, 28 Apr 2026 15:38:48 +0200
- **Sender:** Thomas Müller <t.mueller@rheinasset.de>
- **Subject:** Trade Exception – MU50046625
- **Classification:** settlement_date_mismatch
- **Confidence Score:** 0.78

## Reason for Human Review
HOST trade was found by reference number. Confirm that HOST settlement date is 2026-03-05, not the email/attachment instruction date 2026-02-19. Human review is recommended because the settlement-date difference is material and the HOST counterparty is an identifier that could not be reconciled to the email counterparty name within the request limit.

## Extracted Trade Facts
| Field | Extracted Value |
| :--- | :--- |
| **Reference Number** | MU50046625 |
| **Counterparty Name** | Raiffeisen Bank |
| **Security Name** | Microsoft Corp. |
| **Trade Date** | 2026-03-04 |
| **Settlement Date** | 2026-02-19 |
| **Side** | sell |
| **Quantity** | 63414 |
| **Amount** | 157516.59 |
| **Currency** | EUR |

## Host Reconciliation Status
**Status:** matched

| Field | Email Value | Host Value | Match Status | Severity |
| :--- | :--- | :--- | :--- | :--- |
| reference_number | MU50046625 | MU50046625 | match | none |
| security_name | Microsoft Corp. | Microsoft Corp. | match | none |
| isin | null | US5949181045 | missing_in_email | none |
| trade_date | 2026-03-04 | 2026-03-04 | match | none |
| settlement_date | 2026-02-19 | 2026-03-05 | mismatch | high |
| side | sell | Verkauf | match | none |
| quantity | 63414 | 63414 | match | none |
| amount | 157516.59 | 157516.59 | match | none |
| currency | EUR | EUR | match | none |
| counterparty_name | Raiffeisen Bank | PQOH26KWDF7CG10L6792 | unknown | medium |
| status | unknown | Offen | missing_in_email | none |

## Discrepancy Claims
- **Type:** settlement_date_mismatch
- **Description:** Sender reports a value/settlement date mismatch: their internal booking shows 05-Mar-2026 while the instruction from the recipient side shows 19-Feb-2026; confirmation of the correct settlement date is requested.
- **Sender Value:** 2026-03-05
- **Expected/Requested Value:** 2026-02-19

## Evidence & Attachments
- **Body Quote:** "We have identified a value date mismatch on trade MU50046625. Our internal booking reflects 05-Mar-2026, whereas the instruction received from your side indicates 19-Feb-2026."
- **Attachment Quote:** "Trade Inquiry Details: Stlmt Date 19-Feb-2026; Net Amount 157516.59; Asset Microsoft Corp.; Cpty Raiffeisen Bank; Exec Date 04-Mar-2026; Trade Ref MU50046625; Face Amt 63414; Direction Verkauf; Currency EUR" (Source: trade_details.zip/trade_details.pdf)
- **Attachments Processed:** trade_details.zip (application/zip)

## Recommended Analyst Action
Review the settlement date discrepancy. The sender's internal booking (2026-03-05) matches the HOST system, but the instruction received indicates 2026-02-19. Additionally, verify the counterparty mapping between "Raiffeisen Bank" and HOST identifier "PQOH26KWDF7CG10L6792".