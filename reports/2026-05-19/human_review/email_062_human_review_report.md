# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Route to human review. HOST returned no trade for the provided reference EP95329750, while the sender reports the trade appears in external documentation as closed and asks whether it was booked under an alternative reference or included in the settlement file in error.

**Reason:** HOST returned no trade for the provided reference EP95329750, while the sender reports the trade appears in external documentation as closed.

---

## 2. Email Summary

**Email ID:** email_062  
**Subject:** Trade Exception – EP95329750  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Santander

The sender reports a reconciliation exception for a specific trade reference and asks whether it was booked under an alternative reference or included in the settlement file in error.

---

## 3. Classification
- **Primary Type:** status_unknown (originally generic_trade_details_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | EP95329750 | null | unknown | high |
| security_name | Novartis AG | null | unknown | medium |
| isin | null | null | missing_in_email | none |
| trade_date | 2026-01-27 | null | unknown | medium |
| settlement_date | 2026-01-28 | null | unknown | medium |
| side | sell | null | unknown | medium |
| quantity | 20185 | null | unknown | medium |
| amount | 612506.76 | null | unknown | medium |
| currency | EUR | null | unknown | medium |
| counterparty_name | Santander | null | unknown | medium |
| status | closed | null | unknown | medium |

### Discrepancy Flags
- host_trade_not_found
- sender_reports_no_internal_record
- external_documentation_reported_closed

---

## 6. Findings

HOST returned no trade for the provided reference EP95329750. The sender reports the trade appears in external documentation as closed and asks whether it was booked under an alternative reference or included in the settlement file in error. No HOST trade was available for field-by-field reconciliation; HOST-side values are therefore unknown rather than treated as direct mismatches.

---

## 7. Next Steps

1. Investigate internal systems for possible alternative booking reference for the trade details provided (Novartis AG, 20185 units, EUR 612506.76).

2. Verify if the trade was erroneously included in the settlement file.

3. Respond to the sender confirming the correct booking reference or acknowledging the erroneous inclusion.

---