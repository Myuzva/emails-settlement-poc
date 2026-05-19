# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Investigate settlement date discrepancy. Host reflects 2026-03-23, while email requests 2026-04-23.

**Reason:** A human in the loop is required due to a high-severity mismatch in the settlement date between the email instruction and the internal HOST booking.

---

## 2. Email Summary

**Email ID:** email_009  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** HSBC

The counterparty reports a value date mismatch on trade BP86251923. Their internal booking reflects 23.03.2026, whereas the instruction received indicates 23.04.2026.

---

## 3. Classification
- **Primary Type:** settlement_date_mismatch
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | BP86251923 | BP86251923 | match | none |
| security_isin | null | DE0007236101 | missing_in_email | none |
| security_name | Siemens AG | Siemens AG | match | none |
| settlement_date | 2026-04-23 | 2026-03-23 | mismatch | high |
| trade_date | 2026-03-20 | 2026-03-20 | match | none |
| quantity | 67180 | 67180 | match | none |
| amount | 313757.36 | 313757.36 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | sell | match | none |
| counterparty_name | HSBC | HSBC | match | none |
| status | unknown | Offen | missing_in_email | none |

### Discrepancy Flags
- settlement_date_mismatch

---

## 6. Findings

The trade was found in HOST, but the settlement date differs from the counterparty’s email. The email instruction indicates 2026-04-23, while HOST reflects 2026-03-23.

The likely cause of the settlement break is a settlement date mismatch. The case should be reviewed before any confirmation is sent externally.

---

## 7. Next Steps

1. Verify the correct settlement date against internal trade booking records.

2. Confirm whether the counterparty is referencing the same trade reference.

3. Ask the counterparty to confirm the expected settlement date.

4. Keep the case under analyst review until the discrepancy is resolved.

---