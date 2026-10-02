# Acceptance Criteria

All criteria in one place. Each is a rule a stranger could check with yes or no.
Details and context are in [story-backlog.md](story-backlog.md).

| Story | Acceptance criteria | Status |
|---|---|---|
| 1. Show the source | Every answer shows the policy title and section it came from. | PM-written |
| 2. No approved answer | When no approved source is found, the assistant shows "No approved answer found." | PM-written |
| 2. No approved answer | When no approved source is found, the assistant does not give an answer or guess. | PM-written |
| 3. Flag an answer | A support agent can flag any answer with one click, and it goes to a reviewer. | PM-written |
| 3. Flag an answer | A flagged answer shows as "under review" until a reviewer responds. | PM-written |
| 4. Pilot evidence | To be defined with stakeholders. | Draft placeholder |
| 5. Ask in my own words | A typed question returns an answer based only on approved documents. | Agent draft |
| 5. Ask in my own words | A question with no matching approved document follows Story 2. | Agent draft |
| 6. Approved documents only | Only documents on the approved list can appear as sources. | Agent draft |
| 6. Approved documents only | A document removed from the approved list no longer appears as a source. | Agent draft |
| 7. Drafts stay drafts | The assistant never sends an answer to a customer on its own. | Agent draft |
| 7. Drafts stay drafts | Each answer is labeled as a draft until the agent sends it. | Agent draft |
| 8. Fast enough | Results appear within the agreed internal latency target. | Agent draft (target TBD) |
| 8. Fast enough | The target is measured using pilot data. | Agent draft |

## Notes

- Story 4 has no criteria on purpose: what to measure is a stakeholder decision.
- Story 8's latency target is intentionally not filled in; no number was invented.
- Criteria about model behavior vs. human workflow:
  - Model behavior: Stories 1, 2, 5, 6
  - Human workflow: Stories 3, 7
  - Quality requirement: Story 8
