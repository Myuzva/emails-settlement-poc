# MAIA Settlement Mailbox Report - email_178.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Provide confirmation slip.
**Reason:** The email requests the final confirmation slip for trade QL61776377, and the trade was successfully found in HOST with matching details.

---

## 2. Email Summary

**Email ID:** email_178  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Citigroup

Sender requests confirmation slip for closed trade QL61776377.

---

## 3. Classification
- **Primary Type:** missing_confirmation
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | null | QL61776377 | missing_in_email | none |
| security_isin | null | DE0007664005 | missing_in_email | none |
| security_name | Volkswagen AG | DE0007664005 | match | none |
| settlement_date | 2026-03-06 | 2026-03-06 | match | none |
| trade_date | 2026-03-05 | 2026-03-05 | match | none |
| quantity | 82336 | 82336 | match | none |
| amount | 1764179.85 | 1764179.85 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty_name | Citigroup | E57ODZWZ7FF32TWEFA76 | match | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade QL61776377 matches the email facts (closed, sell, 82,336 @ EUR 1,764,179.85, settlement 2026-03-06).
- [ ] Provide the requested final confirmation slip / trade advice to the counterparty.

---

## 7. Draft Analyst Response Template
```text
Dear Citigroup Settlement Team,

Thank you for your email. 

We can confirm that trade QL61776377 (Sell 82,336 shares of Volkswagen AG) is marked as Closed in our system and all details match perfectly (Net Amount: EUR 1,764,179.85). Please find attached the requested final confirmation slip for this trade.

Best regards,
Settlement Operations
```