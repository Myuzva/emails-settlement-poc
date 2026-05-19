# Settlement Exception Report: HITL Required

## Case Information
- **Date Generated:** 2026-05-19
- **Email File:** email_098.eml
- **Message ID:** <177738352860.31976.5114375138260309234@Arek.yallo.box>
- **Primary Classification:** missing_confirmation
- **Confidence Score:** 0.78

## Trade Details (Extracted)
- **Trade Reference:** PA83889136
- **Counterparty:** Macquarie Group
- **Security:** Tesla Inc.
- **Trade Date:** 2026-03-26
- **Settlement Date:** 2026-03-27
- **Quantity:** 30,550
- **Amount:** 1,167,404.10 EUR

## Host System Reconciliation
- **Host Status:** matched
- **Host Trade Reference:** PA83889136
- **Host Status Value:** Closed
- **Discrepancies Found:**
  - status_mismatch_Closed_vs_settled

## Human-in-the-Loop (HITL) Assessment
- **Review Required:** Yes
- **Reason for Review:** HOST status is 'Closed' while email reports 'settled' — terminology differs and may be meaningful; requires human confirmation.
- **Recommended Action:** Human review: confirm that host status 'Closed' is equivalent to sender's 'settled' for this trade and, if confirmed, provide the requester with the final trade confirmation or SWIFT copy. If not equivalent, investigate settlement exception and advise counterparty.

## Evidence & Attachments
- **Body Quote:** "Trade PA83889136 is recorded as settled in our system. Please provide the final trade confirmation or SWIFT confirmation as appropriate."
- **Attachment Quote:** "Sec Name Tesla Inc.; Nom 30,550; B/S Buy; Dealer Macquarie Group; Face Value 1,167,404.10; Currency EUR; Trd Date 2026.03.26; Stlmt Date 2026.03.27" (from trade_details.txt)