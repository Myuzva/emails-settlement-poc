# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Analyst review required to resolve amount discrepancy.

**Reason:** Amount values conflict within the email for the primary trade. The body explicitly states an inconsistency in the booked amount for trade KN56349555, and the attachment trade details support one of the quoted USD amounts for the same trade reference.

---

## 2. Email Summary

**Email ID:** email_038.eml  
**Subject:** Trade Confirmation Request – KN56349555 (+ 1 more)  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Unknown  
**Counterparty:** UBS

The sender reports a booked amount inconsistency for trade KN56349555 and asks which USD amount is correct before the value date. The email body quotes 1748410.65 USD, while the trade advice quotes 1471393.36 USD.

---

## 3. Classification
- **Primary Type:** amount_mismatch
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** HD63576518 (Raiffeisen Bank, NVIDIA Corp., USD 2666420.07)

---

## 5. HOST Lookup Comparison

HOST lookup was not performed as the case was routed to human review due to conflicting data within the email.

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | KN56349555 | null | N/A | none |
| security_isin | null | null | N/A | none |
| security_name | Roche Holding AG | null | N/A | none |
| settlement_date | 2026-03-19 | null | N/A | none |
| trade_date | 2026-03-18 | null | N/A | none |
| quantity | 68443 | null | N/A | none |
| amount | 1471393.36 / 1748410.65 | null | N/A | none |
| currency | USD | null | N/A | none |
| side | buy | null | N/A | none |
| counterparty_name | UBS | null | N/A | none |
| status | unknown | null | N/A | none |

### Discrepancy Flags
- **Amount Mismatch:** Sender reports a booked amount inconsistency and asks which USD amount is correct before value date. Sender value: 1748410.65, Expected/Requested value: 1471393.36.

---

## 6. Findings & Next Steps

**Findings:**
- The email body explicitly states an inconsistency in the booked amount for trade KN56349555. The sender shows 1748410.65 USD, but the trade advice quotes 1471393.36 USD.
- The attachment trade details support the 1471393.36 USD amount for the same trade reference.
- The attachment contains an additional mentioned trade (HD63576518) not discussed in the email body.

**Next Steps:**
1. Review internal booking records for trade KN56349555 to determine the correct settlement amount.
2. Clarify the correct amount with the counterparty (UBS).
3. Verify if any action is needed for the additional trade (HD63576518) mentioned in the attachment.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for reaching out regarding trade KN56349555. 

We are currently reviewing the booked amount inconsistency (1,748,410.65 USD vs 1,471,393.36 USD) with our internal teams. We will provide you with the correct settlement amount as soon as possible before the value date.

Best regards,
Settlement Operations
```