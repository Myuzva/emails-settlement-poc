# MAIA Settlement Mailbox Report - email_117.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Reply to sender confirming host shows trade WR98673171 as Open (not yet settled) for Microsoft (host ISIN US5949181045) with no differences in amount/quantity/currency. Ask sender if they have any additional settlement instructions or see a different status; if they need escalation, forward to operations with host trade details and LEI.
**Reason:** Sender asks to follow up on a trade as part of settlement monitoring. Request asks whether any action is required to ensure timely settlement.

---

## 2. Email Summary

**Email ID:** email_117.eml  
**Subject:** Trade Inquiry – Reference WR98673171 (+ 1 more)  
**Sender:** Claire Dubois <c.dubois@paribas-ops.fr>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Credit Suisse

The sender requests settlement follow-up and asks whether any action is required for timely settlement.

---

## 3. Classification
- **Primary Type:** settlement_status_request
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** CA48963877 (Morgan Stanley, Tesla Inc., EUR 113681.42)

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | WR98673171 | WR98673171 | match | none |
| security_isin | null | US5949181045 | missing_in_email | none |
| security_name | Microsoft Corp. | null | missing_in_host | low |
| settlement_date | 2026-03-24 | 2026-03-24 | match | none |
| trade_date | 2026-03-23 | 2026-03-23 | match | none |
| quantity | 88764 | 88764 | match | none |
| amount | 193956.88 | 193956.88 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty_name | Credit Suisse | Credit Suisse | match | none |
| status | unknown | Open | missing_in_email | medium |

### Discrepancy Flags
- status_mismatch
- security_isin_present_in_host_only
- counterparty_resolved_via_lei

---

## 6. Recommended Action
- [x] Reply to sender confirming host shows trade WR98673171 as Open (not yet settled) for Microsoft (host ISIN US5949181045) with no differences in amount/quantity/currency.
- [x] Ask sender if they have any additional settlement instructions or see a different status.
- [x] If they need escalation, forward to operations with host trade details and LEI.

---

## 7. Draft Analyst Response Template
```text
Dear Claire Dubois,

Thank you for your inquiry regarding trade WR98673171.

We can confirm that the trade (Sell 88,764 shares of Microsoft Corp., ISIN US5949181045) is currently marked as Open in our system. All trade details match perfectly (Net Amount: EUR 193,956.88, Settlement Date: 2026-03-24). 

Please let us know if you require any specific action on our end or if you see a different status in your system. Regarding the related trade CA48963877, please let us know if you require a status update on that as well.

Best regards,
Settlement Operations
```