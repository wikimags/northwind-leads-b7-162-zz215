# B7-162 Run 1 input data and before-state evidence

Task: Audit lead form submissions from a live site. Assigned surface: Mobile. Platforms: ChatGPT Chat and Claude Chat. This package contains preparation evidence, not an executed model test or its output.

## Exact sources

- Netlify team: zz215; account: zz215@expert.micro1.ai.
- Project: northwind-leads-b7-162-zz215.
- Site ID: cbb4cd0a-3d92-4dd6-b08a-5ee798961708.
- Form: sales-enquiries, ID 6ab3a9b814c7d5000808e45c.
- Final setup deploy: 6ab3ad4e34d622a06f2e58fb.
- Form detection enabled; 16 submissions in the Verified collection; 0 in quarantine; no submission notification hooks.
- Actual creation interval: September 23, 2026, 10:28:58.742 through 10:39:15.110 UTC (13:28:58.742 through 13:39:15.110 EAT).
- Evaluation interval: August 25, 2026 at 00:00 EAT through September 24 at 00:00 EAT, exclusive of the end.

## Why this data supports the test

The form contains detailed buying enquiries with names, emails, companies, roles, interests, messages and follow-up permission, as well as a duplicate, ambiguous or malformed contact details, promotional spam, and non-sales requests. Each record has its original Netlify submission ID and created_at timestamp, plus a fixture ID to make evidence matching easier. All 16 records are retrievable through the Netlify connector with get-submissions and limit 100.

Every content field was compared to the seed file and matched. Source CSV and JSON preserve the records, original timestamps and IDs. IP addresses, user agents and referrers are omitted from the shared copies because they are not needed for the task. All contact details are fictional; example.com email addresses are intentionally non-deliverable placeholders.

## Setup actions and limitations

The site and form were created and enabled before the test. Sixteen synthetic messages were posted to the live form. Netlify quarantined some records and temporarily returned HTTP 429 while seeding; after a cooldown the remaining records were saved. The quarantined fixture records were marked verified during setup so both models receive the same complete list. No protection setting was disabled. Netlify's Verified label is only the prepared collection state, not a claim that all records are genuine sales leads or deliverable email addresses.

All records were seeded today. The fixture supports review of submissions inside the requested period but does not exercise exclusion of older out-of-window records. No artificial historical dates were inserted. No actual outreach was sent and no notification hooks were configured.

The six screenshots are desktop preparation evidence. Capture the actual prompt, tool activity and model result on the assigned mobile surface during each run.

## Evidence files

- LiveForm_01.png: published form and fields.
- FormsEnabledCount_02.png: source project, enabled form detection, one form and 16 submissions.
- AllSubmissions_03.png: full Netlify list including all 16 records.
- ReviewAndSpam_04.png: native Olivia record with malformed email and nearby spam/ambiguous entries.
- GenuineLead_05.png: native Aisha record, pricing interest, message and follow-up permission. Viewport capture cropped below the relevant fields to exclude IP metadata.
- PublicSourceOverview_06.png: public, sanitized copy of the actual source records, not a model answer.
- Submissions.csv / Submissions.json: complete source records, with exact IDs and UTC timestamps.
- Before_Forms.json: original form schema and collection count.
- Before_Manifest.json: capture time, ID inventory, verified/quarantine counts and validation outcome.

## Before links

- Native Netlify records (requires project access): https://app.netlify.com/projects/northwind-leads-b7-162-zz215/forms/6ab3a9b814c7d5000808e45c
- Public live form: https://northwind-leads-b7-162-zz215.netlify.app/
- Fixed before-state evidence page: https://6ab3ad4e34d622a06f2e58fb--northwind-leads-b7-162-zz215.netlify.app/evidence/
- Fixed source CSV: https://6ab3ad4e34d622a06f2e58fb--northwind-leads-b7-162-zz215.netlify.app/evidence/input-records.csv
- Fixed source JSON: https://6ab3ad4e34d622a06f2e58fb--northwind-leads-b7-162-zz215.netlify.app/evidence/input-records.json
- Dataset notes: https://6ab3ad4e34d622a06f2e58fb--northwind-leads-b7-162-zz215.netlify.app/fixture-notes

Public evidence links do not require a Netlify login. They are a snapshot and will not change when the live site or submissions later change. Use native Netlify records as the model's input source; the public copy supports independent verification.

## Run 2 and after-state evidence

Use the same prompt and date window in a fresh chat on the other platform, with access to this same Netlify account. Before Run 2, reread the source and compare the 16 IDs and content with this manifest; save a new Run 2 baseline. After each run, verify that all records, labels and form settings remain unchanged. Preserve the actual model CSV and screenshots separately from the answer key. No reset is necessary if Run 1 stays read-only.
