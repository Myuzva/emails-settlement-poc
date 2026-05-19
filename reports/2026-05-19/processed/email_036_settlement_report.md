# MAIA Settlement Mailbox Report - email_036.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Standard  
**Recommended Action:** Proceed with standard documentation retrieval/response workflow. HOST trade matches the email facts; provide or request the archival settlement confirmation/trade advice for trade UH78032934 according to internal process.
**Reason:** Email explicitly requests archival settlement confirmation or trade advice for a named trade reference.

---

## 2. Email Summary

**Email ID:** email_036  
**Subject:** Clarification Required: Trade UH78032934  
**Sender:** Thomas Müller <t.mueller@rheinasset.de>  
**Received:** 2026-04-28T15:38:47+02:00  
**Counterparty:** Raiffeisen Bank

The sender requests the archival documentation for trade UH78032934, which is recorded as closed in their system.

---

## 3. Classification
- **Primary Type:** documentation_missing (originally instruction_or_document_update)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | UH78032934 | UH78032934 | match | none |
| security_name | UBS Group AG | UBS Group AG | match | none |
| isin | null | CH0244767585 | missing_in_email | none |
| trade_date | 2026-03-04 | 2026-03-04 | match | none |
| settlement_date | 2026-03-05 | 2026-03-05 | match | none |
| side | sell | Sale | match | none |
| quantity | 91177 | 91177 | match | none |
| amount | 235149.90 | 235149.90 | match | none |
| currency | USD | USD | match | none |
| counterparty_name | Raiffeisen Bank | Raiffeisen Bank | match | none |
| status | closed | Closed | match | none |

### Discrepancy Flags
- documentation_missing

---

## 6. Recommended Action
- [x] No reconciliation discrepancy found. Host trade UH78032934 matches the email facts (closed, sell, 91,177 @ USD 235,149.90, settlement 2026-03-05).
- [ ] Provide the requested archival settlement confirmation or trade advice for trade UH78032934.

---

## 7. Draft Analyst Response Template
```text
Dear Thomas Müller,

Thank you for your email regarding trade UH78032934.

We can confirm that the trade (Sell 91,177 shares of UBS Group AG) is recorded as Closed in our system, and all economic details match perfectly (Net Amount: USD 235,149.90, Settlement Date: 2026-03-05). 

As requested, please find attached the archival settlement confirmation/trade advice for your records.

Best regards,
Settlement Operations
```