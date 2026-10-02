# GitHub Issue Plan (EXECUTED 2026-10-02)

This was the plan approved by the PM before any issue was created. It was run
once: 6 issues (#1-#6) were created and added to project 7. See
`ai-pm-audit-summary.md` for the result. The `item-add` step was not needed
because the issues were added to the board automatically.

- Repo: `Dhanyacode12/aipm-user-stories`
- Project: `User Stories Workshop` (number 7, owner `Dhanyacode12`)
- Existing issues in the repo: none (checked)
- Labels: none planned (existing labels like bug/enhancement do not match; Work type is a project field)

## Commands to run (one per story)

```bash
gh issue create \
  --repo Dhanyacode12/aipm-user-stories \
  --title "<title>" \
  --body-file <body file>
```

Then, to add each issue to the board (separate approval):

```bash
gh project item-add 7 --owner Dhanyacode12 --url <issue url>
```

Project fields (Work type, Story quality, Risk area) are set afterwards, in the browser or with `gh project item-edit`.

## Issues

| # | Title | Epic | Work type | Source |
|---|---|---|---|---|
| 1 | Story 1: Show the source of every answer | A | Story | PM |
| 2 | Story 2: Tell the agent when no approved answer exists | A | Story | PM |
| 3 | Story 3: Flag a wrong or unclear answer | C | Story | PM |
| 5 | Story 5 (draft): Ask a policy question in my own words | A | Story | Agent draft, PM kept |
| 6 | Story 6 (draft): Only approved documents are searchable | B | Story | Agent draft, PM kept |
| 7 | Story 7 (draft): Answers stay drafts until the agent sends them | C | Story | Agent draft, PM kept |

**Excluded by the PM (no GitHub issue will be created):** Story 4 (evidence
that the pilot saves time) and Story 8 (fast enough to use). They stay in
`story-backlog.md` for now. Story numbers are kept, so issues are 1, 2, 3, 5, 6, 7.

Each issue body will contain exactly the text in `story-backlog.md` for that
story: the story sentence, acceptance criteria, open questions, risk or
assumption, epic, and a status line saying who wrote it. No text is added.

## Example body (Story 1)

```text
As a support agent,
I want each answer to show its source policy and section,
so that I can verify it before I reply to a customer.

Acceptance criteria:
- Every answer shows the policy title and section it came from.

Open question:
- Which documents count as approved?

Risk / assumption:
- Assumption: the policy documents are up to date.

Epic: A, Trustworthy answers | Work type: Story | Author: PM
```

## Assumptions and weak spots (for the PM to see before approving)

- Story 3 is weak on Small and Estimable (the PM chose to keep it whole).
- Story 6 assumes a "policy owner" role exists.
- Stories 5-7 are agent drafts that the PM kept; they will be labeled as drafts
  in the issue title.

## Risks of running this

- Creating issues on GitHub is visible and not trivially reversible: issues can
  be closed, but not silently erased. Two runs would create duplicates.
- Mitigation: run once, then `gh issue list` before anything else.
