# Human-in-the-Loop (HITL) Review Report

## Case Information
- **Email File:** email_078.eml
- **Message ID:** <177738352836.31976.4563803994726561943@Arek.yallo.box>
- **Date Processed:** 2026-05-19
- **Primary Trade Reference:** DY52987070
- **Classification:** security_mismatch (Confidence: 0.94)

## Review Triggers
- Security values conflict inside the email: booked instrument versus confirmation instrument
- ZIP contained nested image `trade_details.jpg`; OCR/text extraction was unavailable or failed and it may contain trade-critical data

## Extracted Data Summary
| Field | Extracted Value | Confidence |
|-------|-----------------|------------|
| Trade Reference | DY52987070 | 0.97 |
| Instrument | Nestlé S.A. | 0.90 |
| Side | unknown | 0.00 |

## Discrepancy Details
- **Type:** security_mismatch
- **Description:** Sender records show Nestlé S.A.; received confirmation references Alphabet Inc.; sender requests clarification of the correct instrument before settlement.
- **Sender Value:** Nestlé S.A.
- **Expected/Requested Value:** Alphabet Inc. referenced in confirmation; clarification requested

## Evidence
- **subject**: "Clarification Required: Trade DY52987070"
- **body**: "Regarding trade DY52987070, our records indicate the traded security is Nestlé S.A.. However, the confirmation we received references Alphabet Inc."
- **body**: "Could you please clarify the correct instrument and confirm the necessary steps to resolve this before settlement?"

## Attachments
- `trade_details.zip` (application/zip) - parsed 
  - *Warnings:* ZIP opened recursively; contained trade_details.jpg
- `trade_details.jpg` (image/jpeg) - error 
  - *Warnings:* Nested image was unpacked, but OCR/text extraction was unavailable or failed; content not read

## Analyst Action Required
1. Review the conflicting security values (Nestlé S.A. vs Alphabet Inc.).
2. Manually inspect `trade_details.jpg` for the correct trade details.
3. Confirm the correct instrument and proceed with settlement resolution.
