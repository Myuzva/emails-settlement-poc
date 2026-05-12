# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Manual investigation required: Trade NU59609287 was not found in the HOST system using either the reference number or the trade details provided in the email.

**Reason:** The trade is missing in the HOST system (404 Not Found).

---

## 2. Email Summary

**Email ID:** email_139  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Société Générale

Email requests clarification on an unrecognized trade that appears as settled in external records. Trade details extracted from attached ZIP containing a PDF.

---

## 3. Classification
- **Primary Type:** general_status_request (originally generic_trade_details_request)
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
| security_name | UBS Group AG | null | missing_in_host | high |
| isin | null | null | unknown | none |
| settlement_date | 2025-11-28 | null | missing_in_host | high |
| trade_date | 2025-11-27 | null | missing_in_host | high |
| quantity | 75593 | null | missing_in_host | high |
| amount | 534538.78 | null | missing_in_host | high |
| currency | USD | null | missing_in_host | high |
| side | buy | null | missing_in_host | high |
| counterparty_name | Société Générale | null | missing_in_host | high |

### Discrepancy Flags
- trade_not_found_in_host

---

## 6. Findings

The trade NU59609287 was not found in the HOST system using either the reference number or the trade details provided in the email. Security and Counterparty data were successfully enriched but did not lead to a trade match.

---

## 7. Next Steps

1. Verify if the trade exists under a different identifier in internal booking systems.

2. Request clarification from the counterparty regarding the external records showing the trade as settled.

3. Keep the case under analyst review until the discrepancy is resolved.

---