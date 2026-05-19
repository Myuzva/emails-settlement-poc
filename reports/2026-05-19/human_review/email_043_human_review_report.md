# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Escalate to operations: investigate the amount discrepancy (email shows 2,158,002.39 CHF vs host 1,662,949.54 CHF). Confirm which system is authoritative, review settlement/cash postings and provide corrected settlement instructions if required. Include trade ref VE93513959 and LEI 3TK20IVIUJ8J3ZU0QE75 in the investigation.

**Reason:** Human review required because amount is a sensitive field and remains ambiguous after host lookup. Amount on host (1,662,949.54 CHF) differs materially from the email-extracted amount (2,158,002.39 CHF). Host amount equals the sender's 'correct' amount reported in the email body.

---

## 2. Email Summary

**Email ID:** email_043  
**Subject:** Outstanding Trade – Action Required – VE93513959  
**Sender:** Sarah Jensen <s.jensen@nordbank.com>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** ING Bank

The sender claims the correct settled notional is CHF 1662949.54, but settlement was processed at CHF 2158002.39.

---

## 3. Classification
- **Primary Type:** wrong_amount (originally amount_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | VE93513959 | VE93513959 | match | none |
| security_isin | null | CH0012530207 | missing_in_email | none |
| security_name | ABB Ltd. | ABB Ltd. | match | none |
| settlement_date | 2026-03-04 | 2026-03-04 | match | none |
| trade_date | 2026-03-03 | 2026-03-03 | match | none |
| quantity | 46388 | 46388 | match | none |
| amount | 2158002.39 | 1662949.54 | mismatch | high |
| currency | CHF | CHF | match | none |
| side | buy | buy | match | none |
| counterparty_name | ING Bank | ING Bank | match | none |
| status | settled | settled | match | none |

### Discrepancy Flags
- amount_mismatch
- host_amount_matches_sender_expected_value
- human_review_required

---

## 6. Findings

The trade was found in HOST, but the settlement amount differs from the counterparty’s email.

The likely cause of the settlement break is an amount mismatch. The host amount (1,662,949.54 CHF) matches the sender's expected value, but the email states the settlement was processed at 2,158,002.39 CHF. The case should be reviewed before any confirmation is sent externally.

---

## 7. Next Steps

1. Verify the correct amount against internal trade booking records and cash postings.

2. Confirm which system is authoritative regarding the processed amount.

3. Provide corrected settlement instructions if required.

4. Keep the case under analyst review until the discrepancy is resolved.

---