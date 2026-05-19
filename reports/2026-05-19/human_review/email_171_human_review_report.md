# Settlement Discrepancy Report: YN21200009

**Date:** 2026-05-19
**Status:** NEEDS HUMAN REVIEW
**Confidence Score:** 62%
**Source Email:** email_171.eml

## Executive Summary
A counterparty mismatch discrepancy was identified for trade **YN21200009**. The sender (Anna Kowalski) reports that the trade is currently booked with **HSBC**, but their agreement confirms it should be **Citigroup**. They are requesting a procedure to re-open or amend the closed/settled trade. Host reconciliation found the trade, but the host counterparty is an opaque identifier (`E57ODZWZ7FF32TWEFA76`), requiring manual mapping and verification.

## Discrepancy Analysis

| Field | Email Value | Host Value | Status | Severity |
| :--- | :--- | :--- | :--- | :--- |
| Reference Number | YN21200009 | YN21200009 | Match | None |
| Security ISIN | *Missing* | DE000BASF111 | Missing in Email | None |
| Security Name | BASF SE | *Missing* | Missing in Host | Low |
| Settlement Date | 2026-03-23 | 2026-03-23 | Match | None |
| Trade Date | 2026-03-20 | 2026-03-20 | Match | None |
| Quantity | 77,982 | 77,982 | Match | None |
| Amount | 1,301,274.03 | 1,301,274.03 | Match | None |
| Currency | EUR | EUR | Match | None |
| Side | buy | Buy | Match | None |
| Counterparty | HSBC | E57ODZWZ7FF32TWEFA76 | Mismatch | High |
| Status | settled | Closed | Match | Low |

### Discrepancy Flags
* `counterparty_mismatch`
* `counterparty_identifier_difference`
* `security_isin_missing_in_email`

## Host System Data
```json
{
  "Reference Number": "YN21200009",
  "Buy Sale": "Buy",
  "Settlement Date": "2026-03-23",
  "Transaction Date": "2026-03-20",
  "Security": "DE000BASF111",
  "Status": "Closed",
  "Amount": 1301274.03,
  "Currency": "EUR",
  "Quantity": 77982,
  "Counterparty": "E57ODZWZ7FF32TWEFA76"
}
```

## Evidence & Attachments
* **Attachment:** `trade_details.pdf` (Parsed via pdf_text)
  * *Quote:* "Buy; Trans Dt 2026-03-20; Trade Ccy EUR; Settlement Date 2026-03-23; Amount 1,301,274.03; Nom 77,982; Broker HSBC; Security Desc BASF SE"
* **Email Body:**
  * *Quote:* "retrospective counterparty error on trade YN21200009, which is currently marked as settled and closed"
  * *Quote:* "The booking reflects HSBC as the counterparty; however, our agreement confirms this should be Citigroup."

## Recommended Actions
**Human review required:** Verify the host counterparty identifier (`E57ODZWZ7FF32TWEFA76`) and map to the expected legal entity (sender requests Citigroup). Enrich counterparty via HOST counterparty lookup (or internal reference) to confirm whether host ID corresponds to HSBC or another legal entity. If confirmed incorrect, follow escalation to re-open/amend settled trade per firm policy. Also consider security lookup to confirm DE000BASF111 maps to BASF SE for record completeness.