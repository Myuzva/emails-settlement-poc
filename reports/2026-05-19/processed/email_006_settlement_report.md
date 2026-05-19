# MAIA Settlement Mailbox Report - email_006.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Send/attach the final confirmation slip or trade advice for BF92476064 to the requester. If the confirmation cannot be located, escalate to operations with the host trade reference and LEI shown above.
**Reason:** Email explicitly requests final confirmation slip, trade advice, or execution confirmation.

---

## 2. Email Summary

**Email ID:** email_006  
**Subject:** Trade Exception – BF92476064  
**Sender:** Elena Rossi <e.rossi@mediobanca.it>  
**Received:** Tue, 28 Apr 2026 15:38:47 +0200  
**Counterparty:** Société Générale

The sender requests the final confirmation slip or trade advice/execution confirmation for a closed trade.

---

## 3. Classification
- **Primary Type:** missing_confirmation (originally confirmation_missing)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | BF92476064 | BF92476064 | match | none |
| security_name | Tesla Inc. | Tesla Inc. | match | none |
| security_isin | null | US88160R1014 | missing_in_email | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| quantity | 11303 | 11303 | match | none |
| amount | 999202.27 | 999202.27 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | low |
| counterparty_name | Société Générale | Société Générale | match | none |
| counterparty_lei | null | O2RNE8IBXP4R0TD8PL25 | missing_in_email | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- missing_confirmation_requested
- security_isin_missing_in_email
- counterparty_lei_missing_in_email

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade BF92476064 matches the email facts (Closed, Sale, 11,303 @ EUR 999,202.27, settlement 2026-03-13).
- [ ] Send/attach the final confirmation slip or trade advice for BF92476064 to the requester.
- [ ] If the confirmation cannot be located, escalate to operations with the host trade reference and LEI shown above.

---

## 7. Draft Analyst Response Template
```text
Dear Elena Rossi,

Thank you for your email. 

Please find attached the final confirmation slip for trade BF92476064 (Sell 11,303 shares of Tesla Inc., Net Amount: EUR 999,202.27). 

If you require any further documentation, please let us know.

Best regards,
Settlement Operations
```