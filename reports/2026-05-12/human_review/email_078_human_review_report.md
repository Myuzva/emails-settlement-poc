# Human-in-the-Loop (HITL) Review Report

**Date Generated:** 2026-05-12
**Email File:** email_078.eml
**Trade Reference:** DY52987070
**Routing Destination:** `human_review`

## 1. Reason for HITL Routing
- **Primary Reason:** critical attachment extraction failed
- **Secondary Reason(s):** Missing critical fields (trade_date, settlement_date, quantity, currency, net_amount, side)

## 2. Extracted Trade Data (Partial)
| Field | Extracted Value |
| :--- | :--- |
| **Trade Reference** | DY52987070 |
| **Counterparty** | Rhein Asset |
| **Instrument** | Nestlé S.A. |
| **Trade Date** | *Missing* |
| **Settlement Date** | *Missing* |
| **Quantity** | *Missing* |
| **Currency** | *Missing* |
| **Net Amount** | *Missing* |
| **Side** | unknown |

## 3. Discrepancy Claims
- **Type:** wrong_security
- **Description:** Sender booked Nestlé S.A. but confirmation shows Alphabet Inc.
- **Sender Value:** Nestlé S.A.
- **Expected/Requested Value:** Alphabet Inc.

## 4. Attachment Processing Issues
- **File:** `trade_details.zip`
- **Status:** empty
- **Warning:** Zip file extraction returned no content

## 5. Evidence & Context
- **Source:** body
- **Quote:** "our records indicate the traded security is Nestlé S.A.. However, the confirmation we received references Alphabet Inc."

## 6. Recommended Analyst Action
- Review the original email and the unprocessable attachment (`trade_details.zip`).
- Manually extract the missing trade fields.
- Verify the security mismatch (Nestlé S.A. vs Alphabet Inc.) against the host system using Trade Reference DY52987070.