# MAIA Settlement Mailbox Report - email_067.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** High  
**Recommended Action:** Proceed with standard processing.
**Reason:** Settlement-related amount mismatch with a usable trade reference for HOST lookup. Primary trade is clear despite one additional trade record in the attachment.

---

## 2. Email Summary

**Email ID:** email_067  
**Subject:** Pending Settlement – Microsoft Corp. – 2026-03-19 (+ 1 more)  
**Sender:** Michael Hartmann <m.hartmann@eurofin.de>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** HSBC

The sender reports their system notional differs from the counterparty notification and asks to confirm the correct notional before settlement.

---

## 3. Classification
- **Primary Type:** amount_mismatch (originally amount_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** Nestlé S.A. (BNP Paribas, CHF 1,310,952.25)

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | KV78386940 | KV78386940 | match | none |
| security_isin | null | US5949181045 | missing_in_email | none |
| security_name | Microsoft Corp. | Microsoft Corp. | match | none |
| settlement_date | 2026-03-19 | 2026-03-19 | match | none |
| trade_date | 2026-03-18 | 2026-03-18 | match | none |
| quantity | 49789 | 49789 | match | none |
| amount | 588790.65 | 588790.65 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | HSBC | HSBC | match | none |
| counterparty_lei | null | MP6I5ZYZBEU3UXPYFY54 | missing_in_email | none |
| status | pending | Offen | match | none |

### Discrepancy Flags
- counterparty_notification_amount_394329.00_differs_from_host_amount_588790.65
- primary_trade_matched_by_reference_number
- related_trade_present_not_looked_up

---

## 6. Recommended Action
- [x] Proceed with standard processing. HOST trade KV78386940 matches the structured primary email facts, including amount 588790.65 CHF, quantity, dates, currency, side, security after enrichment, and counterparty after enrichment.
- [ ] If responding to the sender, state that HOST records show 588790.65 CHF for the primary trade; the separate counterparty notification amount of 394329.00 CHF remains external to HOST reconciliation.

---

## 7. Draft Analyst Response Template
```text
Dear Michael Hartmann,

Thank you for your email regarding the pending settlement for Microsoft Corp. (Trade KV78386940).

We have reviewed the details in our system. We can confirm that our HOST records show the correct notional amount as 588,790.65 CHF for the sale of 49,789 shares, which matches the figure in your system. The counterparty notification amount of 394,329.00 CHF appears to be incorrect or external to our reconciliation.

Please let us know if you need any further assistance to proceed with the settlement on 2026-03-19.

Best regards,
Settlement Operations
```