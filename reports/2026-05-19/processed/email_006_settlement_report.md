# MAIA Settlement Mailbox Report - email_006.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Proceed with standard processing to obtain or provide the requested final confirmation slip/trade advice for matched closed trade BF92476064. No human review is required based on HOST reconciliation.
**Reason:** Settlement/trade-related document request with clear trade reference BF92476064.

---

## 2. Email Summary

**Email ID:** email_006  
**Subject:** Trade Exception – BF92476064  
**Sender:** Elena Rossi <e.rossi@mediobanca.it>  
**Received:** Tue, 28 Apr 2026 15:38:47 +0200  
**Counterparty:** Société Générale

The sender explicitly requests the final confirmation slip/trade advice/execution confirmation for the closed trade BF92476064.

---

## 3. Classification
- **Primary Type:** confirmation_missing (originally confirmation_missing)
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
| trade_date | 2026-03-12 | 2026-03-12 | match | none |
| settlement_date | 2026-03-13 | 2026-03-13 | match | none |
| side | sell | Sale | match | none |
| quantity | 11303 | 11303 | match | none |
| amount | 999202.27 | 999202.27 | match | none |
| currency | EUR | EUR | match | none |
| counterparty_name | Société Générale | Société Générale | match | none |
| counterparty_lei | null | O2RNE8IBXP4R0TD8PL25 | missing_in_email | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- confirmation_missing_requested

---

## 6. Recommended Action
- [x] Proceed with standard processing to obtain or provide the requested final confirmation slip/trade advice for matched closed trade BF92476064. No human review is required based on HOST reconciliation.
- [ ] Provide the final confirmation slip/trade advice to the sender.

---

## 7. Draft Analyst Response Template
```text
Dear Elena Rossi,

Thank you for your email regarding trade BF92476064.

Please find attached the requested final confirmation slip/trade advice for the closed trade (Sell 11,303 shares of Tesla Inc.). All details match our records perfectly.

Best regards,
Settlement Operations
```