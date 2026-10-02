---
name: grepme
description: grepme scans this machine's coding sessions, local git checkouts, and private GitHub repos the candidate contributes to or maintains, then writes only candidate-approved claims to evidence.md. Never send code, diffs, or private identifiers to Talentsearch.
disable-model-invocation: true
---

# grepme

Build short professional claims from work that is not public. The candidate runs grepme on their own machine. Talentsearch never clones or reads private GitHub repositories.

Read [references/privacy.md](references/privacy.md) and [references/evidence-format.md](references/evidence-format.md) before you scan anything. The privacy rules override every other step.

Stop after you load grepme. Tell the candidate what you are about to do, then wait until they confirm.

## What you may look at

Both sources stay on this machine, using credentials the candidate already has:

1. Local coding-session history for this agent.
2. Local git checkouts.
3. Private GitHub repositories the candidate **contributes to or maintains**, reached only through the GitHub connection already installed in this agent: the GitHub plugin, `gh`, or GitHub MCP.

Do not ask for a new GitHub token. Do not list organizations the candidate merely belongs to. Do not scrape repos they do not contribute to or maintain. If no GitHub connection is available, say so and continue with local checkouts and session history only.

## Steps

1. **Session check.** Look only at local coding-session history on this machine. Report what you can see: tools, a rough date range, and project names. Do not upload transcripts.
2. **Repo pick.** Build one list and ask which repos to scan. Unselected repos are out of scope. The list may include local git checkouts and private GitHub repos from the connection above. Wait for the candidate to choose.
3. **Insight pass.** From commits, reviews, and design discussion in the selected repos, draft claims about bugfixing, review judgment, and system design. Each claim has **Section**, **Signal** (`commit`, `review`, or `design`), **Claim**, and **Mess** (what mess you stopped), plus a rough timeframe and technologies when you know them. Write `Mess`. The server may accept `Summary` as an alias for `Mess`; still write `Mess`. Follow the privacy file. GitHub bodies, diffs, and file contents stay on this machine.
4. **Review.** Show every claim. The candidate approves, edits, or drops each one before you write anything. Dropped claims are gone.
5. **Exit.** After the candidate approves each remaining claim, write a local `evidence.md` using the evidence-format file. Stop there. Do not send the file, and do not ask for a token. Tell the candidate to upload `evidence.md` on the Talentsearch profile editor, in **Private work evidence** (Add evidence). Tell them not to commit that file to a company repository. A highlight attached to an existing role stays off the public page. Other claims stay private until the candidate sets them to public and publishes.
