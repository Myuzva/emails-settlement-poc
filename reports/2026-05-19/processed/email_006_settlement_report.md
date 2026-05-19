# MAIA Settlement Mailbox Report - email_006.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** The trade details in the email match the HOST system exactly. Proceed with generating and sending the requested confirmation slip/trade advice to Société Générale.
**Reason:** The sender explicitly requests the final confirmation slip and trade advice for a specific trade.

---

## 2. Email Summary

**Email ID:** email_006  
**Subject:** Not provided  
**Sender:** Not provided  
**Received:** Not provided  
**Counterparty:** Société Générale

The counterparty is requesting the final confirmation slip and trade advice for closed trade BF92476064.

---

## 3. Classification
- **Primary Type:** confirmation_missing
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
| isin | null | US88160R1014 | missing_in_email | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| quantity | 11303 | 11303 | match | none |
| amount | 999202.27 | 999202.27 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty_name | Société Générale | Société Générale | match | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade BF92476064 matches the email facts (closed, sell, 11,303 @ EUR 999,202.27, settlement 2026-03-13).
- [ ] Respond to requester with the final confirmation slip / trade advice.

---

## 7. Draft Analyst Response Template
```text
Dear Société Générale Settlement Team,

Thank you for your email.

As requested, please find attached the final confirmation slip and trade advice for trade BF92476064 (Sell 11,303 shares of Tesla Inc.). We confirm that the trade is marked as Closed in our system and all details match perfectly (Net Amount: EUR 999,202.27).

Best regards,
Settlement Operations
```