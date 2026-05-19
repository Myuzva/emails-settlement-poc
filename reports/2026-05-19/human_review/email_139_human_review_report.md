# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Manual investigation required: operations should search booking systems and alternative host indices for NU59609287 using trade attributes.

**Reason:** The counterparty reports the trade as settled externally, but it cannot be located in the booking system (HOST lookup returned 404). Human review is required to investigate the missing trade.

---

## 2. Email Summary

**Email ID:** email_139.eml  
**Subject:** Reconciliation Query – NU59609287 – UBS Group AG  
**Sender:** Michael Hartmann <m.hartmann@eurofin.de>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Société Générale

The sender cannot locate the trade in its booking system although it appears settled in external records and requests confirmation or clarification.

---

## 3. Classification
- **Primary Type:** generic_trade_details_request (originally reconciliation_query_trade_lookup)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | NU59609287 | null | missing_in_host | high |
| security_isin | null | null | unknown | none |
| security_name | UBS Group AG | null | missing_in_host | high |
| settlement_date | 2025-11-28 | null | missing_in_host | high |
| trade_date | 2025-11-27 | null | missing_in_host | medium |
| quantity | 75593 | null | missing_in_host | high |
| amount | 534538.78 | null | missing_in_host | high |
| currency | USD | null | missing_in_host | high |
| side | buy | null | missing_in_host | medium |
| counterparty_name | Société Générale | null | missing_in_host | high |
| status | settled | null | missing_in_host | medium |

### Discrepancy Flags
- trade_not_found_on_host
- key_fields_missing_in_host
- external_record_reports_settled

---

## 6. Findings

The trade was not found in HOST (404 Not Found for reference NU59609287). The email and attachment provide complete trade attributes, but the absence of a host record prevents automated reconciliation. The counterparty explicitly requests confirmation of an externally settled record that is missing internally.

---

## 7. Next Steps

1. Search booking systems and alternative host indices for NU59609287 using trade attributes (settlement date 2025-11-28, security UBS Group AG, quantity 75593, amount 534,538.78 USD).
2. Check external settlement feeds and verify counterparty mapping for Société Générale (including alternate spellings/identifiers like SG, SocGen).
3. Consider searching by related external references or trade lifecycle messages.
4. Escalate to the settlement desk for further investigation.

---