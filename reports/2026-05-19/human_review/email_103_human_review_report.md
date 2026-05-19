# Settlement Discrepancy Report: VE93513959 / email_103.eml

| Field | Value |
| --- | --- |
| **Date Generated** | 2026-05-19 |
| **Email File** | email_103.eml |
| **Sender** | Anna Kowalski <a.kowalski@warsawsec.pl> |
| **Subject** | Settlement Query – ABB Ltd. – 2026-03-04 |
| **Status** | Needs Human Review |
| **Confidence Score** | 86% |

## 1. Case Summary
The sender is requesting archival settlement confirmation or trade advice for a closed trade (VE93513959). The trade details were extracted from the email body and the attached PDF (`trade_details.pdf`). Host reconciliation found a matching trade by reference number, but flagged discrepancies regarding the counterparty identifier and missing security name mapping.

## 2. Extracted Trade Details

| Field | Email/Attachment Value | Host Value | Status | Severity |
| --- | --- | --- | --- | --- |
| **Reference Number** | VE93513959 | VE93513959 | Match | None |
| **Security Name** | ABB Ltd. | *Missing* | Missing in Host | Low |
| **Security ISIN** | *Missing* | CH0012530207 | Missing in Email | None |
| **Settlement Date** | 2026-03-04 | 2026-03-04 | Match | None |
| **Trade Date** | 2026-03-03 | 2026-03-03 | Match | None |
| **Quantity** | 46,388 | 46,388 | Match | None |
| **Amount** | 1,662,949.54 | 1,662,949.54 | Match | None |
| **Currency** | CHF | CHF | Match | None |
| **Side** | buy | Kauf | Match | None |
| **Counterparty** | ING Bank | REDACTED_IDENTIFIER | Mismatch | High |
| **Status** | closed | Geschlossen | Match | None |

## 3. Discrepancy Analysis
- **Counterparty Mismatch:** The email specifies "ING Bank" as the counterparty, whereas the host system returns a redacted identifier (`REDACTED_IDENTIFIER`). This requires human confirmation to ensure the identifier maps correctly to ING Bank.
- **Security Mapping:** The email provides the security name "ABB Ltd." but lacks an ISIN. The host provides the ISIN "CH0012530207" but lacks the security name.
- **Language Differences:** Host values for Side ("Kauf") and Status ("Geschlossen") are in German, which correctly map to "buy" and "closed".

## 4. Evidence & Attachments
- **Attachment:** `trade_details.pdf` (Parsed successfully)
- **Quote (Body):** *"requesting the archival documentation for trade VE93513959, which is recorded as closed in our system"*
- **Quote (Body):** *"Please provide a copy of the relevant settlement confirmation or trade advice for our records"*
- **Quote (Attachment):** *"Value Date 04.03.2026; Counterpart ING Bank; Notional 1662949.54; Direction Kauf; Nominal 46388; Security Desc ABB Ltd.; Currency CHF; Trd Dt 03.03.2026"*

## 5. Recommended Action
**Human review required:** Confirm the mapping between the host counterparty identifier (`REDACTED_IDENTIFIER`) and 'ING Bank'. If confirmed, provide the requested archival settlement confirmation / trade advice to the sender. Optionally, enrich the host record with the security name for ISIN CH0012530207 to confirm the 'ABB Ltd.' mapping.