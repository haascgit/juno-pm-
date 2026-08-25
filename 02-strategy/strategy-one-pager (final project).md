# AI Strategy One-Pager - Juno Automated Prioritization

## 1. Problem & Workflow

Watchlist Product Recaps
Problem: Customer engagement with the Watchlist has fallen off, as competitors offer similar products.
Prevention: Using our proprietary information and data sources, introducing a recap feature briefs customers on market moves that matter to them, and will keep them engaging weekly.

## 2. Target Metrics

Increase weekly active Watchlist users by 30%. 

## 3. Autonomy Level

Choice: Agent for speed and scale. Explicitly avoiding feedback loops that add time and cost. 

## 4. Data & Model Approach

Ground (RAG) for market data accuracy and proprietary watchlist and news content. 
Explicitly avoiding: generic LLM (Buy). Using a general model without RAG grounding would lead to hallucinations of market movements that might contradict the internal data or proprietary news.

## 5. Risks & Mitigations

Risk: if the data volatility is high during the week, the AI might output contradictory summaries between the data and the news.

## 6. V1 Scope

In: Watchlist with publicly traded stocks on NYSE and Nasdaq stock exchanges.
Out: (1) Global market coverage, (2) non-stock asset types (cryptocurrencies, bonds, funds, futures)
