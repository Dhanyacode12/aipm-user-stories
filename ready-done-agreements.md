# Ready and Done Agreements

**Status: draft.** To become real, the team must discuss and agree on these. Start
small and revise after the pilot checkpoint.

Priority key: **Now** (required immediately), **Soon**, **Later**.

---

## Definition of Ready (DoR): "Can we start?"

DoR is a team agreement, not a Scrum requirement. Use it to expose missing
context early, not as a wall. **Discovery stories** (for example Story 4, whose
metrics are unknown) are exempt and may start before they are fully ready.

| Priority | Criterion | Example of "met" |
|---|---|---|
| Now | Role, goal, and benefit are written | "As a support agent, I want ..., so that ..." with a real role |
| Now | Acceptance criteria are written | At least one rule that can be checked with yes or no |
| Now | Open questions and risks are visible | Listed under the story |
| Now | Small enough for the delivery cycle | Can be finished within the four-week pilot window |
| Soon | Major dependencies are known | "Needs the approved document list from the policy owner" |
| Soon | Enough context to estimate the work | The team can say roughly how long it takes |
| Later | Designs, data, or source materials are available | Approved documents provided |

## Definition of Done (DoD): "Are we finished?"

DoD applies to **every** story. Acceptance criteria belong to one story; DoD
applies to all.

| Priority | Criterion | Example of "met" (evidence) |
|---|---|---|
| Now | Acceptance criteria are met | Each criterion checked and ticked on the issue |
| Now | Work is reviewed | A teammate checks it against the acceptance criteria and writes "approved" or "changes needed" on the issue |
| Soon | Known limitations are recorded | Listed on the issue |
| Soon | Affected people are informed | Team told in the project channel |
| Later | Privacy, security, or accessibility checks done | Checklist attached |

### Extra DoD items for AI work

| Priority | Criterion | Example of "met" (evidence) |
|---|---|---|
| Now | Only approved data sources are used | Source list checked against the approved list |
| Now | Fallback behavior is tested | Tested a question with no answer; "No approved answer found." shown |
| Soon | Human escalation path works | A flagged answer reached a reviewer |
| Soon | Outputs reviewed against agreed examples | Compared with the agreed test questions |
| Soon | Evaluation results are labeled | Marked as pilot, mock, or validated |
| Later | Prompt or model changes are documented | Change note written |

## Board mapping

- **Ready** column = story passed the DoR.
- **Done** column = story passed the DoD.
- Field **Story quality**: Draft, Needs refinement, Ready.

## Pitfalls to avoid

- Too many criteria: keep this first version minimal.
- DoD without evidence: every "Now" item has an example of proof.
- No revision loop: revisit after the next checkpoint.
- DoR as a wall: discovery stories are exempt.
