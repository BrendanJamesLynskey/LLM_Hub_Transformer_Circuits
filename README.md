# The Transformer Circuits Thread

Anthropic's **mechanistic interpretability** research &mdash; the line of work published at [transformer-circuits.pub](https://transformer-circuits.pub/) that reverse-engineers what is actually happening inside a transformer &mdash; presented for engineers. Six deep-dive decks trace one continuous arc: from the linear-algebra framework that turned attention into something you can read off the weights, through superposition and the dictionary-learning breakthrough that resolves it, up to tracing the step-by-step computation of a deployed Claude model. Each deck takes a single landmark publication and answers three questions &mdash; *what problem it solves*, *what the core mechanism is*, and *why it matters to someone building and operating LLM/agent systems* &mdash; with hand-drawn diagrams of the key idea.

**Live index:** https://brendanjameslynskey.github.io/LLM_Hub_Transformer_Circuits/

## Presentations in this series

| # | Title | Status | Publication covered |
|---|-------|--------|---------------------|
| 01 | [A Mathematical Framework for Transformer Circuits](https://brendanjameslynskey.github.io/Circuits_01_Mathematical_Framework/) | live | Elhage, Nanda, Olsson et al., Anthropic (Dec 2021) &mdash; the residual stream, QK/OV circuits, path expansion, and how composition in two-layer models produces induction heads. |
| 02 | [In-context Learning &amp; Induction Heads](https://brendanjameslynskey.github.io/Circuits_02_Induction_Heads/) | live | Olsson, Elhage, Nanda et al., Anthropic (Mar 2022) &mdash; the phase change in training where induction heads form, and the evidence they are the primary mechanism behind in-context learning. |
| 03 | [Toy Models of Superposition](https://brendanjameslynskey.github.io/Circuits_03_Toy_Models_of_Superposition/) | live | Elhage, Hume, Olsson et al., Anthropic (Sep 2022) &mdash; features as directions, how networks pack more features than neurons via sparsity, the geometry of superposition, and why neurons are polysemantic. |
| 04 | [Towards Monosemanticity](https://brendanjameslynskey.github.io/Circuits_04_Towards_Monosemanticity/) | live | Bricken, Templeton, Batson et al., Anthropic (Oct 2023) &mdash; sparse autoencoders decompose a one-layer model into thousands of interpretable, causal features; feature splitting and universality. |
| 05 | [Scaling Monosemanticity](https://brendanjameslynskey.github.io/Circuits_05_Scaling_Monosemanticity/) | live | Templeton, Conerly, Batson et al., Anthropic (May 2024) &mdash; SAEs scaled to Claude 3 Sonnet; millions of abstract multimodal features, safety-relevant features, feature steering and "Golden Gate Claude". |
| 06 | [On the Biology of a Large Language Model](https://brendanjameslynskey.github.io/Circuits_06_Biology_of_an_LLM/) | live | Lindsey, Ameisen, Batson et al., Anthropic (Mar 2025) &mdash; circuit tracing with cross-layer transcoders and attribution graphs; multi-step reasoning, poem planning, multilingual circuits, arithmetic, hallucination and unfaithful chain-of-thought in Claude 3.5 Haiku. |

## How to read this series

The six decks are chronological and build on one another &mdash; the framework (01) gives the vocabulary; induction heads (02) are the first real circuit found with it; superposition (03) explains why interpretation is hard; dictionary learning (04) and its scaling to a production model (05) resolve superposition into readable features; and circuit tracing (06) uses those features to watch a deployed model think. Each deck also stands alone.

## Where this fits

Part of the [LLMs hub](https://github.com/BrendanJamesLynskey/LLMs) &mdash; an index of presentation series for AI/LLM engineers. Complements the [Key LLM Publications](https://github.com/BrendanJamesLynskey/LLM_Hub_Key_Publications) series (which covers the broader paper canon, including Anthropic's Constitutional AI, Sleeper Agents, Building Effective Agents and MCP) and the [Safety, Alignment &amp; Red-Teaming](https://github.com/BrendanJamesLynskey/LLM_Hub_Safety_Alignment) hub.
