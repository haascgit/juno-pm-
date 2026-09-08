## Harness architecture (Juno PM)

**Archetype: Tool-using copilot**

Real actions are needed and a human is close enough to confirm the consequential ones. This is where most 2026 PM products belong.

| Surface | Setting |
|---|---|
| 01 Context | Name the required sources explicitly and fail loudly when one is unreachable. |
| 02 Tools | Only the verbs this task needs. Omissions documented. |
| 03 Loop | Ceiling of 10 to 25, with a hard cost ceiling per task turns. Escalate after 3 consecutive failures or 80% of the cost ceiling. Target p95 not user-facing, budget on cost instead. |
| 04 Memory | Persist the rationale for the current cycle. Expire on the next one. |
| 05 Permissions | read auto, draft auto, write confirm, send blocked in V1 |
| 06 Verification | Automated check on the machine-checkable part, plus a source citation on the rest. On failure: Block on the checkable failure. Label the rest unverified. |

### Drivers

- **Blast radius**: Customers see it
- **Recoverability**: Trivially, one click
- **Verifiability**: Partly checkable
- **Repetition**: Weekly-ish
- **Latency budget**: Async / overnight
