# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Route to analyst review.

**Reason:** Human review is required due to an unsupported schema and a security mismatch. The sender claims the correct security is ABB Ltd., but the booking reflects Zurich Insurance Group AG.

---

## 2. Email Summary

**Email ID:** email_162.eml  
**Subject:** N/A  
**Sender:** N/A  
**Received:** N/A  
**Counterparty:** Citigroup

The email reports a retrospective instrument mismatch on trade ZA30446760. Our records show the correct security as ABB Ltd., however the booking reflects Zurich Insurance Group AG.

---

## 3. Classification
- **Primary Type:** wrong_security (originally security_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** ZA30446760 (Citigroup, Zurich Insurance Group AG, CHF 1941113.74)

---

## 5. HOST Lookup Comparison

*Note: HOST lookup was not performed for this case.*

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | ZA30446760 | N/A | N/A | N/A |
| security_isin | null | N/A | N/A | N/A |
| security_name | Zurich Insurance Group AG | N/A | N/A | N/A |
| settlement_date | 2026-03-03 | N/A | N/A | N/A |
| trade_date | 2026-03-02 | N/A | N/A | N/A |
| quantity | 86001 | N/A | N/A | N/A |
| amount | 1941113.74 | N/A | N/A | N/A |
| currency | CHF | N/A | N/A | N/A |
| side | buy | N/A | N/A | N/A |
| counterparty_name | Citigroup | N/A | N/A | N/A |
| status | closed | N/A | N/A | N/A |

### Discrepancy Flags
- **security_mismatch**: Sender claims correct security is ABB Ltd., but booking reflects Zurich Insurance Group AG.

---

## 6. Findings

The email indicates a security mismatch for trade ZA30446760. The sender claims the correct security is ABB Ltd., while the booking reflects Zurich Insurance Group AG. The case requires human review due to an unsupported schema.

---

## 7. Next Steps

1. Review the trade booking for ZA30446760 to verify the correct security.
2. Confirm with the counterparty whether the intended security was ABB Ltd. or Zurich Insurance Group AG.
3. Amend the trade booking if necessary to reflect the correct security.
4. Keep the case under analyst review until the discrepancy is resolved.

---