# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required. The trade FA51193163 was found and trade details match, but the host counterparty is represented by an identifier (3TK20IVIUJ8J3ZU0QE75) that could not be resolved. The sender requests changing the counterparty to ING Bank.

**Reason:** Host counterparty is an unresolved identifier (3TK20IVIUJ8J3ZU0QE75). The sender requests changing the counterparty to ING Bank on a closed/settled trade, which requires operational/legal action and cannot be auto-resolved.

---

## 2. Email Summary

**Email ID:** email_057.eml  
**Subject:** Outstanding Trade – Action Required – FA51193163  
**Sender:** James O'Brien <j.obrien@meridianfunds.co.uk>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** JP Morgan (expected ING Bank)

The sender reports a retrospective counterparty error on trade FA51193163, which is currently marked as settled and closed. The booking reflects JP Morgan as the counterparty, but their agreement confirms it should be ING Bank.

---

## 3. Classification
- **Primary Type:** wrong_counterparty (originally counterparty_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | FA51193163 | FA51193163 | match | none |
| security_isin | null | US46625H1005 | missing_in_email | none |
| security_name | JPMorgan Chase & Co. | null | missing_in_host | low |
| settlement_date | 2026-03-27 | 2026-03-27 | match | none |
| trade_date | 2026-03-26 | 2026-03-26 | match | none |
| quantity | 55538 | 55538 | match | none |
| amount | 1306885.78 | 1306885.78 | match | none |
| currency | USD | USD | match | none |
| side | sell | Sale | match | none |
| counterparty_name | JP Morgan | 3TK20IVIUJ8J3ZU0QE75 | mismatch | high |
| status | settled | Closed | match | low |

### Discrepancy Flags
- counterparty_mismatch
- counterparty_host_id_unresolved
- security_identified_by_isin_only_in_host

---

## 6. Findings

The trade FA51193163 was found in HOST and trade details (dates, quantity, amount, currency, side) match the email. However, the host counterparty is represented by an identifier (3TK20IVIUJ8J3ZU0QE75) that could not be resolved to a name via /counterparty lookup (404). The sender requests changing the counterparty to ING Bank on a closed/settled trade.

---

## 7. Next Steps

1. Manually resolve the host counterparty id (3TK20IVIUJ8J3ZU0QE75) in internal systems or reconcile against LEI records.
2. Verify whether the booked counterparty is JP Morgan (LEI 8I5DZWZKVSZI1NUHU748) or another entity.
3. If host booking is incorrect, escalate to trade support/legal to reopen or correct a closed/settled trade and follow internal remediation process.
4. Include sender evidence and host trade extract in the ticket.

---