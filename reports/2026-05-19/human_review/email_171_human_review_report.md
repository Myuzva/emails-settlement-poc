# Settlement Inquiry Report

## 1. Decision

**Settlement Inquiry:** Yes  

**Priority:** High  

**Recommended Action:** Route to human review / operations.

**Reason:** HOST has a single trade match for YN21200009 and shows counterparty LEI E57ODZWZ7FF32TWEFA76, enriched as Citigroup, while the email states the booking reflects HSBC. The counterparty discrepancy is material and concerns a closed trade, so amendment or reopen procedure should be handled manually.

---

## 2. Email Summary

**Email ID:** email_171.eml  
**Subject:** Trade Exception – YN21200009  
**Sender:** Anna Kowalski <a.kowalski@warsawsec.pl>  
**Received:** Tue, 28 Apr 2026 15:38:49 +0200  
**Counterparty:** HSBC (Email) / Citigroup (Expected/HOST)

The sender reports a retrospective counterparty error on trade YN21200009, which is currently marked as settled and closed. The booking reflects HSBC as the counterparty; however, the agreement confirms this should be Citigroup. The sender asks how to reopen or amend the settled/closed trade.

---

## 3. Classification
- **Primary Type:** counterparty_mismatch
- **Multi-type:** false

---

## 4. Multi-Trade Notes
- **Multi-trade Email:** Yes
- **Related Trades:** ZQ36307399 (Macquarie Group, Novartis AG, EUR 271,863.21), YJ04718367 (ING Bank, Meta Platforms Inc., EUR 1,571,449.56)

---

## 5. HOST Lookup Comparison

| Field | Email Value | HOST Value | Status | Severity |
|-------|-------------|------------|--------|----------|
| reference_number | YN21200009 | YN21200009 | match | none |
| counterparty_name | HSBC | Citigroup | mismatch | high |
| counterparty_lei | null | E57ODZWZ7FF32TWEFA76 | missing_in_email | none |
| security | null | DE000BASF111 | missing_in_email | none |
| trade_date | null | 2026-03-20 | missing_in_email | none |
| settlement_date | null | 2026-03-23 | missing_in_email | none |
| side | unknown | Buy | unknown | none |
| quantity | null | 77982 | missing_in_email | none |
| amount | null | 1301274.03 | missing_in_email | none |
| currency | null | EUR | missing_in_email | none |
| status | settled/closed | Closed | match | none |

### Discrepancy Flags
- counterparty_mismatch
- host_counterparty_matches_requested_citigroup
- email_counterparty_hsbc_maps_to_different_lei
- settled_closed_trade_amendment_requested

---

## 6. Findings

The trade YN21200009 was found in HOST. The HOST system shows the counterparty as Citigroup (LEI E57ODZWZ7FF32TWEFA76), which aligns with the sender's expected counterparty. However, the sender claims their booking reflects HSBC. The trade is already marked as Closed in HOST.

The discrepancy is material as it involves a counterparty mismatch on a closed trade, requiring manual intervention to determine if an amendment or reopen procedure is necessary.

---

## 7. Next Steps

1. Review the trade booking in the internal system to confirm the counterparty details.
2. Investigate the discrepancy between the sender's booking (HSBC) and the HOST system (Citigroup).
3. Determine the appropriate procedure for amending or reopening a closed trade if necessary.
4. Respond to the sender with instructions on how to proceed with the amendment.
