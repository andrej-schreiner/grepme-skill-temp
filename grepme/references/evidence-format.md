# evidence.md

A local markdown file the candidate can re-read. It is not a git commit. Do not add code blocks.

```markdown
# Private work evidence

Nothing in this file is company-confidential. Only the approved claim lines may be shared with Talentsearch. Do not commit this file to a company repository.

## Owned a migration rollback plan

- Section: project
- Signal: design
- Claim: Owned a migration rollback plan for a production data store.
- Mess: Stopped a failed migration from leaving the store half-applied.
- Dates: 2024-03 to 2024-06
- Technologies: PostgreSQL

## Caught a retry bug in review

- Section: achievement
- Signal: review
- Claim: Caught a retry bug in review before it shipped.
- Mess: Stopped a retry loop from shipping.
- Dates: 2025
- Technologies: none
```

Rules:

- The header states that nothing here is company-confidential and that only approved lines may be shared.
- One section per approved claim.
- Each claim has **Section** (`experience`, `project`, or `achievement`), **Signal** (`commit`, `review`, or `design`), **Claim**, and **Mess** (what mess you stopped). Then rough dates and technologies when you know them.
- The mess line is named `Mess`. The server may accept `Summary` as an alias for `Mess`. Still write `Mess`.
- No code blocks, diffs, private repository names, secret employer names, confidential codenames, hostnames, ticket ids, or transcripts. A public employer already on the draft may be named.
- Dates are `YYYY` or `YYYY-MM`. Omit a date you do not know. A range is `YYYY-MM to YYYY-MM`. Use `none` when there are no technologies.
- The candidate uploads this file. Do not send it yourself.
