# AI Strategy One-Pager - Juno Automated Prioritization

## 1. Problem & Workflow

The problem: Scattered feedback loops leads to poor prioritization. 
Prevention: By giving product managers the information to make strategic decisions and sell those decisions to business stakeholders. 

## 2. Target Metrics

Count of priority 1 escalations reduced to <2 per week. Average time to resolution for all tickets per week reduced by 50%.

## 3. Autonomy Level

Hybrid RAG+Agentic with copilot for dashboard draft review by PM before publishing to stakeholders. 
Need more than a Reactive Assist tool to efficiently synthesize the data. Would not use LLM to reason the feedback independently due to the critical nature. 

## 4. Data & Model Approach

Ground (RAG) in customer data citing specific sources from Jira and Slack to identify common themes and patterns in the dates/times being reported to provide insights for triaging teams.

## 5. Risks & Mitigations

A standalone customer could file multiple complaints that lead to a false impression of criticality.

## 6. V1 Scope

In: Both customer escalations and slack threads which mix customer complaints and feedback or ideas.
Out: (1) cross-reference PII of the customer making claims, (2) attempt to resolve or suggest resolutions. Both require human judgment in priority, business system architecture, and scope tradeoffs.  
