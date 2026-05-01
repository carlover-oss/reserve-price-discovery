# Prompts

The LLM system prompts used in the study.

## What each prompt does

| File | Role |
|---|---|
| [`guide/guide_v5.txt`](./guide/guide_v5.txt) | The Guide. Holds P<sub>5</sub> and revises it during the dialogue in response to evidence the operator surfaces. Receives P<sub>1</sub>–P<sub>4</sub> as scalars; has no tool access during the dialogue. |
| [`operator/distributive_v5a.txt`](./operator/distributive_v5a.txt) | The distributive operator. Audits P<sub>5</sub> through pointed, evidence-demanding questioning. Does not propose a price. |
| [`operator/integrative_v5a.txt`](./operator/integrative_v5a.txt) | The integrative operator. Engages the guide collaboratively, sharing listing details and decomposing value across dimensions. Does not propose a price. |
| [`p5/p5_no_search_v3.txt`](./p5/p5_no_search_v3.txt) | P<sub>5</sub> synthesis. The guide aggregates P<sub>1</sub>–P<sub>4</sub> into a single estimate. No external retrieval. |
| [`p5/p5_with_search_v5b.txt`](./p5/p5_with_search_v5b.txt) | P<sub>5</sub> synthesis with web search. The guide may issue web searches during this synthesis call (no fixed cap on the number of searches). VIN- and date-based leakage guards are enforced at both prompt and platform level. After the call returns, the guide has no further search access. |
| [`p4/p4_with_tools.txt`](./p4/p4_with_tools.txt) | P<sub>4</sub>. A peer LLM that queries the platform database via two tools to produce a free-form valuation. |

## Substitution tokens

Several prompts contain placeholders the orchestrator fills in per-car at
runtime:

| Token | Substituted with |
|---|---|
| `${P5}` | The Guide's current P<sub>5</sub> in dollars |
| `${P1}` … `${P4}` | The four scalar signals |
| `${VIN}` | The test car's VIN |
| `${SALE_DATE}` | The car's auction-clearing date |
