# Epic Map: Policy Assistant Pilot

Traceability from initiative to epic to story.

**Initiative:** Improve internal policy-support workflows.

```text
Initiative: Improve internal policy-support workflows
|
+-- Epic A: Let support agents find trustworthy policy answers
|     +-- Story 1: Show the source of every answer
|     +-- Story 2: Tell the agent when no approved answer exists
|     +-- Story 5: Ask a policy question in my own words   (agent draft)
|
+-- Epic B: Keep policy sources approved
|     +-- Story 6: Only approved documents are searchable  (agent draft)
|
+-- Epic C: Keep humans in the loop
|     +-- Story 3: Flag a wrong or unclear answer
|     +-- Story 7: Answers stay drafts until the agent sends them  (agent draft)
|
+-- Epic D: Prove the pilot's value
      +-- Story 4: Evidence that the pilot saves time      (draft placeholder)
      +-- Story 8: Fast enough to use during a conversation (agent draft, Requirement)
```

| Epic | Goal | Stories | AI needs covered |
|---|---|---|---|
| A | Let support agents find trustworthy policy answers | 1, 2, 5 | Source traceability, fallback behavior |
| B | Keep policy sources approved | 6 | Approved data sources |
| C | Keep humans in the loop | 3, 7 | Human review, escalation |
| D | Prove the pilot's value | 4, 8 | Latency, evidence of results |

## Known gaps (from the lesson 03 list of AI needs)

Not covered by any story yet, and not invented here:
- Logging and auditability
- Privacy and data minimization
- Monitoring
- Accessibility and usability

These are open questions for stakeholders, not decisions.

## Board fields

| Work type | Count |
|---|---|
| Epic | 4 |
| Story | 7 (Stories 1-7) |
| Requirement | 1 (Story 8) |
