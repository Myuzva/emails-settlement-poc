# Settlement Discrepancy Report: Needs Human Review

## Case Metadata
- **Date Generated:** 2026-05-19
- **Email File:** email_168.eml
- **Trade Reference:** BR57017960
- **Case Type:** security_mismatch
- **Confidence Score:** 84%
- **Status:** Needs Human Review

## Executive Summary
The system successfully matched trade BR57017960 in the HOST system. However, a significant security mismatch was identified. The email states the security is "Deutsche Bank AG" but claims it should be "Novartis AG". The HOST system shows the security as "CH0012221716" (Novartis AG). Additionally, there is a status difference (Email: settled vs HOST: Closed).

## Discrepancy Analysis

| Field | Email Value | HOST Value | Status | Severity |
| :--- | :--- | :--- | :--- | :--- |
| **Security Name** | Deutsche Bank AG | Novartis AG | 🔴 Mismatch | High |
| **Status** | settled | Closed | 🟡 Mismatch | Medium |
| **Security ISIN** | *Missing* | CH0012221716 | ⚪ Missing in Email | None |
| **Counterparty LEI** | *Missing* | O2RNE8IBXP4R0TD8PL25 | ⚪ Missing in Email | None |

*Note: All other economic fields (Quantity, Amount, Currency, Trade Date, Settlement Date, Side, Counterparty Name) matched successfully.*

## Host System Data
**Selected Trade Details:**
- **Reference Number:** BR57017960
- **Buy Sale:** Sale
- **Settlement Date:** 2026-03-03
- **Transaction Date:** 2026-03-02
- **Security:** CH0012221716
- **Security Name:** Novartis AG
- **Status:** Closed
- **Amount:** 1922030.11
- **Currency:** USD
- **Quantity:** 78711
- **Counterparty:** O2RNE8IBXP4R0TD8PL25
- **Counterparty Name:** Société Générale

## Evidence Extracted
- **Subject:** "Unmatched Trade – Deutsche Bank AG – BR57017960" (Confidence: 92%)
- **Body:** "trade BR57017960 has revealed that the security booked does not correspond to our agreed terms" (Confidence: 96%)
- **Body:** "The trade appears to reference Deutsche Bank AG, whereas our records indicate it should have been booked against Novartis AG." (Confidence: 96%)
- **Attachment (trade_details.pdf):** "BR57017960; Deutsche Bank AG; USD; 2026-03-03; 78711; Société Générale; 2026-03-02; Sale; 1922030.11" (Confidence: 94%)

## Recommended Actions
1. **Verify Security Mismatch:** Human analyst needs to verify the security mismatch. The HOST system reflects the requested/correct value (Novartis AG) rather than the extracted booked value (Deutsche Bank AG).
2. **Confirm Status Equivalence:** Verify whether HOST status "Closed" is operationally equivalent to reported "settled".
