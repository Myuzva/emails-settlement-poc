# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Human review required to resolve amount discrepancy. HOST records match the sender's claimed 'correct' amount (244,106.23 USD) but differ from the reported 'settled' amount (481,263.40 USD).

**Reason:** The email explicitly states a discrepancy in the settled amount versus the correct amount, and HOST reconciliation confirms a high-severity amount mismatch.

---

## 2. Email Summary

**Email ID:** email_091.eml  
**Subject:** Unknown  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** BNP Paribas

The trade appears to have been settled at 481,263.40 USD, whereas our records indicate the correct amount should be 244,106.23 USD.

---

## 3. Classification
- **Primary Type:** wrong_amount (originally amount_mismatch)
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
| status | closed | Closed | match | none |

### Discrepancy Flags
- amount_mismatch

---

## 6. Findings

The trade was found in HOST, but the settlement amount differs from the counterparty’s reported settled amount.
HOST records match the sender's claimed 'correct' amount (244,106.23 USD) but differ from the reported 'settled' amount (481,263.40 USD).

---

## 7. Next Steps

1. Verify the correct settlement amount against internal trade booking records and payment instructions.
2. Confirm whether the counterparty is referencing the same trade reference and if a partial settlement or fee was applied.
3. Ask the counterparty to provide further details on how the 481,263.40 USD figure was derived.
4. Keep the case under analyst review until the discrepancy is resolved.

---
