# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** Medium  

**Recommended Action:** Human review recommended before automated closure.

**Reason:** The lead trade was found and core economic fields match, but the email omits currency and the counterparty name could not be reconciled to the HOST counterparty identifier after enrichment lookup.

---

## 2. Email Summary

**Email ID:** email_184  
**Subject:** Trade Confirmation Request – CU42877208 (+ 1 more)  
**Sender:** Sarah Jensen <s.jensen@nordbank.com>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** Nordbank

The sender states documentation is incomplete and requests resubmission of full trade details for processing/pre-settlement checks.

---

## 3. Classification
- **Primary Type:** documentation_missing (originally instruction_or_document_update)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** RF07007889 (Nordbank, UBS Group AG, 1,545,709.32)

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | CU42877208 | CU42877208 | match | none |
| security_isin | null | CH0012221716 | missing_in_email | none |
| security_name | Novartis AG | Novartis AG | match | none |
| settlement_date | 2026-03-26 | 2026-03-26 | match | none |
| trade_date | 2026-03-25 | 2026-03-25 | match | none |
| quantity | 67080 | 67080 | match | none |
| amount | 1370201.89 | 1370201.89 | match | none |
| currency | null | CHF | missing_in_email | medium |
| side | buy | Buy | match | none |
| counterparty_name | Nordbank | 8I5DZWZKVSZI1NUHU748 | unknown | medium |
| status | unknown | Open | missing_in_email | none |

### Discrepancy Flags
- currency_missing_in_email
- counterparty_identifier_unresolved
- email_requests_full_trade_details
- related_trade_not_host_queried

---

## 6. Findings

The primary trade (CU42877208) was found in HOST and core economic fields match. However, the email omits the currency, and the counterparty name (Nordbank) could not be reconciled to the HOST counterparty identifier (8I5DZWZKVSZI1NUHU748) after enrichment lookup. Additionally, the email requests full trade details due to incomplete documentation.

---

## 7. Next Steps

1. Verify the counterparty identifier (8I5DZWZKVSZI1NUHU748) corresponds to Nordbank.
2. Confirm the currency (CHF) for the trade.
3. Provide the requested full trade details to the counterparty for both trades (CU42877208 and RF07007889).
4. Keep the case under analyst review until the documentation request is fulfilled.

---