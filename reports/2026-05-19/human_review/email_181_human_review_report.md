# Human-in-the-Loop (HITL) Review Report

## Case Metadata
- **Date Generated:** 2026-05-19
- **Source Email:** `email_181.eml`
- **Case Status:** `needs_human_review`
- **Confidence Score:** 0.95
- **Target Folder:** `human_review`

## Reason for Review
- **Primary Reason:** unsupported_schema
- **Description:** The case requires human review due to an unsupported schema or routing reason.

## Extracted Trade Details
- **Trade Reference:** QQ86998552
- **Counterparty:** Credit Suisse
- **Security:** Nestlé S.A.
- **Trade Date:** 2026-03-27
- **Settlement Date:** 2026-03-30
- **Side:** sell
- **Quantity:** 87,455
- **Amount:** 557,959.98 CHF
- **Reported Status:** closed

## Discrepancy / Request Details
- **Type:** missing_confirmation
- **Description:** Requesting archival documentation / settlement confirmation

## Evidence
- **Body Snippet:** "Please provide a copy of the relevant settlement confirmation or trade advice for our records" (Supports: classification.primary_type)
- **Attachment Snippet (trade_details.txt):** "Net Amount 557,959.98\nSecurity Nestlé S.A.\nSettlement Date 30.03.2026\nQuantity 87,455" (Supports: extracted_data.trades[0].quantity, extracted_data.trades[0].net_amount)

## Attachments
- `trade_details.txt` (text/plain) - parsed

## Action Required
- [ ] Review the unsupported schema issue.
- [ ] Verify the extracted trade details against the original email and attachment.
- [ ] Provide the requested settlement confirmation to the counterparty.
