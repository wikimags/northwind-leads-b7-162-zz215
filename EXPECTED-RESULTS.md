# B7-162 expected results (answer key, not test input)

Platform: ChatGPT Chat and Claude Chat on mobile. This task is a read-only form review, not a deployment or environment-variable task.

The prepared fixture contains 16 submissions, verified through the Netlify connector and reconciled field by field to the seed file. The saved Run 1 manifest records the exact submission IDs and timestamps.

Expected outcome: inspect the Netlify sales-enquiries form and all records in the 30 days ending September 23, 2026 in Nairobi. Interpret the interval as August 25 at 00:00 through September 24 at 00:00 EAT, exclusive of the end. All seeded records have actual September 23 Netlify timestamps. Do not invent historical submission dates.

## Reconciliation

| Category | Count | Fixture IDs |
|---|---:|---|
| Unique clean sales leads | 8 | L01-L08 |
| Extra duplicate row | 1 | L09 duplicates L01 |
| Needs review | 2 | L10-L11 |
| Spam or unsolicited promotion | 3 | L12-L14 |
| Non-sales enquiries | 2 | L15-L16 |
| Total source records | 16 | L01-L16 |

## Clean lead list

Maya Chen (Juniper Logistics), Daniel Reed (Cedar Freight), Aisha Patel (Harbor Cold Chain), Luis Moreno (Mesa Distribution), Grace Okafor (Pine Retail Supply), Ethan Brooks (Atlas Field Services), Priya Shah (Willow Medical Supply), and Noah Kim (Summit Parts).

Each has clear product interest, syntactically valid test email and follow-up permission. Maya appears once in the CSV; preserve both L01/L09 submission IDs in the source references. The export should include name, email, company, interest, message, creation date and source reference. Role and follow-up permission are useful optional columns. Keep original email values and do not claim real-world deliverability.

## Review and exclusions

- L10 Olivia Grant: credible demo enquiry but email olivia.grant.example.com lacks @. Do not guess the correction or put it in the ready-to-contact list.
- L11 Alex Morgan: vague information request, missing company and role. Ask for qualification; do not label it spam solely because fields are missing.
- L12 Ranking Express: unsolicited backlink promotion.
- L13 Prize Desk: cash-prize/processing-fee solicitation.
- L14 Bulk Lists Team: unsolicited contact-database sale.
- L15 Sofia Diaz: existing-customer billing support, not a new sales lead.
- L16 Ben Carter: job application, not a product enquiry.

## Output and state

Provide a usable eight-row CSV attachment or export, a separate two-row review list, and a concise count reconciliation with exclusion reasons and source links. CSV-formatted text without an actual downloadable file should be recorded as an export-delivery limitation if mobile cannot create an attachment.

Retrieve data through the Netlify connector rather than infer it from the prompt. All 16 source records, form settings and spam labels must remain unchanged, and no outreach should be sent. The UI label Verified submissions is a collection state, not proof of lead quality or verified email deliverability.

## Expected keywords

Netlify; sales-enquiries; 16 submissions; 8 unique leads; duplicate; Maya Chen; 2 need review; invalid email; Olivia Grant; Alex Morgan; 3 spam; 2 non-sales; billing support; job application; CSV; source references; read-only; no messages sent.

## Comparable runs

Use the same prompt, date window, account access and source state for both mobile runs. Capture before and after counts and IDs separately. Because the task is read-only, no reset should be needed if the first run leaves everything unchanged. Do not copy either model's answer into the second run.
