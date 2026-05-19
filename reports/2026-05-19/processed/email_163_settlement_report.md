# MAIA Settlement Mailbox Report - email_163.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Record matches host trade LX63131554. Provide the requester with the final confirmation slip / trade advice or an explicit statement that the trade record matches internal records. Attach confirmation/execution advice as requested.
**Reason:** Sender explicitly requests final confirmation slip for a specific trade reference.

---

## 2. Email Summary

**Email ID:** email_163  
**Subject:** Settlement Query – Novartis AG – 2026-03-10  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Macquarie Group

The sender requests the final confirmation slip, trade advice, or execution confirmation for trade LX63131554.

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
| reference_number | LX63131554 | LX63131554 | match | none |
| security_name | Novartis AG | Novartis AG | match | none |
| isin | null | CH0012221716 | missing_in_email | none |
| settlement_date | 2026-03-10 | 2026-03-10 | match | none |
| trade_date | 2026-03-09 | 2026-03-09 | match | none |
| quantity | 71681 | 71681 | match | none |
| amount | 558977.16 | 558977.16 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | Macquarie Group | Macquarie Group (LEI: KG1ELAF8FBU2GBW60X80) | match | none |
| reported_status | closed | Geschlossen | match | none |

### Discrepancy Flags
- missing_confirmation_requested

---

## 6. Recommended Action
- [x] Record matches host trade LX63131554.
- [x] Provide the requester with the final confirmation slip / trade advice or an explicit statement that the trade record matches internal records.
- [x] Attach confirmation/execution advice as requested.

---

## 7. Draft Analyst Response Template
```text
Dear Anna Kowalski,

Thank you for your email.

We can confirm that trade LX63131554 (Sell 71,681 shares of Novartis AG) matches our internal records perfectly (ISIN CH0012221716, Net Amount: CHF 558,977.16, Value Date: 2026-03-10). 

Please find attached the requested final confirmation slip / trade advice for your records.

Best regards,
Settlement Operations
```