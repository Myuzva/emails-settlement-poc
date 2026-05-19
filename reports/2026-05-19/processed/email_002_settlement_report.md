# MAIA Settlement Mailbox Report - email_002.eml

## 1. Decision

**Settlement Inquiry:** Yes  
**Priority:** Medium  
**Recommended Action:** Respond to sender with the confirmed trade details from host.
**Reason:** Email asks to supply missing details for a specific trade record.

---

## 2. Email Summary

**Email ID:** email_002  
**Subject:** Outstanding Trade – Action Required – XJ02184853  
**Sender:** John Smith <j.smith@globalcapital.com>  
**Received:** Tue, 28 Apr 2026 15:38:47 +0200  
**Counterparty:** Unknown (HOST ID: 5UMCZOEYKCVFAW8ZLO05)

The sender states the trade record is incomplete and requests missing details for reconciliation and archiving.

---

## 3. Classification
- **Primary Type:** generic_trade_details_request
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | XJ02184853 | XJ02184853 | match | none |
| security_name | UBS Group AG | UBS Group AG | match | none |
| isin | null | CH0244767585 | missing_in_email | none |
| settlement_date | null | 2026-03-20 | missing_in_email | none |
| trade_date | null | 2026-03-19 | missing_in_email | none |
| quantity | 29837 | 29837 | match | none |
| amount | 1666712.84 | 1666712.84 | match | none |
| currency | EUR | EUR | match | none |
| side | sell | Verkauf | match | none |
| counterparty | null | 5UMCZOEYKCVFAW8ZLO05 | missing_in_email | none |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- missing_in_email:isin
- missing_in_email:settlement_date
- missing_in_email:trade_date
- missing_in_email:counterparty

---

## 6. Recommended Action
- [x] Respond to sender with the confirmed trade details from host: ISIN CH0244767585 (UBS Group AG), trade date 2026-03-19, settlement date 2026-03-20, quantity 29,837, amount EUR 1,666,712.84, side SELL. 
- [x] Note that the host counterparty is recorded as identifier 5UMCZOEYKCVFAW8ZLO05 — confirm the legal counterparty name if required for archiving. 
- [x] Close the documentation gap once confirmation received.

---

## 7. Draft Analyst Response Template
```text
Dear John Smith,

Thank you for your email regarding trade XJ02184853.

We can confirm the following details from our system to help complete your records:
- ISIN: CH0244767585 (UBS Group AG)
- Trade Date: 2026-03-19
- Settlement Date: 2026-03-20
- Quantity: 29,837
- Net Amount: EUR 1,666,712.84
- Side: Sell

Please note our system records the counterparty under identifier 5UMCZOEYKCVFAW8ZLO05. Let us know if you need further clarification or confirmation of the legal counterparty name.

Best regards,
Settlement Operations
```