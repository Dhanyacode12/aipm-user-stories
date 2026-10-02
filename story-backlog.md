# Story Backlog: Policy Assistant Pilot

Scenario: an internal AI assistant helps support agents find answers in
**approved policy documents only**. Pilot target: four weeks.

Status: **Draft**. Stories 1-4 were written by the PM (Phase 1) and reviewed in
Phase 2. Stories 5-8 are **agent-drafted proposals** and must be accepted,
edited, or rejected by the PM. No user research or business evidence has been
invented; anything unknown is marked as an open question or assumption.

Epic key: see [epic-map.md](epic-map.md).

---

## Story 1: Show the source of every answer

**Epic:** A, Trustworthy answers | **Work type:** Story | **Author:** PM

**Story**
As a support agent,
I want each answer to show its source policy and section,
so that I can verify it before I reply to a customer.

**Acceptance criteria**
- Every answer shows the policy title and section it came from.

(The "no source found" rule lives in Story 2, so it was removed here.)

**Open question**
- Which documents count as approved?

**Risk / assumption**
- Assumption: the policy documents are up to date.

---

## Story 2: Tell the agent when no approved answer exists

**Epic:** A, Trustworthy answers | **Work type:** Story | **Author:** PM

**Story**
As a support agent,
I want to be told when no approved answer exists,
so that I don't guess and can pass the question to someone who can help.

**Acceptance criteria**
- When no approved source is found, the assistant shows "No approved answer found."
- When no approved source is found, the assistant does not give an answer or guess.

**Open questions**
- Are the most common questions answered in the policy?
- Who owns the policy, and should it be updated?

**Risk / assumption**
- Risk: the assistant guesses and the agent repeats a wrong answer to a customer.

---

## Story 3: Flag a wrong or unclear answer

**Epic:** C, Humans stay in the loop | **Work type:** Story | **Author:** PM

**Story**
As a support agent,
I want to flag a wrong or unclear answer,
so that it gets reviewed before it reaches a customer again.

**Acceptance criteria**
- A support agent can flag any answer with one click, and it goes to a reviewer.
- A flagged answer shows as "under review" until a reviewer responds.

**Open question**
- Who reviews flagged answers, and how fast?

**Risk / assumption**
- Risk: nobody reviews the flags, so the same wrong answer keeps appearing.

**INVEST note (own review)**
- Weak on **S (Small)**: bundles three jobs (flagging, reviewing, "under review"
  label). The PM chose to keep it as one story.
- Weak on **E (Estimable)**: review time is unknown.

---

## Story 4 (draft): Evidence that the pilot saves time

**Epic:** D, Prove the pilot's value | **Work type:** Story | **Author:** Agent placeholder (PM accepted)

Status: **Draft placeholder**. Acceptance criteria and metrics are **not
defined**; stakeholders must decide what to measure. No numbers invented.

**Story**
As a product lead,
I want evidence on whether the assistant saves time without raising answer risk,
so that I can decide whether the pilot should continue.

**Acceptance criteria**
- To be defined with stakeholders.

**Open question**
- What should be measured, and who decides the success threshold?

---

## Story 5 (agent draft): Ask a policy question in my own words

**Epic:** A, Trustworthy answers | **Work type:** Story | **Author:** Agent proposal, needs PM decision

**Story**
As a support agent,
I want to ask a policy question in my own words and get an answer drawn from approved documents,
so that I can reply to customers faster.

**Acceptance criteria**
- A typed question returns an answer based only on approved documents.
- A question with no matching approved document follows the behavior in Story 2.

**Open questions**
- Which questions will be used to test this (the agreed pilot test questions)?
- In what language(s) will agents ask?

**Risk / assumption**
- Assumption: the approved documents actually contain answers to common questions.

---

## Story 6 (agent draft): Only approved documents are searchable

**Epic:** B, Approved sources | **Work type:** Story | **Author:** Agent proposal, needs PM decision

**Story**
As a policy owner (assumed role),
I want only approved policy documents to be searchable,
so that the assistant never cites an unapproved source.

**Acceptance criteria**
- Only documents on the approved list can appear as sources.
- A document removed from the approved list no longer appears as a source.

**Open questions**
- Who maintains the approved list?
- Does the "policy owner" role exist in this organization?

**Risk / assumption**
- Risk: the approved list goes stale and outdated documents keep being cited.

---

## Story 7 (agent draft): Answers stay drafts until the agent sends them

**Epic:** C, Humans stay in the loop | **Work type:** Story | **Author:** Agent proposal, needs PM decision

**Story**
As a support agent,
I want the assistant's answer to stay a draft that I send myself,
so that no unchecked answer reaches a customer automatically.

**Acceptance criteria**
- The assistant never sends an answer to a customer on its own.
- Each answer is labeled as a draft until the agent sends it.

**Open question**
- Do agents copy the answer, or is there a send button in the support tool?

**Risk / assumption**
- Risk: agents paste drafts to customers without checking them.

---

## Story 8 (agent draft): Fast enough to use during a conversation

**Epic:** D, Prove the pilot's value | **Work type:** Requirement (non-functional) | **Author:** Agent proposal, needs PM decision

**Story**
As a support agent,
I want results to appear fast enough to use during a customer conversation,
so that the tool saves time instead of costing it.

**Acceptance criteria**
- Results appear within the agreed internal latency target.
- The target is measured using pilot data.

**Open question**
- What is the latency target? (Not invented here; stakeholders must set it.)

**Risk / assumption**
- Assumption: a realistic target can be agreed within the four-week pilot.

---

## Scope

**Out of scope for the pilot**
- Writing legal disclaimer wording (handled by the legal team; legal review is a
  dependency, not a story in this backlog).

**Suggested for PM approval (not yet decided)**
- Generating final customer-facing answers without human review.
- Searching unapproved document sources.

---

## Assumptions needing human validation

- Which documents count as approved, and who maintains the list (Stories 1, 6).
- Who owns the policy content (Story 2).
- Who reviews flags and the expected response time (Story 3).
- What to measure for the pilot and the success threshold (Story 4).
- That a policy owner role exists (Story 6).
- Whether agents send answers by copying or by a send button (Story 7).
- The latency target (Story 8).
