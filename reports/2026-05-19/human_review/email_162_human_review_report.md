# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required: HOST trade was found and economics match, but the security differs materially. Review the sender's claimed instrument mismatch and determine whether re-booking or formal amendment is required.

**Reason:** The sender explicitly states an instrument mismatch for trade ZA30446760, claiming the correct security is ABB Ltd. while the booking reflects Zurich Insurance Group AG. HOST reconciliation confirms a material security mismatch (email security name Zurich Insurance Group AG enriches to ISIN CH0011075394, while HOST trade carries security identifier CH0012530207).

---

## 2. Email Summary

**Email ID:** email_162.eml  
**Subject:** Outstanding Trade – Action Required – ZA30446760  
**Sender:** John Smith <j.smith@globalcapital.com>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Citigroup

The sender reports a retrospective instrument mismatch on trade ZA30446760, which is marked as closed in their system. They state the correct security is ABB Ltd., but the booking reflects Zurich Insurance Group AG.

---

## 3. Classification
- **Primary Type:** security_mismatch (originally security_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | ZA30446760 | ZA30446760 | match | none |
| security_name | Zurich Insurance Group AG | CH0012530207 | mismatch | high |
| isin | null | CH0012530207 | missing_in_email | none |
| trade_date | 2026-03-02 | 2026-03-02 | match | none |
| settlement_date | 2026-03-03 | 2026-03-03 | match | none |
| side | buy | Kauf | match | none |
| quantity | 86001 | 86001 | match | none |
| amount | 1941113.74 | 1941113.74 | match | none |
| currency | CHF | CHF | match | none |
| counterparty_name | Citigroup | E57ODZWZ7FF32TWEFA76 | match | none |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- security_mismatch_confirmed
- host_security_identifier_differs_from_email_security_name
- email_security_name_enrichment_isin_differs_from_host_security_identifier

---

## 6. Findings

HOST returned exactly one trade for reference ZA30446760. Reference number, dates, quantity, amount, currency, side, counterparty, and status reconcile after safe normalization/enrichment.

However, security comparison indicates a material mismatch: email security name Zurich Insurance Group AG maps to CH0011075394, while HOST trade security is CH0012530207. The sender claims the correct security should be ABB Ltd.

---

## 7. Next Steps

1. Review the sender's claimed instrument mismatch (ABB Ltd. vs Zurich Insurance Group AG).
2. Verify the correct security against internal trade booking records for trade ZA30446760.
3. Determine whether re-booking or a formal amendment trade is required.
4. Keep the case under analyst review until the discrepancy is resolved.
