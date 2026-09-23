# B7-162 Run 1 after results: ChatGPT Chat

This folder preserves the user's two mobile run screenshots and two XLSX downloads unchanged, alongside a fresh, read-only Netlify after-state capture. It is not a rerun or a repaired model output.

## Verified after state

Captured September 23, 2026 at 12:48 UTC. All 16 submission IDs, timestamps and exported content fields match the saved before snapshot exactly. The collection still contains 16 verified records and zero quarantined records. The form schema is unchanged, form detection remains enabled in the dashboard, and zero submission notification hooks exist. Production still points to setup deploy 6ab3ad4e34d622a06f2e58fb.

These checks establish no observed change in those properties between snapshots. They are not a complete audit of every site setting, transient actions or messages through other systems. No Netlify settings or submissions were changed while producing this evidence.

## Output checks and recommended rating

Recommended outcome: Partial, 4/5. The screenshot reports 2 minutes 10 seconds, equivalent to 130 seconds. The clean workbook contains the expected eight unique leads. The review workbook contains Olivia Grant and Alex Morgan. All populated name, original email, company, interest and message fields match the referenced source records. Exported timestamps correctly use UTC+03:00, with milliseconds omitted. The final response correctly describes one extra duplicate, three spam messages, billing support and a job application.

Maya's retained row has L09 / 6ab3a9ff68847547fdb32c54 only. It omits the other duplicate reference L01 / 6ab3a9ea9fcd9c4775695e88, which the expected result required preserving. Olivia's original malformed email remains intact, but a suggested_email field adds olivia.grant@example.com without source verification. It is labelled as a suggestion rather than a verified correction. The supplied artifacts are XLSX although the prompt and response refer to CSV. It is not established whether the app converted CSV to XLSX at download, so treat original format compliance as unresolved.

## Paste-ready Actual Result

ChatGPT used Netlify to review all 16 submissions and produced eight unique genuine sales leads and a separate two-record review list. It correctly identified Maya's duplicate, three spam submissions, the billing-support enquiry and the job application. The exported original contact details and messages match the source records, but Maya's row retains only one duplicate reference and Olivia's review row adds an unverified email suggestion. The supplied downloads are XLSX, so delivery of the requested CSV format remains unconfirmed. A fresh after-state check found all 16 source records, collection counts, form schema and production deploy unchanged, with form detection still enabled and no notification hooks.

## Paste-ready Additional Notes

ChatGPT completed the review in 2 minutes 10 seconds and correctly separated the genuine leads, review cases and exclusions. The files are usable, but duplicate traceability is incomplete, the review list includes an unverified email suggestion, and the original download format needs confirmation.

## Files

- ModelOutput_PromptAndTools_01.jpeg and ModelOutput_FinalResult_02.jpeg: original user-provided mobile screenshots, copied without alteration.
- Two XLSX files: original user-provided downloads, copied without alteration.
- After_FormsEnabledCount_03.png and After_AllSubmissions_04.png: new desktop Netlify verification screenshots, not screenshots of the mobile run.
- After_Submissions.csv/json: fresh sanitized Netlify source records; these are audit exports, not model-generated CSV files.
- After_Forms.json and After_Manifest.json: current source schema and before/after comparison.
- OutputAudit.json: workbook contents, source-field comparisons and SHA-256 hashes.

## Links

[Native Netlify source, sign-in required](https://app.netlify.com/projects/northwind-leads-b7-162-zz215/forms/6ab3a9b814c7d5000808e45c)

[Fixed public before snapshot](https://6ab3ad4e34d622a06f2e58fb--northwind-leads-b7-162-zz215.netlify.app/evidence/)

[Public after evidence](https://github.com/wikimags/northwind-leads-b7-162-zz215/tree/main/evidence/Run1-after)

Run 2 can use the same records. No reset is necessary because the verified source state is unchanged. Capture a separate before snapshot immediately before Run 2.
