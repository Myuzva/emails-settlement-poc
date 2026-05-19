# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required: host system returned no trade for reference PH61323120. Please verify with operations/tech that reference was searched correctly and confirm trade details with the counterparty (Morgan Stanley). Consider running a field-based host lookup (settlement date/security/quantity/amount) and/or checking alternate host systems if available.

**Reason:** Host lookup by trade reference returned 404 (no match). The trade could not be found in the host system.

---

## 2. Email Summary

**Email ID:** email_166  
**Subject:** Query: Verkauf of BASF SE [PH61323120]  
**Sender:** Thomas Müller <t.mueller@rheinasset.de>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Morgan Stanley

The sender states they have no record of the referenced trade and requests confirmation of trade details. The attachment provides a single trade candidate with reference, security, dates, quantity, amount and currency.

---

## 3. Classification
- **Primary Type:** generic_trade_details_request
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | PH61323120 | null | missing_in_host | high |
| security_name | BASF SE | null | missing_in_host | high |
| isin | null | null | missing_in_email | none |
| trade_date | 2026-01-25 | null | missing_in_host | high |
| settlement_date | 2026-01-26 | null | missing_in_host | high |
| quantity | 24489 | null | missing_in_host | high |
| amount | 189842.96 | null | missing_in_host | high |
| currency | CHF | null | missing_in_host | high |
| side | sell | null | missing_in_host | high |
| counterparty_name | Morgan Stanley | null | missing_in_host | high |
| reported_status | unknown | null | missing_in_host | medium |

### Discrepancy Flags
- trade_not_found_on_host
- critical_fields_missing_on_host

---

## 6. Findings

The host system returned no trade for reference PH61323120. The email extraction confidence is high (0.93) and the attachment provides clear trade data, but the absence on the host makes automated matching unreliable.

---

## 7. Next Steps

1. Verify with operations/tech that the reference was searched correctly.
2. Consider running a field-based host lookup (settlement date/security/quantity/amount) and/or checking alternate host systems if available.
3. Confirm trade details with the counterparty (Morgan Stanley).
4. Keep the case under analyst review until the discrepancy is resolved.

---