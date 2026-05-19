# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Human review required to confirm counterparty mapping.

**Reason:** Verify whether host counterparty identifier 9R7GPTSO7KV3UQJZQ078 corresponds to 'Morgan Stanley'. Otherwise, trade details match host and settlement status is Open; no operational settlement action recommended until counterparty identity is confirmed.

---

## 2. Email Summary

**Email ID:** email_176.eml  
**Subject:** Reconciliation Query – ME19312140 – Roche Holding AG  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Morgan Stanley

The sender explicitly asks to follow up on settlement monitoring for a single trade and whether any action is required to ensure smooth and timely settlement.

---

## 3. Classification
- **Primary Type:** settlement_status_request (originally settlement_status_request)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | ME19312140 | ME19312140 | match | none |
| security_name | Roche Holding AG | Roche Holding AG (resolved to ISIN CH0012032048) | match | none |
| isin | null | CH0012032048 | missing_in_email | none |
| settlement_date | 2026-03-17 | 2026-03-17 | match | none |
| trade_date | 2026-03-16 | 2026-03-16 | match | none |
| quantity | 88389 | 88389 | match | none |
| amount | 1212017.91 | 1212017.91 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Sale | match | none |
| counterparty | Morgan Stanley | 9R7GPTSO7KV3UQJZQ078 | mismatch | high |
| status | unknown | Open | missing_in_email | none |

### Discrepancy Flags
- counterparty_identifier_only
- counterparty_unverified
- security_enriched_with_isin

---

## 6. Findings

The trade was found in HOST and all trade details (reference, dates, amounts, quantity, side, currency) match perfectly. The security name was successfully resolved to ISIN CH0012032048. However, the HOST counterparty is returned as an identifier (9R7GPTSO7KV3UQJZQ078) rather than a human-readable name, and it has not been verified against the email's counterparty ("Morgan Stanley").

---

## 7. Next Steps

1. Perform a counterparty lookup or check internal mapping to verify if identifier 9R7GPTSO7KV3UQJZQ078 corresponds to Morgan Stanley.
2. If the counterparty matches, confirm to the sender that the trade is Open and on track for settlement.
3. If the counterparty does not match, investigate the booking discrepancy before taking any settlement action.
4. Keep the case under analyst review until the counterparty identity is confirmed.
