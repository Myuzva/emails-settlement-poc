# MAIA Settlement Mailbox Report - email_006.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Proceed with providing the requested confirmation as the trade details match the host system.
**Reason:** Email explicitly requests final confirmation slip/trade advice/execution confirmation for a single identified trade. Trade reference and supporting trade details are present in the email body.

---

## 2. Email Summary

**Email ID:** email_006  
**Subject:** Trade Exception – BF92476064  
**Sender:** Unknown  
**Received:** Unknown  
**Counterparty:** Société Générale

The sender requests the final confirmation slip, trade advice, or execution confirmation for a closed trade.

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
| security_name | Tesla Inc. | US88160R1014 | match | none |
| isin | null | US88160R1014 | missing_in_email | none |
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| side | sell | Sale | match | none |
| quantity | 11303 | 11303 | match | none |
| amount | 999202.27 | 999202.27 | match | none |
| currency | EUR | EUR | match | none |
| counterparty_name | Société Générale | O2RNE8IBXP4R0TD8PL25 | match | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade BF92476064 matches the email facts (Closed, Sale, 11,303 @ EUR 999,202.27, settlement 2026-03-13).
- [ ] Respond to requester providing the requested final confirmation slip / trade advice / execution confirmation.

---

## 7. Draft Analyst Response Template
```text
Dear Société Générale Settlement Team,

Thank you for your email. 

Please find attached the requested final confirmation slip / execution confirmation for trade BF92476064 (Sale 11,303 shares of Tesla Inc.). The trade is marked as Closed in our system and all details match perfectly (Net Amount: EUR 999,202.27, Settlement Date: 2026-03-13).

Best regards,
Settlement Operations
```