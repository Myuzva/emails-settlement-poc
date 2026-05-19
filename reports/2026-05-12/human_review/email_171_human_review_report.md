# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Investigate why the sender believes the booking reflects HSBC when the HOST system correctly shows Citigroup. Confirm with the sender that the trade is correctly booked as Citigroup.

**Reason:** The sender explicitly states that the booking reflects HSBC as the counterparty, but their agreement confirms it should be Citigroup. A human in the loop is required to clarify the discrepancy between the sender's records and the HOST system, which already reflects Citigroup.

---

## 2. Email Summary

**Email ID:** email_171.eml  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** HSBC (Sender claims booking reflects HSBC, expected Citigroup)

The sender reports a counterparty mismatch for trade YN21200009. The booking reflects HSBC as the counterparty, but their agreement confirms it should be Citigroup. Trade details were extracted from the attached PDF.

---

## 3. Classification
- **Primary Type:** wrong_counterparty (originally counterparty_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | YN21200009 | YN21200009 | match | none |
| security_isin | null | DE000BASF111 | missing_in_email | none |
| security_name | BASF SE | BASF SE | match | none |
| settlement_date | 2026-03-23 | 2026-03-23 | match | none |
| trade_date | 2026-03-20 | 2026-03-20 | match | none |
| quantity | 77982 | 77982 | match | none |
| amount | 1301274.03 | 1301274.03 | match | none |
| currency | EUR | EUR | match | none |
| side | buy | Buy | match | none |
| counterparty_name | HSBC | Citigroup | mismatch | high |
| status | settled | Closed | match | none |

### Discrepancy Flags
- counterparty_mismatch

---

## 6. Findings

The trade was found in HOST by reference number. All trade details match except for the counterparty. The HOST counterparty (Citigroup) matches the sender's expected value, but mismatches the value reported as 'currently booked' (HSBC) in the email.

The likely cause of the settlement break is a counterparty mismatch in the sender's view of the booking. The case should be reviewed to confirm the correct counterparty with the sender.

---

## 7. Next Steps

1. Verify the correct counterparty against internal trade booking records.
2. Confirm with the sender that the trade is correctly booked as Citigroup in our HOST system.
3. Ask the sender to update their records if necessary.
4. Keep the case under analyst review until the discrepancy is resolved.
