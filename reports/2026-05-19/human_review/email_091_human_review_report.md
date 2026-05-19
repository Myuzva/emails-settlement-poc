# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required: confirm which amount is authoritative (host 244,106.23 USD vs sender reported settled 481,263.40 USD). Investigate ledger/settlement records, check payment/settlement instructions, and, if host is correct, advise sender on adjustment/correction process. Also resolve security mapping (map ISIN DE0007664005 to 'Volkswagen AG') to remove the name/identifier gap before actioning any adjustment.

**Reason:** Host trade amount (244,106.23 USD) differs materially from email/attachment reported settled amount (481,263.40 USD). Because the amount is a sensitive financial field and differs between sources, automated resolution is unsafe — human intervention recommended.

---

## 2. Email Summary

**Email ID:** email_091  
**Subject:** Trade Inquiry – Reference GS58538212  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** BNP Paribas

The sender reports trade was settled at USD 481,263.40 but their records indicate the correct amount should be USD 244,106.23 and asks how to process an adjustment or correction.

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
| security_name | Volkswagen AG | null | missing_in_host | medium |
| settlement_date | 2026-03-11 | 2026-03-11 | match | none |
| trade_date | 2026-03-10 | 2026-03-10 | match | none |
| quantity | 42781 | 42781 | match | none |
| amount | 481263.40 | 244106.23 | mismatch | high |
| currency | USD | USD | match | none |
| side | sell | Sale | match | none |
| counterparty_name | BNP Paribas | BNP Paribas (LEI R0MUWSFPU8MPRO8K5P83) | match | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- amount_mismatch
- security_identifier_only_in_host
- counterparty_matched_by_lei

---

## 6. Findings

The trade was found in HOST, but the settlement amount differs from the counterparty’s email. The host amount (244,106.23 USD) matches the sender's expected amount, but differs from the reported settled amount (481,263.40 USD). Additionally, the security identifier is only present as an ISIN in the host and as a name in the email.

The likely cause of the settlement break is an amount mismatch. The case should be reviewed before any confirmation is sent externally.

---

## 7. Next Steps

1. Verify the correct amount against internal trade booking records.

2. Confirm whether the counterparty is referencing the same trade reference.

3. Ask the counterparty to confirm the expected amount and settlement details.

4. Keep the case under analyst review until the discrepancy is resolved.

---