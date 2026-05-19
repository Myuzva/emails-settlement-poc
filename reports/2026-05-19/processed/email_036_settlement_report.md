# MAIA Settlement Mailbox Report - email_036.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Low  
**Recommended Action:** Provide archival settlement confirmation / trade advice to requester.
**Reason:** Sender requests archival settlement confirmation or trade advice copy for records; no mismatch alleged.

---

## 2. Email Summary

**Email ID:** email_036  
**Subject:** Clarification Required: Trade UH78032934  
**Sender:** Thomas Müller <t.mueller@rheinasset.de>  
**Received:** Tue, 28 Apr 2026 15:38:47 +0200  
**Counterparty:** Raiffeisen Bank

The sender requests archival documentation for trade UH78032934, which is recorded as closed in their system.

---

## 3. Classification
- **Primary Type:** instruction_or_document_update
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | UH78032934 | UH78032934 | match | high |
| security_isin | null | CH0244767585 | missing_in_email | none |
| security_name | UBS Group AG | UBS Group AG | match | none |
| settlement_date | 2026-03-05 | 2026-03-05 | match | none |
| trade_date | 2026-03-04 | 2026-03-04 | match | none |
| quantity | 91177 | 91177 | match | none |
| amount | 235149.9 | 235149.9 | match | none |
| currency | USD | USD | match | none |
| side | sell | Sale | match | low |
| counterparty_name | Raiffeisen Bank | Raiffeisen Bank | match | none |
| counterparty_lei | null | PQOH26KWDF7CG10L6792 | missing_in_email | low |
| reported_status | closed | Closed | match | none |

### Discrepancy Flags
- None

---

## 6. Recommended Action
- [x] Provide archival settlement confirmation / trade advice to requester (attach trade advice PDF or archival record). All material fields match host; no reconciliation discrepancies requiring escalation.

---

## 7. Draft Analyst Response Template
```text
Dear Thomas Müller,

Thank you for your email. 

Please find attached the requested archival settlement confirmation and trade advice for trade UH78032934 (Sale of 91,177 shares of UBS Group AG). Our records confirm that the trade successfully settled on 2026-03-05 and is marked as Closed in our system.

If you need any further documentation, please let us know.

Best regards,
Settlement Operations
```