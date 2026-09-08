# AI Solution Decision Matrix · Juno

## The decision

Whether RocketShip builds a dashboard for the PM to synthesize bugs and features in Juno as a Hybrid (RAG + Agentic) Copilot, vs buying a generic LLM API or fine-tuning a model on our corpus.

Why now: critical bugs and valuable feedback to inform features are getting lost, costing the product manager time and the business opportunity cost and customer churn.

## Options scored

| Option | Cost | Speed | Control | Moat | Risk | Score |
|---|---|---|---|---|---|---|
| Build | 2 | 2 | 5 | 5 | 4 | 3.6 |
| Buy / API | 1 | 5 | 1 | 1 | 2 | 2.0 |
| Fine-tune | 2 | 2 | 4 | 4 | 3 | 3.0 |

## Recommendation

Build. Highest score because Control and Risk of sensitive data matter for a system of trust. A Buy faster, but it cannot cite RocketShip sources critical for usability. Fine-tune is slower than we can wait and still needs the corpus Juno would retrieve live. Autonomy stays Copilot: Juno drafts the ranked backlog with citations; the PM approves before publish.
