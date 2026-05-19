# Settlement Analyst Report - email_164.eml

**Date Generated:** 2026-05-19
**Status:** Needs Human Review
**Confidence Score:** 78%
**Email File:** `email_164.eml`

---

## 1. Case Overview
* **Primary Issue:** Security Mismatch
* **Action Required:** Investigate instrument discrepancy (Tesla Inc. vs Amazon.com Inc.)

## 2. Extracted Trade Facts
| Field | Extracted Value | Confidence |
| :--- | :--- | :--- |
| **Trade Reference** | FR58455504 | High (98%) |
| **Counterparty** | Merrill Lynch | High (95%) |
| **Security Name** | Amazon.com Inc. (Sender claims Tesla Inc.) | High (94%) |
| **Trade Date** | 2026-02-27 | High (95%) |
| **Settlement Date** | 2026-03-02 | High (95%) |
| **Quantity** | 28,614 | High (95%) |
| **Amount** | 546,752.05 EUR | High (95%) |
| **Side** | Sell | High (95%) |

## 3. Host System Reconciliation
| Field | Email Value | Host Value | Status | Severity |
| :--- | :--- | :--- | :--- | :--- |
| **Trade Reference** | FR58455504 | FR58455504 | Match | None |
| **Security Name** | Amazon.com Inc. | US88160R1014 (Tesla ISIN) | Mismatch | High |
| **Quantity** | 28,614 | 28,614 | Match | None |
| **Amount** | 546,752.05 | 546,752.05 | Match | None |
| **Currency** | EUR | EUR | Match | None |
| **Side** | Sell | Verkauf | Match | None |
| **Counterparty** | Merrill Lynch | Merrill Lynch (lei: FAK6QKWT97JDDAHS3S03) | Match | None |

## 4. Discrepancy Analysis
* **Security Mismatch:** The email body contains an internal claim that the 'correct' security is Tesla Inc., while the booking reflects Amazon.com Inc. The host trade shows identifier US88160R1014, which appears to represent Tesla. This creates a booking vs. record contradiction that must be resolved by operations.
* **Security Lookup:** A security lookup performed for 'Amazon.com Inc.' returned ISIN US0231351067, which differs from the host security identifier.

## 5. Recommended Action
**Human review required:** Investigate the instrument discrepancy. The host trade shows identifier US88160R1014 (appears to be Tesla), while email facts/booking reference Amazon.com Inc. (ISIN US0231351067). Confirm which instrument is correct for FR58455504 and whether an amendment or re-book is needed. Provide reconciled instrument identifier/name and update booking if required.