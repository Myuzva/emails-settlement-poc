# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required to determine whether trade IP36951687 should be newly booked, resubmitted, or investigated further because HOST returned no match for the provided reference number.

**Reason:** HOST trade not found (`no_match`). The sender also reports they are unable to locate a matching record.

---

## 2. Email Summary

**Email ID:** email_148.eml  
**Subject:** Trade Exception – IP36951687  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Citigroup

The sender states they cannot locate a matching record in their system and asks the recipient to verify the trade details and confirm whether this is a new booking or a resubmission.

---

## 3. Classification
- **Primary Type:** generic_trade_details_request (originally generic_trade_details_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | IP36951687 | null | unknown | high |
| security_name | Roche Holding AG | null | unknown | medium |
| isin | null | null | missing_in_email | none |
| trade_date | 2025-12-22 | null | unknown | medium |
| settlement_date | 2025-12-23 | null | unknown | medium |
| side | buy | null | unknown | medium |
| quantity | 98076 | null | unknown | medium |
| amount | 1538459.01 | null | unknown | medium |
| currency | EUR | null | unknown | medium |
| counterparty_name | Citigroup | null | unknown | medium |
| status | unknown | null | unknown | none |

### Discrepancy Flags
- host_trade_not_found
- sender_reports_unable_to_locate_matching_record

---

## 6. Findings

A HOST lookup was performed using the provided reference number (IP36951687), but no matching trade was found. The email contains a complete and internally consistent primary trade, but no HOST trade is available for field-by-field reconciliation. The sender also reports they are unable to locate a matching record in their system.

---

## 7. Next Steps

1. Investigate internally why trade IP36951687 is missing from the HOST system.
2. Determine if the trade needs to be newly booked or resubmitted.
3. Respond to the counterparty with the verified trade details and confirmation of the booking status.
4. Keep the case under analyst review until the discrepancy is resolved.

---