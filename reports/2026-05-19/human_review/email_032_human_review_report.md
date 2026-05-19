# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required: booking desk/operations should confirm whether reference IT87021310 was assigned in error or provide the correct booking reference. Provide host system search results and attach the sender's extracted trade details (attachment) to assist manual reconciliation.

**Reason:** HOST returned 404 for reference_number=IT87021310; no host trade found. Because the reference is present in the email and attachment but not in HOST, human-in-the-loop is required to avoid unsafe assumptions.

---

## 2. Email Summary

**Email ID:** email_032.eml  
**Subject:** Query: Buy of Deutsche Bank AG [IT87021310]  
**Sender:** John Smith <j.smith@globalcapital.com>  
**Received:** Tue, 28 Apr 2026 15:38:47 +0200  
**Counterparty:** UBS

The sender cannot reconcile the referenced closed trade against any booking and requests confirmation or corrected reference.

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
| reference_number | IT87021310 | null | missing_in_host | high |
| security_isin | null | null | missing_in_email | none |
| security_name | Deutsche Bank AG | null | missing_in_host | medium |
| settlement_date | 2026-03-10 | null | missing_in_host | high |
| trade_date | 2026-03-09 | null | missing_in_host | medium |
| quantity | 62256 | null | missing_in_host | medium |
| amount | 1716867.31 | null | missing_in_host | high |
| currency | CHF | null | missing_in_host | low |
| side | buy | null | missing_in_host | low |
| counterparty_name | UBS | null | missing_in_host | medium |
| status | closed | null | missing_in_host | medium |

### Discrepancy Flags
- trade_not_found_in_host
- sender_requests_reference_confirmation

---

## 6. Findings

The trade was not found in HOST. The HOST `/trades` lookup by reference returned 404 (no match).
Email extraction (including PDF attachment) is high-confidence and consistently reports trade details for IT87021310.
No HOST enrichment was possible; reconciliation depends on human confirmation of whether reference is incorrect or missing in host bookings.

---

## 7. Next Steps

1. Manually review the email and the attached `trade_details.pdf`.
2. Verify if the trade reference IT87021310 was assigned in error or if the booking is missing in the host system.
3. Check internal systems for any trades matching the provided details (Deutsche Bank AG, 62256 units, CHF 1716867.31, settlement 2026-03-10).
4. Contact the counterparty to confirm the correct reference number or provide the missing booking details.

---
