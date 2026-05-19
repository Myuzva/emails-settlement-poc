# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Route to analyst review to resolve security mismatch and verify ISIN.

**Reason:** Instrument/security values conflict: the email body states Alphabet Inc. on sender books, while the trade notification/PDF reference Microsoft Corp. The email requests verification of the correct ISIN, but no ISIN is provided.

---

## 2. Email Summary

**Email ID:** email_019  
**Subject:** Unmatched Trade – Microsoft Corp. – QR20201268  
**Sender:** Thomas Müller <t.mueller@rheinasset.de>  
**Received:** 2026-04-28T15:38:47+02:00  
**Counterparty:** Deutsche Bank

The sender reports an unmatched trade due to an instrument identifier discrepancy. Their books show Alphabet Inc., but the trade notification references Microsoft Corp. They requested ISIN verification, but no ISIN was provided in the email or attachment.

---

## 3. Classification
- **Primary Type:** security_mismatch
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | QR20201268 | N/A | pending | none |
| security_isin | null | N/A | missing_in_email | none |
| security_name | Microsoft Corp. (Alphabet Inc. in body) | N/A | conflict | high |
| settlement_date | 2026-03-10 | N/A | pending | none |
| trade_date | 2026-03-09 | N/A | pending | none |
| quantity | 75634 | N/A | pending | none |
| amount | 605945.09 | N/A | pending | none |
| currency | EUR | N/A | pending | none |
| side | buy | N/A | pending | none |
| counterparty_name | Deutsche Bank | N/A | pending | none |
| status | unknown | N/A | pending | none |

### Discrepancy Flags
- **Security Mismatch:** Sender reports Alphabet Inc. on their books, but the trade notification and attachment show Microsoft Corp.

---

## 6. Findings

The email contains conflicting security names: the body mentions "Alphabet Inc." while the subject and attached PDF reference "Microsoft Corp.". The sender requested verification of the correct ISIN, but no ISIN was provided in the email or attachment. HOST lookup was not performed as the case requires human review to resolve the ambiguity first.

---

## 7. Next Steps

1. Review the trade reference QR20201268 in the internal system to determine the correct security (Alphabet Inc. vs. Microsoft Corp.).
2. Identify the correct ISIN for the traded security.
3. Reply to the counterparty clarifying the correct security name and providing the requested ISIN.
