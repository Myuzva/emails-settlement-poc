# Settlement Discrepancy Report: Human Review Required

## Case Overview
- **Email File:** email_025.eml
- **Reference Number:** HS69732881
- **Date Processed:** 2026-05-19
- **Status:** Needs Human Review
- **Confidence Score:** 0.22

## Reason for Human Review
The automated host lookup by trade reference (HS69732881) returned a 404 Not Found. Because the email explicitly requests confirmation on whether the reference was assigned in error, the absence of a HOST match should not be assumed to prove the email incorrect. Manual investigation is required to locate the trade using alternate systems or soft-matching.

## Extracted Email Data
- **Trade Reference:** HS69732881
- **Security Name:** Goldman Sachs Group Inc.
- **Counterparty:** Nomura Securities
- **Trade Date:** 2026-03-02
- **Settlement Date:** 2026-03-03
- **Side:** sell
- **Quantity:** 70,804
- **Amount:** 1,237,667.68 USD
- **Reported Status:** closed

## Host System Data
- **Lookup Strategy:** by_trade_reference
- **Host Status:** no_match (404 Not Found)
- **Host Trade Reference:** N/A
- **Host Security:** N/A
- **Host Counterparty:** N/A
- **Host Settlement Date:** N/A
- **Host Quantity:** N/A
- **Host Amount:** N/A

## Discrepancies & Flags
- **no_host_match:** Trade reference HS69732881 was not found in the host system.
- **reference_missing_on_host:** High severity.
- **trade_missing_on_host:** High severity.
- **requires_manual_investigation:** High severity.

## Recommended Action
Human review required. Operations team should perform manual booking/system search for trade reference HS69732881 (including alternate systems and soft-matching on security name, dates, and counterparty), confirm whether the reference was assigned in error, and contact the sender to request clarification or the correct reference if necessary. Do not assume the host absence implies the email is incorrect; escalate if no record is found after manual search.

## Evidence & Attachments
- **Attachment:** `trade_details.txt` (Parsed successfully, contains trade data)
- **Quote 1:** "we encountered reference HS69732881, which we are unable to reconcile against any booking in our system."
- **Quote 2:** "Please confirm whether this reference was assigned in error, or provide the correct reference number"