# Settlement Analyst Report: email_050.eml

| Field | Value |
|---|---|
| **Report Date** | 2026-05-19 |
| **Status** | Needs Human Review |
| **Confidence Score** | 72% |
| **Source Email** | email_050.eml |
| **Trade Reference** | OA38238234 |

## 1. Executive Summary
This case requires human review due to missing critical trade details in the email (Security Name, ISIN, and Side) and a counterparty mismatch during host reconciliation. The sender (Meridian Funds) indicated that trade documentation is incomplete and requested full trade details to be resubmitted for pre-settlement checks.

## 2. Case Classification & Routing
* **Primary Classification:** Instruction or Document Update (Documentation Missing)
* **Secondary Classifications:** Generic Trade Details Request
* **Routing Decision:** `human_review`
* **Reason:** Counterparty mismatch and missing critical fields (security and side) require human-in-the-loop review before settlement actions.

## 3. Extracted Trade Facts
| Field | Extracted Value | Confidence |
|---|---|---|
| Reference Number | OA38238234 | High |
| Trade Date | 2026-03-13 | High |
| Settlement Date | 2026-03-16 | High |
| Quantity | 51,993 | High |
| Amount | 1,915,019.39 | High |
| Currency | CHF | High |
| Counterparty | Meridian Funds | Medium |
| Security / ISIN | *Missing* | N/A |
| Side | *Missing* | N/A |

## 4. Host Reconciliation & Discrepancies
Host lookup was performed using the trade reference `OA38238234`.

| Field | Email Value | Host Value | Status | Severity |
|---|---|---|---|---|
| Reference Number | OA38238234 | OA38238234 | Match | None |
| Security ISIN | *Missing* | US0378331005 | Missing in Email | None |
| Settlement Date | 2026-03-16 | 2026-03-16 | Match | None |
| Trade Date | 2026-03-13 | 2026-03-13 | Match | None |
| Quantity | 51993 | 51993 | Match | None |
| Amount | 1915019.39 | 1915019.39 | Match | None |
| Currency | CHF | CHF | Match | None |
| Side | *Missing* | Sale | Missing in Email | Medium |
| Counterparty | Meridian Funds | ANGGYXNX0JLX3X63W380 | Mismatch | High |

**Discrepancy Notes:**
* Counterparty enrichment call (`/counterparty?name=Meridian Funds`) returned 404. Unable to confirm that 'Meridian Funds' maps to host counterparty identifier `ANGGYXNX0JLX3X63W380`.
* Security name/ISIN absent in the email; host reports security ISIN `US0378331005`.
* Trade side missing in email (host indicates 'Sale').

## 5. Evidence & Attachments
**Evidence:**
* *Subject:* "Trade Inquiry – Reference OA38238234" (Supports: Reference Number)
* *Body:* "documentation appears to be incomplete. Several key fields required for processing are absent." (Supports: Documentation Missing)
* *Body:* "Amount 1915019.39; Val Dt 2026.03.16; Ref No OA38238234; Trade Date 2026.03.13; Currency CHF; Quantity 51993" (Supports: Trade Facts)

**Attachments:**
* No attachments present.

## 6. Recommended Next Steps
1. **Confirm Counterparty Identity:** Verify the counterparty LEI/ID mapping or legal name for "Meridian Funds" against host identifier `ANGGYXNX0JLX3X63W380`.
2. **Request Missing Details:** Contact the sender to provide the missing security details (ISIN or security name) and the trade side.
3. **Hold Settlement:** Do not proceed with settlement processing until the counterparty identity is confirmed and missing critical fields are verified.