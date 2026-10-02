# AI Project Manager Audit Summary

Date: 2026-10-02 | Project: Policy Assistant Pilot | Agent: Claude (Sonnet 5.5)

## 1. Files created or changed (local, not committed or pushed)

All six are new, untracked files in the repo folder. No existing course file was modified.

| File | Purpose |
|---|---|
| `story-backlog.md` | 8 stories: 1-3 PM-written, 4 placeholder, 5-8 agent drafts |
| `epic-map.md` | Initiative, 4 epics, story placement, known gaps |
| `acceptance-criteria.md` | All criteria in one table |
| `ready-done-agreements.md` | Draft DoR and DoD (Now / Soon / Later) |
| `ai-collaboration-log.md` | Decisions on agent suggestions |
| `github-issue-plan.md` | The plan approved before issues were created |

## 2. GitHub issues created

6 issues in `Dhanyacode12/aipm-user-stories`, created once each, verified with
`gh issue list` (no duplicates, no missing):

| Issue | Title |
|---|---|
| #1 | Story 1: Show the source of every answer |
| #2 | Story 2: Tell the agent when no approved answer exists |
| #3 | Story 3: Flag a wrong or unclear answer |
| #4 | Story 5 (draft): Ask a policy question in my own words |
| #5 | Story 6 (draft): Only approved documents are searchable |
| #6 | Story 7 (draft): Answers stay drafts until the agent sends them |

Issue numbers do not match story numbers (Stories 4 and 8 have no issue).

## 3. Project items

- Board: `User Stories Workshop` (project 7, owner `Dhanyacode12`).
- All 6 issues were already on the board after creation. The agent did not run
  `item-add`. The cause (auto-add through the linked repository) was not confirmed.
- Fields set by the agent after PM approval, verified by reading the board back:

| Issue | Status | Work type | Story quality | Risk area |
|---|---|---|---|---|
| #1 | Backlog | Story | Ready | Source quality |
| #2 | Backlog | Story | Ready | Source quality |
| #3 | Backlog | Story | Needs refinement | Human review |
| #4 | Backlog | Story | Draft | Source quality |
| #5 | Backlog | Story | Draft | Source quality |
| #6 | Backlog | Story | Draft | Human review |

## 4. Commands and tools used

| Command | Effect |
|---|---|
| `brew --version` | Read-only check |
| `brew install gh` | **Installed software** (GitHub CLI 2.102.0); Homebrew also ran routine cache cleanup |
| `gh auth status` | Read-only |
| `gh project list/view/item-list/field-list` | Read-only |
| `gh label list`, `gh issue list` | Read-only |
| `gh issue create` x6 | **Created 6 issues** |
| `gh project item-edit` x18 | **Set 3 fields on 6 items** |
| `git remote -v`, `git status` | Read-only |

Done by the PM, not the agent: `gh auth login` and `gh auth refresh -s project`
(browser login), creating the project, columns, and fields in the browser.
The login flow also registered an SSH key on the PM's GitHub account (chosen by
the PM during the prompts).

## 5. Assumptions still unvalidated

- Which documents count as approved, and who maintains the list (Stories 1, 6).
- Who owns the policy content (Story 2).
- Who reviews flags and how fast (Story 3).
- That a "policy owner" role exists (Story 6).
- Whether agents send answers by copy or by a send button (Story 7).
- What to measure for pilot success, and the latency target (Stories 4, 8; no issue yet).
- Why issues were auto-added to the board.

## 6. Risks and weak stories to revisit

- **Story 3:** weak on Small and Estimable. The PM chose to keep it whole.
- **Story 7:** may overlap with Story 1's purpose (verify before replying).
- **Story 6:** depends on an assumed role.
- **Stories 4 and 8:** have no GitHub issue, but still exist in the local files.
  The local backlog and GitHub now differ on purpose; decide whether to keep or delete them.
- **Gaps not covered by any story:** logging, privacy, monitoring, accessibility.
- **Legal disclaimer wording:** out of scope by PM decision; it is a dependency on the legal team.
- **Agent overreach to note:** the agent added four stories (5-8) because the approved
  prompt said "at least four more". The PM had not asked for new stories and kept
  them as drafts. Future prompts should say so explicitly.

## 7. Deferred for human approval (not done)

- Committing and pushing the new files.
- Moving any issue to the Ready column (PM chose to keep everything in Backlog).
- Creating issues for Stories 4 and 8 (PM removed them from the plan).
- Remaining undecided rows in `ai-collaboration-log.md`: epic grouping,
  draft DoR/DoD, suggested out-of-scope items.
- Deciding the suggested out-of-scope items (no unreviewed customer answers,
  no unapproved sources).
- Agreement on `ready-done-agreements.md` with the real team.

## 8. What the PM corrected or rejected

- Rejected 8 of 10 critique suggestions (1.1, 1.2, 2.1, 2.2, 3.1, 3.2, 3.3, 4.1).
  Reasons recorded for 3.1 and 4.1.
- Removed Stories 4 and 8 from the GitHub plan.
- Changed Story 2's risk area from Human review to Source quality.
- Questioned the agent's addition of Stories 5-7.
