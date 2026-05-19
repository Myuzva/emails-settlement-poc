# MAIA Settlement Analyst Report - HITL Required

**Date Generated:** 2026-05-19
**Email File:** email_162.eml
**Primary Reference:** ZA30446760
**Status:** Needs Human Review
**Confidence Score:** 0.45

## Case Summary
The sender reported a retrospective instrument mismatch on trade ZA30446760. The sender claims the correct security should be ABB Ltd., while the booking reflects Zurich Insurance Group AG. Host reconciliation revealed further ambiguity, as the host trade's Security field contains an identifier (CH0012530207) that does not match the Zurich ISIN (CH0011075394).

## Extracted Trade Facts
- **Trade Reference:** ZA30446760
- **Trade Date:** 2026-03-02
- **Settlement Date:** 2026-03-03
- **Side:** buy
- **Quantity:** 86001
- **Amount:** 1941113.74
- **Currency:** CHF
- **Counterparty:** Citigroup
- **Security Name (Email):** Zurich Insurance Group AG

## Host Reconciliation Status
**Status:** matched (with material discrepancies)

| Field | Email Value | Host Value | Match Status |
|-------|-------------|------------|--------------|
| Reference Number | ZA30446760 | ZA30446760 | match |
| Security | Zurich Insurance Group AG | CH0012530207 | mismatch |
| Settlement Date | 2026-03-03 | 2026-03-03 | match |
| Trade Date | 2026-03-02 | 2026-03-02 | match |
| Side | buy | Kauf | match |
| Quantity | 86001 | 86001 | match |
| Amount | 1941113.74 | 1941113.74 | match |
| Currency | CHF | CHF | match |
| Counterparty | Citigroup | Citigroup | match |

## Discrepancies & Evidence
- **Security Mismatch:** Sender reports the correct security should be ABB Ltd., while the booking/trade table reflects Zurich Insurance Group AG, and asks whether re-booking or amendment is required.
  - *Evidence:* "correct security as ABB Ltd., however the booking reflects Zurich Insurance Group AG"

## Analyst Recommendation
Human review required. Investigate the host trade security identifier CH0012530207 (host record) and determine which instrument it refers to. Confirm whether the booked instrument is Zurich Insurance Group AG (ISIN CH0011075394) or ABB Ltd., per sender claim. If sender is correct, perform re-booking or formal amendment. Include counterparty/LEI E57ODZWZ7FF32TWEFA76 in the investigation and retain evidence from the sender before amendment.