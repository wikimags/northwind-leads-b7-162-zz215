# Northwind lead form audit: B7-162

Public test fixture and before-state evidence for the Netlify connector evaluation. All contacts and companies are fictional. This repository is preparation material, not a model run result.

## Inspect the data

- [All 16 source submissions (CSV)](site/evidence/input-records.csv)
- [Source submissions with Netlify IDs and timestamps (JSON)](site/evidence/input-records.json)
- [Before-state screenshots and records](evidence/Run1-before/)
- [Download before-state evidence ZIP](B7-162_Run1_BeforeEvidence.zip)
- [Input inventory, setup details and limitations](evidence/Run1-before/B7-162_Run1_InputData_README.md)
- [Prompt](PROMPT.txt)
- [Expected results and keywords](EXPECTED-RESULTS.md)
- [Expected clean leads CSV, answer key only](EXPECTED-clean-leads.csv)

## Source application

Project: northwind-leads-b7-162-zz215. Site ID: cbb4cd0a-3d92-4dd6-b08a-5ee798961708. Form: sales-enquiries. Form ID: 6ab3a9b814c7d5000808e45c.

- [Native Netlify submissions, requires project access](https://app.netlify.com/projects/northwind-leads-b7-162-zz215/forms/6ab3a9b814c7d5000808e45c)
- [Public before-state snapshot](https://6ab3ad4e34d622a06f2e58fb--northwind-leads-b7-162-zz215.netlify.app/evidence/)
- [Live test form](https://northwind-leads-b7-162-zz215.netlify.app/)

There are 16 submissions: eight unique genuine leads, one extra duplicate, two records for review, three spam messages and two non-sales enquiries. Netlify's Verified collection label is a storage state, not a lead-quality or email-deliverability judgment. All records were created on September 23, 2026, so this fixture does not test exclusion of older records. Shared exports omit IP addresses, user agents and referrers.

Run the test in a fresh mobile ChatGPT Chat or Claude Chat session against the Netlify connector. Keep the answer key out of the model's input. No messages, submission edits, spam-label changes or site-setting changes are authorized by the test prompt. Verify the same 16 records before Run 2 and capture each run separately.
