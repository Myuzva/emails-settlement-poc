# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required to resolve settlement date ambiguity.

**Reason:** Email and attachment indicate settlement date 2026-04-03 while host record shows 2026-03-04 (likely due to ambiguous 03/04/2026 formatting). Confirm intended settlement date with the sender or source systems and update the host record if necessary.

---

## 2. Email Summary

**Email ID:** email_007.eml  
**Subject:** Trade Inquiry – Reference AY31008827 (+ 1 more)  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:47 +0200  
**Counterparty:** Nomura Securities

The sender requests confirmation that pre-settlement checks are complete and timely settlement is on track for an open trade.

---

## 3. Classification
- **Primary Type:** general_status_request (originally settlement_status_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** MM07121551

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | AY31008827 | AY31008827 | match | none |
| security_isin | null | DE0007236101 | missing_in_email | none |
| security_name | Siemens AG | Siemens AG | match | none |
| settlement_date | 2026-04-03 | 2026-03-04 | mismatch | high |
| trade_date | 2026-03-03 | 2026-03-03 | match | none |
| quantity | 54329 | 54329 | match | none |
| amount | 514093.82 | 514093.82 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | Nomura Securities | Nomura Securities (LEI YFSWKL48C7RRQDP89D10) | match | none |
| status | open | Offen | match | none |

### Discrepancy Flags
- settlement_date_mismatch
- ambiguous_date_format
- hitl_required_set

---

## 6. Findings

The trade was found in HOST, but the settlement date differs. The email/attachment normalized to 2026-04-03 while the host shows 2026-03-04. The original source used '03/04/2026' which is ambiguous.

All other fields (reference, quantity, amount, currency, security, counterparty, side, trade date, status) are consistent between email and host after normalization.

---

## 7. Next Steps

1. Confirm the intended settlement date with the sender or source systems.
2. Update the host record if necessary.
3. Keep the case under analyst review until the discrepancy is resolved.

---
