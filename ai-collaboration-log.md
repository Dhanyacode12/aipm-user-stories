# AI Collaboration Log

Records what the AI suggested and what I decided.

| Prompt or request | Accepted | Edited | Rejected | Reason |
|---|---|---|---|---|
| Story 1: reword "the AI should show the source" to "I want each answer to show its source" | X |  |  | The "I want" should state the agent's need, not an instruction to the system |
| Story 1: make the WHY "so that I can verify it before I reply to a customer" | X |  |  | Says what the agent does with the source |
| Story 1: make criterion 2 testable ("no approved source found, says so and gives no answer") | X |  |  | "Correctly mentioned" was too fuzzy to check |
| Story 2: change WHY from "add the answer in the policy" to "so I don't guess and can pass it on" | X |  |  | Editing policy may not be the agent's job; the WHY should describe the moment of use |
| Story 2: rewrite "give a clear message" as the exact text "No approved answer found." | X |  |  | "Clear" is a fuzzy word; exact text is checkable |
| Story 2: rewrite "does not give a wrong answer" as "does not give an answer or guess" | X |  |  | Write rules about behavior, not about results that cannot be checked |
| Story 3: replace "all answers verified by the agent" with a flagging criterion | X |  |  | The original was a different, oversized story |
| Story 3: replace "why does AI give wrong answers" with "who reviews flags, and how fast?" | X |  |  | The original was not about this story |
| Story 3: sharpen risk to "nobody reviews the flags" | X |  |  | Ties the risk to this workflow |
| Story 3: split into 3a / 3b / 3c because it is not Small | X |  |  | INVEST: bundles three jobs; review time unknown |
| Critique 1.1: add criterion that the agent can open the cited section |  |  | X | No reason given yet |
| Critique 1.2: show last-updated date on the source |  |  | X | No reason given yet |
| Critique 1.3: remove duplicate "no source" criterion from Story 1 | X |  |  | It already lives in Story 2 |
| Critique 2.1: add escalation target to the "no answer" message |  |  | X | No reason given yet |
| Critique 2.2: log "no answer" cases |  |  | X | No reason given yet |
| Critique 3.1: split Story 3 into 3a / 3b / 3c |  |  | X | Splitting would not fix the unknown review time (E) |
| Critique 3.2: flag records who, what, and when |  |  | X | No reason given yet |
| Critique 3.3: reword Story 3 WHY |  |  | X | No reason given yet |
| Critique 4.1: add a legal disclaimer story |  |  | X | Legal wording is outside my scope |
| Critique 4.2: add a placeholder story for pilot evidence | X |  |  | Scenario requires evidence of time saved; metrics left open |
| Phase 4: Story 5, ask a policy question in my own words | X |  |  | Kept as a draft to reach the handout's eight stories. I had not asked for new stories; the prompt I approved said to add at least four. |
| Phase 4: Story 6, only approved documents are searchable (assumes a "policy owner" role) | X |  |  | Kept as a draft (same reason). The "policy owner" role is an assumption to validate. |
| Phase 4: Story 7, answers stay drafts until the agent sends them | X |  |  | Kept as a draft (same reason). May overlap with Story 1. |
| Phase 4: Story 8, fast enough to use during a conversation (latency target left open) | X |  |  | Kept as a draft (same reason). Target left blank on purpose. |
| Phase 4: epic grouping A-D in epic-map.md |  |  |  |  |
| Phase 4: draft DoR and DoD in ready-done-agreements.md |  |  |  |  |
| Phase 4: suggested out-of-scope items (no unreviewed customer answers, no unapproved sources) |  |  |  |  |

## One example where I corrected or rejected the agent

Rejected 4.1 (legal disclaimer story): legal wording is not in my scope, so I
do not write a story for it. The scenario's legal-review constraint stays a
dependency on the legal team.

## Notes

- The agent must not invent user research or business evidence.
- Assumptions that still need human validation are listed in `story-backlog.md`.
