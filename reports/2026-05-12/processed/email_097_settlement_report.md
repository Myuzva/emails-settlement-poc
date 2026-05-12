# MAIA Settlement Mailbox Report - email_097.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** The trade details match the HOST records. Provide the missing ISIN (CH0012221716) and Counterparty (Goldman Sachs) to the client as requested.  
**Reason:** The sender states that the trade record is incomplete in their system and requests the missing details to reconcile and archive.

---

## 2. Email Summary

**Email ID:** email_097  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Goldman Sachs

The sender states that the trade record is incomplete in their system and requests the missing details to reconcile and archive.

---

## 3. Classification
- **Primary Type:** missing_details (originally generic_trade_details_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** KY05031605

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | QZ85525941 | QZ85525941 | match | none |
| security_isin | null | CH0012221716 | missing_in_email | none |
| security_name | Novartis AG | Novartis AG | match | none |
| settlement_date | 2026-03-30 | 2026-03-30 | match | none |
| trade_date | 2026-03-27 | 2026-03-27 | match | none |
| quantity | 45458 | 45458 | match | none |
| amount | 1141321.88 | 1141321.88 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | sell | match | none |
| counterparty_name | null | Goldman Sachs | missing_in_email | none |
| status | closed | closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade QZ85525941 matches the email facts (closed, sell, 45,458 @ EUR 1,141,321.88, settlement 2026-03-30).
- [ ] Provide the missing ISIN (CH0012221716) and Counterparty (Goldman Sachs) to the client as requested.
- [ ] Optionally, perform a host lookup for related trade KY05031605 if the requester requires its status.

---

## 7. Draft Analyst Response Template
```text
Dear Client,

Thank you for your email.

We can confirm that trade QZ85525941 (Sell 45,458 shares of Novartis AG) is currently marked as closed in our system and all details match perfectly (Net Amount: EUR 1,141,321.88). 

As requested, here are the missing details for your records:
- ISIN: CH0012221716
- Counterparty: Goldman Sachs

Regarding the related trade KY05031605 mentioned in the attachment, please let us know if you require any details on that as well.

Best regards,
Settlement Operations
```