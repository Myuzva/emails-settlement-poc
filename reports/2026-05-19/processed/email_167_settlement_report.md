# MAIA Settlement Mailbox Report - email_167.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Respond to sender confirming the trade details and providing the requested documentation.
**Reason:** Sender requests missing information/complete trade details for a closed/settled trade.

---

## 2. Email Summary

**Email ID:** email_167  
**Subject:** Trade Status Update Request – HJ10386713  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** UniCredit

The sender states the closed trade has incomplete documentation and requests missing information/complete trade details.

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
| reference_number | HJ10386713 | HJ10386713 | match | none |
| security_identifier | null | US67066G1040 | missing_in_email | none |
| security_name | null | null | unknown | none |
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| side | sell | Sale | match | none |
| quantity | 72417 | 72417 | match | none |
| amount | 1650395.89 | 1650395.89 | match | none |
| currency | null | USD | missing_in_email | none |
| counterparty | UniCredit | UniCredit (LEI: F1T87K3OQ2OV1UORLH26) | match | low |
| status | closed | Closed | match | none |

### Discrepancy Flags
- documentation_missing_claim
- security_missing_in_email
- currency_missing_in_email

---

## 6. Recommended Action
- [x] Host trade matches the email reference and key economics (quantity, amount, dates, side). Counterparty name resolved to host LEI.
- [ ] Respond to sender confirming the trade details and providing the requested documentation; attach or indicate location of supporting documents.
- [ ] If sender requires security identifier/type clarification, provide host security identifier (US67066G1040) and indicate that no security name was provided in the email.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email regarding trade HJ10386713.

We can confirm that the trade details in our system match your records (Sale of 72,417 units, Amount: USD 1,650,395.89, Trade Date: 2026-03-12, Settlement Date: 2026-03-13). The security identifier for this trade is US67066G1040.

Regarding your request for complete trade details and missing documentation, please find the requested information attached/below.

Best regards,
Settlement Operations
```