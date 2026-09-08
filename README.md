# Watchlist Recaps Weekly

> You are an expert research analyst who turns complex data into concise summaries. Your job is to give customers a quick summary explaining the weekly performance of their list, what moved (based on data query) and why (published articles).

_Crystal Haas - #ai-product-management-aug17-26-weeknights_

Repo: https://github.com/haascgit/juno-pm-

This repo is my final project for the AI Product Management Certification — **Watchlist Recaps Weekly**. Each module’s artefact lives in its own folder; this README is the dashboard and the pitch.

---

## Module artefacts

### M1 · Prompting
- **System prompt** — [`01-prompting/system-prompt.md`](01-prompting/system-prompt.md)
- **Prototype** — https://lovable.dev/projects/7b253e9d-f843-4a45-b1a6-d4154b837a41?magic_link=mc_bc879035-0b08-4e05-92e5-eb861cf7beb9

### M2 · Strategy
- **Decision matrix** — [`02-strategy/decision-matrix.md`](02-strategy/decision-matrix.md)
- **AI Strategy one-pager** — [`02-strategy/strategy-one-pager.md`](02-strategy/strategy-one-pager.md)

### M3 · RAG / AI PRD
- **AI PRD** — [`03-rag-prd/prd.md`](03-rag-prd/prd.md)

### M4 · AI-Native UX
- **AI user flow** — [`04-ai-ux/user-flow.md`](04-ai-ux/user-flow.md)
- **Trust-gap mitigations** — [`04-ai-ux/trust-gaps.md`](04-ai-ux/trust-gaps.md)

### M5 · Agentic Workflows
- **Agent Workflow Spec (AWSpec)** — [`05-agentic-workflows/awspec.md`](05-agentic-workflows/awspec.md)
- **Agent Control Panel** — [`05-agentic-workflows/agent-control-panel.md`](05-agentic-workflows/agent-control-panel.md)

### M6 · Evals &amp; Guardrails
- **Eval stack** — [`06-evals/eval-stack.md`](06-evals/eval-stack.md)
- **Human evaluation rubric** — [`06-evals/human-rubric.md`](06-evals/human-rubric.md)

---

## PM Execution Plan

### Where Juno is today
- M1–M6 specified and committed.
- Automated evals: 300-item golden set drafted, judge prompt validated against 6 week trial period; not yet wired to CI.
- Human rubric drafted; 2 grader candidates + 1 engineer support lined up; no calibration round yet.

### What ships next (next 2 sprints)
- Sprint 1: wire the eval harness to CI; confirm engineering alignment to RAG data connectivity and frontend display.
- Sprint 2: wire up thumbs down report, reviewal and feedback process for daily report, and initial manage of weekly process.

### What I watch (dashboards)
- Daily: thumbs-down rate, regen rate, hand-off rate.
- Weekly: human-rubric mean per dimension; refusal hit-rate; cost per run.
- Per release: golden-set accuracy; format/citation/refusal pass rate.

### Red lines (what blocks shipping)
- Any critical-safety fail (any "1" on safety dimension in human eval).
- <90% golden-set accuracy on automated layer.
- Customer-name fabrication in last 30 days.
- Cost >$0.07 per run.
- P95 latency >3s on triage flow.

### Governance
- Compliance: PII scrubber pre-LLM.
- Safety: prompt-injection eval row in golden set; refusal on data mismatch content.
- Reliability: 99.5% SLO; not displayed if model is down.
- Reputation: 2-hour incident-response playbook in /docs; fallback to no display.

---

## Build Insights

- **Friction point.** RAG retrieval of data matters more than the display — model summarization accuracy assumes that backend data returned from the GraphQL query is correct.
- **Key learning.** Clear hallucinations can be made if the strategy doc is not provided for context; and this is more important than detailed requirements.
- **Aha moment.** Writing detailed/thorough requirements for a AI agent may cause more harm than good (too rigid for usefulness, hard to change later, hides errors, amplifies hallucinations).

---

_Certification submission — AI Product Management Certification._
