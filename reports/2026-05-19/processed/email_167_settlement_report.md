# MAIA Settlement Mailbox Report - email_167.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing. HOST trade was matched by reference number and core provided facts reconcile; use HOST values to complete missing documentation fields, especially currency USD and security identifier US67066G1040.
**Reason:** Settlement/trade-related documentation update request with clear trade reference for HOST lookup.

---

## 2. Email Summary

**Email ID:** email_167  
**Subject:** Trade Status Update Request – HJ10386713  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** UniCredit

Sender reports incomplete documentation on file and requests missing information/complete trade details for a closed settled transaction.

---

## 3. Classification
- **Primary Type:** instruction_or_document_update
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | HJ10386713 | HJ10386713 | match | none |
| counterparty_name | UniCredit | UniCredit | match | none |
| counterparty_identifier | null | F1T87K3OQ2OV1UORLH26 | missing_in_email | low |
| security_isin | null | US67066G1040 | missing_in_email | none |
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| side | sell | Sale | match | none |
| quantity | 72417 | 72417 | match | none |
| amount | 1650395.89 | 1650395.89 | match | none |
| currency | null | USD | missing_in_email | medium |
| status | closed | Closed | match | none |

### Discrepancy Flags
- currency_missing_in_email
- security_identifier_missing_in_email
- counterparty_identifier_missing_in_email
- documentation_missing_claim

---

## 6. Recommended Action
- [x] Proceed with standard processing. HOST trade was matched by reference number and core provided facts reconcile; use HOST values to complete missing documentation fields, especially currency USD and security identifier US67066G1040.
- [ ] Respond to requester providing the missing trade details (Currency: USD, Security: US67066G1040, Counterparty LEI: F1T87K3OQ2OV1UORLH26).

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email regarding trade HJ10386713.

We can confirm the following complete trade details from our system to assist with your documentation:
- Reference Number: HJ10386713
- Counterparty: UniCredit (LEI: F1T87K3OQ2OV1UORLH26)
- Security: US67066G1040
- Trade Date: 2026-03-12
- Settlement Date: 2026-03-13
- Side: Sale
- Quantity: 72,417
- Amount: 1,650,395.89
- Currency: USD
- Status: Closed

Please let us know if you require any further information.

Best regards,
Settlement Operations
```