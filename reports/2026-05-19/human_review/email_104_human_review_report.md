# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Route to analyst review for ISIN verification.

**Reason:** Conflicting security values in the email require verification of correct instrument/ISIN. Correct ISIN is requested but not present in email or attachment.

---

## 2. Email Summary

**Email ID:** email_104  
**Subject:** Reconciliation Query – MB75276355 – Swiss Re AG  
**Sender:** James O'Brien <j.obrien@meridianfunds.co.uk>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Citigroup

The sender reports a discrepancy in the instrument identifier for trade MB75276355, noting BASF SE on their books versus Swiss Re AG in the trade notification, and requests correct ISIN verification.

---

## 3. Classification
- **Primary Type:** wrong_security (originally security_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | MB75276355 | N/A | pending | none |
| security_isin | null | N/A | pending | none |
| security_name | Swiss Re AG / BASF SE | N/A | mismatch | high |
| settlement_date | 2026-03-10 | N/A | pending | none |
| trade_date | 2026-03-09 | N/A | pending | none |
| quantity | 21635 | N/A | pending | none |
| amount | 1546104.19 | N/A | pending | none |
| currency | USD | N/A | pending | none |
| side | buy | N/A | pending | none |
| counterparty_name | Citigroup | N/A | pending | none |
| status | unknown | N/A | pending | none |

### Discrepancy Flags
- Instrument/security identifier mismatch: sender books show BASF SE while trade notification and attachment reference Swiss Re AG; sender requests correct ISIN verification and re-booking advice.

---

## 6. Findings

The email explicitly states a discrepancy in the instrument identifier. The sender contrasts BASF SE on their books with Swiss Re AG in the trade notification. The attachment contains the referenced trade and security description Swiss Re AG. Correct ISIN is requested but not present in the email or attachment.

---

## 7. Next Steps

1. Verify the correct instrument/ISIN for trade MB75276355 against internal trade booking records.

2. Confirm whether the correct security is BASF SE or Swiss Re AG.

3. Provide the correct ISIN and re-booking advice to the counterparty.

4. Keep the case under analyst review until the discrepancy is resolved.

---