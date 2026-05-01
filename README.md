# Negotiation-Theoretic Frameworks for Human-AI Price Discovery

Supplementary materials for the ICIS 2026 short paper of the same title.

> Repository is private during blind review. Will be made public (with an
> anonymized snapshot URL for reviewers) at submission.

---

## About

This repository accompanies an ICIS 2026 short paper on **AI-assisted reserve price discovery for collector and enthusiast vehicles** (Bring a Trailer auctions).

An LLM guide (Claude Opus-4.7) produces an initial reserve estimate P<sub>5</sub> by aggregating four upstream signals — **P<sub>1</sub>**, a six-month exact-match market average (Classic.com); **P<sub>2</sub>**, a *k*-NN price estimate over matched features; **P<sub>3</sub>**, a trained mixture-of-experts model; and **P<sub>4</sub>**, a peer LLM (Gemini 3.1 Pro) with database access. A second LLM (GPT-5.5) playing the platform operator then engages the guide in a multi-turn conversation to stress-test P<sub>5</sub> — without proposing a number of its own. We vary the operator's interaction strategy between two conditions drawn from classical bargaining theory:

- **Distributive (D)** — adversarial questioning; demands evidence for every claim.
- **Integrative (I)** — collaborative exploration; decomposes value across dimensions.

The guide may revise P<sub>5</sub> in response to evidence the operator surfaces. The terminal value P<sub>5</sub>\* is compared against the realized auction price.

---

## Contents

### Architecture

- [P<sub>3</sub> — Mixture of Experts Attention-based model](./architecture/README.md)

### Examples

- [Examples index](./examples/README.md)
- [1986 Alfa Romeo Spider (Series 3)](./examples/1986_alfa_romeo_spider.md)
- [1986 Chevrolet Corvette (C4)](./examples/1986_chevrolet_corvette_c4.md)
- [2009 BMW 135i (E8x)](./examples/2009_bmw_135i.md)
- [2019 Ford Shelby GT350R (S550)](./examples/2019_ford_shelby_gt350r.md)
- [1996 Land Rover Defender 90 (L316)](./examples/1996_land_rover_defender_90.md)

### Prompts

- [Prompts index](./prompts/README.md)
- [Guide — `guide_v5.txt`](./prompts/guide/guide_v5.txt)
- [Operator (distributive) — `distributive_v5a.txt`](./prompts/operator/distributive_v5a.txt)
- [Operator (integrative) — `integrative_v5a.txt`](./prompts/operator/integrative_v5a.txt)
- [P<sub>5</sub> synthesis (no search) — `p5_no_search_v3.txt`](./prompts/p5/p5_no_search_v3.txt)
- [P<sub>5</sub> synthesis (with web search) — `p5_with_search_v5b.txt`](./prompts/p5/p5_with_search_v5b.txt)
- [P<sub>4</sub> with database tools — `p4_with_tools.txt`](./prompts/p4/p4_with_tools.txt)

### Post-Hoc Analysis

- [Comparing web-search capability for P5](./post_hoc/README.md)
---

## License

Content is licensed under [Creative Commons Attribution 4.0 International](./LICENSE)
(CC-BY 4.0).
