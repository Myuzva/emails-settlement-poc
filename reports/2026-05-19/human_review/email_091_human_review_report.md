# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Route to human review for settlement amount discrepancy investigation.

**Reason:** HOST amount is 244,106.23 USD while email facts report settled/net amount 481,263.40 USD; this is material and aligns with the sender's stated mismatch claim.

---

## 2. Email Summary

**Email ID:** email_091  
**Subject:** Trade Inquiry – Reference GS58538212  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** 2026-04-28 15:38:48 +0200  
**Counterparty:** BNP Paribas

The sender reports the trade settled/net amount is 481,263.40 USD but their records indicate the correct amount should be 244,106.23 USD and requests adjustment/correction procedure.

---

## 3. Classification
- **Primary Type:** amount_mismatch (originally amount_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | GS58538212 | GS58538212 | match | none |
| security_isin | null | DE0007664005 | missing_in_email | none |
| security_name | Volkswagen AG | Volkswagen AG | match | none |
| settlement_date | 2026-03-11 | 2026-03-11 | match | none |
| trade_date | 2026-03-10 | 2026-03-10 | match | none |
| quantity | 42781 | 42781 | match | none |
| amount | 481263.40 | 244106.23 | mismatch | high |
| currency | USD | USD | match | none |
| side | sell | Sale | match | none |
| counterparty_name | BNP Paribas | BNP Paribas | match | none |
| counterparty_lei | null | R0MUWSFPU8MPRO8K5P83 | missing_in_email | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- amount_mismatch

---

## 5. Findings

The trade was found in HOST, but the settlement amount differs significantly from the counterparty’s email.

The likely cause of the settlement break is an amount mismatch. The email explicitly states the trade was settled at 481,263.40 USD while sender records indicate a different correct amount (244,106.23 USD). The HOST system confirms the amount as 244,106.23 USD. The case should be reviewed before any confirmation is sent externally.

---

## 6. Next Steps

1. Verify the correct amount against internal trade booking records.

2. Confirm whether the counterparty is referencing the same trade reference and if any partial settlements occurred.

3. Ask the counterparty to confirm the expected settlement amount and provide further breakdown if necessary.

4. Keep the case under analyst review until the discrepancy is resolved.

---