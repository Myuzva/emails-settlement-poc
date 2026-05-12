# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Investigate security mismatch and route to analyst review.

**Reason:** The sender explicitly states a retrospective instrument mismatch, noting their records show ABB Ltd. while the booking reflects Zurich Insurance Group AG. Human review is required to verify if the sender's view is outdated or if there is a display issue.

---

## 2. Email Summary

**Email ID:** email_162.eml  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Citigroup

The sender reports an instrument mismatch for trade ZA30446760, claiming their records show ABB Ltd. but the booking reflects Zurich Insurance Group AG.

---

## 3. Classification
- **Primary Type:** wrong_security (originally security_mismatch)
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
| security_isin | null | CH0012530207 | missing_in_email | none |
| security_name | Zurich Insurance Group AG | ABB Ltd. | mismatch | high |
| settlement_date | 2026-03-03 | 2026-03-03 | match | none |
| trade_date | 2026-03-02 | 2026-03-02 | match | none |
| quantity | 86001 | 86001 | match | none |
| amount | 1941113.74 | 1941113.74 | match | none |
| currency | CHF | CHF | match | none |
| side | buy | buy | match | none |
| counterparty_name | Citigroup | Citigroup | match | none |
| status | closed | closed | match | none |

### Discrepancy Flags
- security_name_mismatch

---

## 6. Findings

The trade was found in HOST. The HOST record already shows 'ABB Ltd.', which matches the sender's requested value, but the sender claims the booking reflects 'Zurich Insurance Group AG'. All other trade parameters match exactly.

The likely cause of the issue is a display issue or the sender's view being outdated. The case should be reviewed before any confirmation is sent externally.

---

## 7. Next Steps

1. Verify the correct security against internal trade booking records.

2. Confirm whether the counterparty is referencing the same trade reference and if their view is outdated.

3. Ask the counterparty to confirm the expected security.

4. Keep the case under analyst review until the discrepancy is resolved.

---