# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Human review required to confirm whether the email counterparty name HSBC corresponds to HOST counterparty identifier MP6I5ZYZBEU3UXPYFY54.

**Reason:** Counterparty identifier type unresolved. Email provides a name (HSBC) while HOST provides an identifier (MP6I5ZYZBEU3UXPYFY54).

---

## 2. Email Summary

**Email ID:** email_045  
**Subject:** Unmatched Trade – Roche Holding AG – WB07398077  
**Sender:** James O'Brien <j.obrien@meridianfunds.co.uk>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** HSBC

Sender requests confirmation that internal pre-settlement checks are complete and timely settlement is on track for an open trade.

---

## 3. Classification
- **Primary Type:** settlement_status_request
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | WB07398077 | WB07398077 | match | none |
| security_isin | null | CH0012032048 | missing_in_email | none |
| security_name | Roche Holding AG | Roche Holding AG | match | none |
| settlement_date | 2026-03-19 | 2026-03-19 | match | none |
| trade_date | 2026-03-18 | 2026-03-18 | match | none |
| quantity | 98649 | 98649 | match | none |
| amount | 1242006.89 | 1242006.89 | match | none |
| currency | USD | USD | match | none |
| side | sell | Sale | match | none |
| counterparty_name | HSBC | MP6I5ZYZBEU3UXPYFY54 | unknown | medium |
| status | open | Open | match | none |

### Discrepancy Flags
- counterparty_identifier_type_unresolved

---

## 6. Findings

The trade was found in HOST and all primary trade economics and dates match. However, the counterparty could not be safely reconciled because the email provides a name (HSBC) while HOST provides an identifier (MP6I5ZYZBEU3UXPYFY54).

---

## 7. Next Steps

1. Verify if the HOST counterparty identifier MP6I5ZYZBEU3UXPYFY54 corresponds to HSBC.

2. Confirm internal pre-settlement checks are complete.

3. Respond to the counterparty confirming settlement readiness once the counterparty identity is verified.

---