# MAIA Settlement Mailbox Report - email_006.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** The trade details match the HOST system. Proceed with providing the requested confirmation slip.
**Reason:** Email explicitly requests final confirmation slip/trade advice/execution confirmation for a specific trade reference. Single trade table provides sufficient HOST lookup data.

---

## 2. Email Summary

**Email ID:** email_006.eml  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Société Générale

Sender requests the final confirmation slip, trade advice, or execution confirmation for a closed trade.

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
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| side | sell | Sale | match | none |
| quantity | 11303 | 11303 | match | none |
| amount | 999202.27 | 999202.27 | match | none |
| currency | EUR | EUR | match | none |
| security_name | Tesla Inc. | Tesla Inc. | match | none |
| isin | null | US88160R1014 | missing_in_email | none |
| counterparty_name | Société Générale | Société Générale | match | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade BF92476064 matches the email facts perfectly.
- [ ] Respond to requester providing the requested final confirmation slip / trade advice.

---

## 7. Draft Analyst Response Template
```text
Dear Société Générale Settlement Team,

Thank you for your email. 

Please find attached the final confirmation slip for trade BF92476064 (Sale of 11,303 shares of Tesla Inc., Net Amount: EUR 999,202.27, Settlement Date: 2026-03-13). 

Our records indicate that this trade is successfully closed. Let us know if you need any further assistance.

Best regards,
Settlement Operations
```