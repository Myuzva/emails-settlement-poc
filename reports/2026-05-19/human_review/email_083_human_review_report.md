# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Route to human review.

**Reason:** The discrepancy claim states Merrill Lynch appears in the counterparty confirmation/attachment broker detail, but reconciliation against primary email facts and HOST shows BNP Paribas; this unresolved evidence conflict requires human review.

---

## 2. Email Summary

**Email ID:** email_083  
**Subject:** Unmatched Trade – Roche Holding AG – JF61444313  
**Sender:** Thomas Müller <t.mueller@rheinasset.de>  
**Received:** 2026-04-28 13:38 UTC  
**Counterparty:** BNP Paribas / Merrill Lynch

The sender reports a counterparty mismatch for trade JF61444313, stating it is booked against BNP Paribas while the counterparty confirmation and attachment reference Merrill Lynch.

---

## 3. Classification
- **Primary Type:** counterparty_mismatch
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | JF61444313 | JF61444313 | match | none |
| security_isin | null | CH0012032048 | missing_in_email | none |
| security_name | Roche Holding AG | null | missing_in_host | low |
| settlement_date | 2026-03-19 | 2026-03-19 | match | none |
| trade_date | 2026-03-18 | 2026-03-18 | match | none |
| quantity | 35819 | 35819 | match | none |
| amount | 1276309.39 | 1276309.39 | match | none |
| currency | CHF | CHF | match | none |
| side | sell | Verkauf | match | none |
| counterparty_name | BNP Paribas | BNP Paribas | match | none |
| counterparty_lei | null | R0MUWSFPU8MPRO8K5P83 | missing_in_email | low |
| status | unknown | Offen | missing_in_email | none |

### Discrepancy Flags
- counterparty_confirmation_claim_differs_from_host_and_email_facts
- security_name_vs_host_identifier_not_enriched
- initial_trades_lookup_422_retry_serialization_issue

---

## 6. Findings

The trade was found in HOST and matches the primary email facts (BNP Paribas). However, the email evidence explicitly claims a counterparty confirmation/broker value of Merrill Lynch, which is not the HOST counterparty and is not represented as the primary email fact.

---

## 7. Next Steps

1. Review the attached trade details (trade_details.pdf) to verify the broker/counterparty information.

2. Confirm the correct counterparty for trade JF61444313 in internal systems.

3. Contact the sender to clarify the counterparty mismatch and confirm the correct booking details.

4. Keep the case under analyst review until the discrepancy is resolved.

---