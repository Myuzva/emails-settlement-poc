# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Human review required. Investigate the trade date discrepancy (email: 2026-03-26 vs host: 2026-03-19) to determine whether the email/attachment or the booking contains an error. Confirm whether the settlement date amendment is needed once trade date provenance is established. Use counterparty LEI FAK6QKWT97JDDAHS3S03 (Merrill Lynch) for any amendment routing.

**Reason:** Critical mismatch on trade_date between email and host reduces overall confidence and requires human review.

---

## 2. Email Summary

**Email ID:** email_053  
**Subject:** Trade Status Update Request – KR86473518  
**Sender:** Claire Dubois <c.dubois@paribas-ops.fr>  
**Received:** Tue, 28 Apr 2026 15:38:48 +0200  
**Counterparty:** Merrill Lynch

The sender reports a settlement date inconsistency for trade KR86473518, which is already closed in their system. The trade should have settled on 2026-03-20, but the booking reflects a different date.

---

## 3. Classification
- **Primary Type:** wrong_date (originally settlement_date_mismatch)
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** No
- **Related Trades:** None

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | KR86473518 | KR86473518 | match | none |
| security_isin | null | US0378331005 | missing_in_email | none |
| security_name | Apple Inc. | null | missing_in_host | low |
| settlement_date | 2026-03-20 | 2026-03-20 | match | none |
| trade_date | 2026-03-26 | 2026-03-19 | mismatch | high |
| quantity | 85772 | 85772 | match | none |
| amount | 1549075.48 | 1549075.48 | match | none |
| currency | EUR | EUR | match | none |
| side | buy | Kauf | match | none |
| counterparty_name | Merrill Lynch | Merrill Lynch (LEI FAK6QKWT97JDDAHS3S03) | match | none |
| status | closed | Geschlossen | match | none |

### Discrepancy Flags
- trade_date_mismatch
- security_name_missing_in_host

---

## 6. Findings

The trade was found in HOST, but there is a critical mismatch on the trade date (email: 2026-03-26 vs host: 2026-03-19).

The email reports a settlement date (2026-03-20) that precedes the email trade date (2026-03-26), which is highly unusual and suggests an error in the email or attachment.

Host record contains ISIN only (US0378331005); security name is missing in host response.

---

## 7. Next Steps

1. Investigate the trade date discrepancy to determine whether the email/attachment or the booking contains an error.

2. Confirm the source of the email trade date, as the reported settlement date precedes it.

3. Confirm whether the settlement date amendment is needed once trade date provenance is established.

4. Use counterparty LEI FAK6QKWT97JDDAHS3S03 (Merrill Lynch) for any amendment routing.

---