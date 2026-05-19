# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Investigate why trade IP36951687 is missing from the HOST system. The sender also reports being unable to locate the record in their system.

**Reason:** The trade is missing in the HOST system (404 Not Found), and the sender also reports being unable to locate the record.

---

## 2. Email Summary

**Email ID:** email_148.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Citigroup

The sender received a trade notification but cannot find the trade in their system.

---

## 3. Classification
- **Primary Type:** missing_confirmation (originally confirmation_missing)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | IP36951687 | null | missing_in_host | high |
| security_name | Roche Holding AG | Roche Holding AG | match | none |
| isin | null | CH0012032048 | missing_in_email | none |
| settlement_date | 2025-12-23 | null | missing_in_host | high |
| trade_date | 2025-12-22 | null | missing_in_host | high |
| quantity | 98076 | null | missing_in_host | high |
| amount | 1538459.01 | null | missing_in_host | high |
| currency | EUR | null | missing_in_host | high |
| side | buy | null | missing_in_host | high |
| counterparty_name | Citigroup | Citigroup | match | none |
| status | unknown | null | missing_in_host | medium |

### Discrepancy Flags
- trade_not_found_in_host

---

## 6. Findings

The trade IP36951687 was not found in the HOST system (404 Not Found). The sender also explicitly states: "we are unable to locate a matching record in our system".

Security and counterparty names were successfully validated against HOST reference data, but the trade itself is missing from both sides.

---

## 7. Next Steps

1. Verify if the trade exists under a different identifier in internal booking systems.
2. Confirm with internal trading desks if this trade was cancelled, booked incorrectly, or never executed.
3. Respond to the counterparty to confirm the trade status once internal investigation is complete.
4. Keep the case under analyst review until the discrepancy is resolved.

---