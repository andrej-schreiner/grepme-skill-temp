# Privacy rules

These rules bind the skill and anything it sends to Talentsearch.

## Allowed in a claim

- Role-level outcomes ("owned a migration rollback plan").
- Technologies ("PostgreSQL", "TypeScript").
- Kinds of work: debugging, review, architecture, implementation.
- A rough timeframe (`YYYY` or `YYYY-MM`).
- That the work was private.

## Forbidden in any file that leaves this machine and in any API body

- Source code, diffs, patches, and logs.
- Secrets, tokens, keys, and connection strings.
- Hostnames and internal URLs.
- Secret employer names, customer names, and confidential codenames. A public employer name already on the candidate's draft may be named.
- Internal ticket ids.
- Private repository names. A public repository name is allowed only when the candidate explicitly keeps it.
- Raw session transcripts.
- File paths, commit hashes, and review-thread quotes.

GitHub file contents, pull request bodies, diffs, and review comments stay on this machine. Only candidate-approved claim text may be written to `evidence.md` or sent to Talentsearch.

Talentsearch servers must not be asked to clone or read private GitHub repositories. Do not paste a GitHub token into Talentsearch.

## Good claims

- "Designed a rollback for a production schema migration." Signal: `design`. Section: `project`.
- "Caught a retry bug in review before it shipped." Signal: `review`. Section: `achievement`.
- "Fixed a data race in a background worker." Signal: `commit`. Section: `experience`. Technologies: `Go`.

## Bad claims

- "Fixed the null pointer in `src/payments/Charge.ts` at Acme Corp, ticket PAY-4412."
- A unified diff, a `diff --git` header, or a fenced code block.
- "In the private repo `acme/billing-api` I rewrote `applyInvoice`."
- A pasted chat transcript from this session.

If a draft claim needs a forbidden detail to make sense, generalize it or drop it. Do not "anonymize" by leaving the name and asking Talentsearch to strip it later.

## evidence.md

Write `evidence.md` only after the candidate approves each claim. Tell them not to commit that file to a company repository.
