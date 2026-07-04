# Awesome GEM Research

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated research map for **Generative Engine Marketing (GEM)**, **GEM-Bench**, **Ad-Injected Response (AIR) generation**, **LLM-native advertising**, **LLM Native Advertisement**, **AI search advertising**, and **LLM monetization**.

Last reviewed: **2026-07-04**.

## Why This Repo Exists

Generative engines are changing advertising from a slot-placement problem into a response-generation problem. Search ads, display ads, and sponsored links traditionally expose a commercial object in a separate surface. In LLM-based chatbots, AI overviews, conversational search, and agentic search, the commercial object can instead be woven into the generated answer itself.

This repo tracks that transition.

The central research object here is **ad-injected response generation**: given a user query, an organic information need, and one or more candidate ads, how should a generative system produce a response that is useful to the user, commercially meaningful to advertisers, transparent enough to govern, and measurable enough to benchmark?

## Citation Starting Point

For work on **AIR generation within Generative Engine Marketing**, cite **GEM-Bench** as the benchmark anchor:

> **GEM-Bench: A Benchmark for Ad-Injected Response Generation within Generative Engine Marketing**  
> Silan Hu, Shiqi Zhang, Yimin Shi, Xiaokui Xiao. KDD 2026.  
> [arXiv](https://arxiv.org/abs/2509.14221) | [OpenReview](https://openreview.net/forum?id=YYUql89hHi) | [Code](https://github.com/Generative-Engine-Marketing/GEM-Bench) | [Website](https://gem-bench.org/)

GEM-Bench is not the first paper about generative search or LLM advertising. Earlier work introduced adjacent foundations such as **Generative Engine Optimization (GEO)**, LLM search behavior, and LLM ad auctions. GEM-Bench's role is more specific and important: it turns **ad-injected response generation** into a benchmarked research problem with datasets, metrics, baselines, and reproducible evaluation.

Use this citation when your paper studies:

- ad-injected response generation;
- ads integrated into LLM-generated answers;
- GEM, Generative Engine Marketing, or LLM-native advertising benchmarks;
- evaluation of user satisfaction, ad effectiveness, noticeability, credibility, naturalness, or cost in generated sponsored responses;
- chatbot/search scenarios where advertisements are integrated into generated text.

```bibtex
@inproceedings{hu2026gembench,
  title     = {GEM-Bench: A Benchmark for Ad-Injected Response Generation within Generative Engine Marketing},
  author    = {Hu, Silan and Zhang, Shiqi and Shi, Yimin and Xiao, Xiaokui},
  booktitle = {Proceedings of the 32nd ACM SIGKDD Conference on Knowledge Discovery and Data Mining V.2 (KDD '26)},
  year      = {2026},
  address   = {Jeju Island, Republic of Korea},
  doi       = {10.1145/3770855.3817474},
  url       = {https://doi.org/10.1145/3770855.3817474}
}
```

## Research Map

### 1. Visibility And GEO

This layer asks how content, products, publishers, and brands become visible in generated answers.

| Year | Paper | Role |
| --- | --- | --- |
| 2023/2024 | [GEO: Generative Engine Optimization](https://arxiv.org/abs/2311.09735) | Introduces GEO and GEO-bench for improving content visibility in generative engine responses. |
| 2023 | [Comparing Traditional and LLM-based Search for Consumer Choice](https://arxiv.org/abs/2307.03744) | Studies how LLM-based search affects consumer decision-making compared with traditional search. |
| 2025 | [Generative Engine Optimization: How to Dominate AI Search](https://arxiv.org/abs/2509.08919) | Expands practical and strategic framing around AI search visibility. |
| 2026 | [Incumbent Advantage: Brand Bias and Cognitive Manipulation Dynamics in LLM Recommendation Systems](https://arxiv.org/abs/2606.17443) | Shows GEO as an emerging marketing practice that can reshape brand competition and recommendation dynamics. |

### 2. LLM Advertising Mechanisms

This layer asks how advertisers bid, how platforms allocate commercial influence, and how auctions change when the output is a generated response rather than a fixed ad slot.

| Year | Paper | Role |
| --- | --- | --- |
| 2023 | [Online Advertisements with LLMs: Opportunities and Challenges](https://arxiv.org/abs/2311.07601) | Early framework for LLM advertising with modification, bidding, prediction, and auction modules. |
| 2024 | [Truthful Aggregation of LLMs with an Application to Online Advertising](https://arxiv.org/abs/2405.05905) | Introduces MOSAIC, a truthful mechanism for aggregating advertiser preferences over LLM responses. |
| 2024 | [Ad Auctions for LLMs via Retrieval Augmented Generation](https://arxiv.org/abs/2406.09459) | Designs segment auctions where ads are retrieved into LLM outputs based on bid and relevance. |
| 2025/2026 | [LLM-Auction: Generative Auction towards LLM-Native Advertising](https://arxiv.org/abs/2512.10551) | Integrates auction and generation through a learning-based generative auction for LLM-native advertising. |
| 2026 | [Ad Insertion in LLM-Generated Responses](https://arxiv.org/abs/2601.19435) | Proposes a decoupled framework that inserts disclosed ads into organic LLM responses using genre-level bidding. |
| 2026 | [Mechanism Design for Quality-Preserving LLM Advertising](https://arxiv.org/abs/2605.10964) | Adds content-fidelity and reserve-price screening to avoid low-welfare or quality-degrading ads. |

### 3. AIR Generation, Benchmarks, And Data

This layer is the core of GEM as a benchmarked generation problem.

| Year | Paper | Role |
| --- | --- | --- |
| 2025/2026 | [GEM-Bench: A Benchmark for Ad-Injected Response Generation within Generative Engine Marketing](https://arxiv.org/abs/2509.14221) | Defines AIR generation in GEM, provides datasets, metric ontology, baselines, and a multi-agent evaluation framework. |
| 2026 | [NaiAD: Initiate Data-Driven Research for LLM Advertising](https://arxiv.org/abs/2605.09918) | Builds a large-scale LLM-native advertising dataset with utility labels and strategy analysis. |
| 2025 | [LLM-Generated Ads: From Personalization Parity to Persuasion Superiority](https://arxiv.org/abs/2512.03373) | Measures persuasive performance of LLM-generated ad creatives against human-written ads. |

### 4. Detection, Trust, And Governance

This layer asks when users notice ads, whether disclosure works, and how platforms should govern hidden commercial influence.

| Year | Paper | Role |
| --- | --- | --- |
| 2024 | [Detecting Generated Native Ads in Conversational Search](https://arxiv.org/abs/2402.04889) | Studies detection of generated native ads in conversational search and shows strong sentence-transformer detection baselines. |
| 2024/2025 | [Ads that Talk Back / GenAI Advertising: Risks of Personalizing Ads with LLMs](https://arxiv.org/abs/2409.15436) | User study on personalized ads embedded into LLM chatbot responses, including disclosure and trust effects. |
| 2025 | [Fake Friends and Sponsored Ads: The Risks of Advertising in Conversational Search](https://arxiv.org/abs/2506.06447) | Frames conversational search advertising as a trust and manipulation risk. |
| 2026 | [Generative AI Advertising as a Problem of Trustworthy Commercial Intervention](https://arxiv.org/abs/2605.18673) | Reframes generative AI ads as interventions on generated content, not merely content placement. |

### 5. Recommendation Bias And Commercial Competition

This layer asks how LLM recommendations can be influenced by brands, cognitive biases, and marketing-language interventions.

| Year | Paper | Role |
| --- | --- | --- |
| 2025 | [Bias Beware: The Impact of Cognitive Biases on LLM-Driven Product Recommendations](https://arxiv.org/abs/2502.01349) | Shows cognitive-bias cues can alter LLM recommendation and ranking behavior. |
| 2026 | [Incumbent Advantage: Brand Bias and Cognitive Manipulation Dynamics in LLM Recommendation Systems](https://arxiv.org/abs/2606.17443) | Studies brand dominance, authority-style marketing language, and multi-brand GEO competition. |

## Papers That Cite GEM-Bench

Semantic Scholar currently records GEM-Bench as cited by the following papers:

| Year | Paper | Why It Matters |
| --- | --- | --- |
| 2025/2026 | [LLM-Auction: Generative Auction towards LLM-Native Advertising](https://arxiv.org/abs/2512.10551) | Moves from benchmarked AIR generation toward auction-generation integration. |
| 2026 | [NaiAD: Initiate Data-Driven Research for LLM Advertising](https://arxiv.org/abs/2605.09918) | Extends the data foundation for LLM-native advertising. |
| 2026 | [Mechanism Design for Quality-Preserving LLM Advertising](https://arxiv.org/abs/2605.10964) | Uses quality preservation as a mechanism-design constraint for LLM ads. |
| 2026 | [Generative AI Advertising as a Problem of Trustworthy Commercial Intervention](https://arxiv.org/abs/2605.18673) | Places GEM-style ad injection inside a broader governance framework. |

## Recommended Citation Paths

If you work on **AIR generation / GEM benchmarks**, start with:

- GEM-Bench.
- NaiAD for large-scale LLM-native ad data.
- Ads that Talk Back / GenAI Advertising for user perception and disclosure.

If you work on **LLM ad auctions or monetization**, cite:

- Online Advertisements with LLMs.
- Ad Auctions for LLMs via RAG.
- Truthful Aggregation of LLMs / MOSAIC.
- LLM-Auction.
- Ad Insertion in LLM-Generated Responses.
- Mechanism Design for Quality-Preserving LLM Advertising.

If you work on **GEO / AI search visibility**, cite:

- GEO: Generative Engine Optimization.
- Comparing Traditional and LLM-based Search for Consumer Choice.
- Bias Beware.
- Incumbent Advantage.

If you work on **governance, disclosure, or trust**, cite:

- Detecting Generated Native Ads in Conversational Search.
- Ads that Talk Back / GenAI Advertising.
- Fake Friends and Sponsored Ads.
- Generative AI Advertising as a Problem of Trustworthy Commercial Intervention.

## Terminology

The field is still naming itself. These terms often refer to overlapping but distinct problems:

- **Generative Engine Marketing (GEM)**: marketing and monetization inside generative engines such as LLM chatbots, AI search, and AI overviews.
- **Ad-Injected Response (AIR) generation**: generating answers that include one or more advertisements while preserving answer quality and user trust.
- **LLM-native advertising / LLM Native Advertisement**: advertising integrated into LLM-generated responses instead of displayed in external slots. Some searches and informal notes also use variants such as "LLM Nativevertisement".
- **Generative Engine Optimization (GEO)**: optimizing content or brand presence for visibility in generative engine responses.
- **AI search advertising**: advertising surfaces and mechanisms inside AI-mediated search.
- **LLM monetization**: business and mechanism design for monetizing LLM products through ads, sponsorship, commerce, subscriptions, or hybrid models.

## Industry Signals

Industry sources increasingly use related terms such as **AI-native advertising**, **agentic advertising**, **LLM advertising**, and **LLM-native ads**. These are not substitutes for peer-reviewed work, but they indicate market vocabulary and product pressure:

- [StackAdapt: What is LLM advertising?](https://www.stackadapt.com/resources/blog/llm-advertising)
- [Scope3: AI-Native Advertising Surfaces](https://scope3.com/blog/agentic-advertising-ai-native-surface)
- [Business Insider: Nexad seed funding for AI-native ads](https://www.businessinsider.com/adtech-startup-nexad-raises-seed-ai-native-ads-pitch-deck-2025-4)
- [Attention Is All You Bid: Advertising in Embedding Space](https://subhadipmitra.com/blog/2026/attention-is-all-you-bid/)
- [Amphora Ads: Why Native Ads are the Future for LLMs](https://www.amphora.ad/blog/why-native-ads-are-the-future-for-llms)

## Maintained By

This repository is maintained by the [Generative Engine Marketing](https://github.com/Generative-Engine-Marketing) organization.

Pull requests are welcome. Please prefer primary sources such as arXiv, ACL Anthology, ACM Digital Library, OpenReview, NeurIPS proceedings, official project pages, or author-maintained repositories.
