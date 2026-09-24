<a id="readme-top"></a>

<div align="center">

<h1>Awesome Recursive Self-Improvement (RSI)</h1>

<strong>A taxonomy-first, auditable map of recursive self-improvement research.</strong>

<p>
  <a href="#paper-catalog"><img alt="Papers" src="https://img.shields.io/badge/papers-521-2563eb?style=flat-square"></a>
  <a href="https://arxiv.org/abs/2609.11873"><img alt="Companion survey" src="https://img.shields.io/badge/Companion%20Survey-arXiv%3A2609.11873-b31b1b?style=flat-square&amp;logo=arxiv&amp;logoColor=white"></a>
  <a href="#taxonomy-at-a-glance"><img alt="Taxonomy" src="https://img.shields.io/badge/taxonomy-L1--L5-7c3aed?style=flat-square"></a>
</p>

<p>
  <a href="https://arxiv.org/abs/2609.11873">📄 Survey</a> &nbsp;•&nbsp;
  <a href="#citation">📝 Cite</a> &nbsp;•&nbsp;
  <a href="#taxonomy-at-a-glance">🧭 Taxonomy</a> &nbsp;•&nbsp;
  <a href="#paper-catalog">📚 Catalog</a> &nbsp;•&nbsp;
  <a href="#industry-practices">🏭 Industry Cases</a> &nbsp;•&nbsp;
  <a href="#latest-updates">🆕 Updates</a> &nbsp;•&nbsp;
  <a href="#contributing">🤝 Contribute</a>
</p>

</div>

> This repository accompanies [**The Last AI Built by Humans: Toward Genuine Recursive Self-Improvement**](https://arxiv.org/abs/2609.11873) (Yi Duan et al., 2026; [arXiv:2609.11873](https://arxiv.org/abs/2609.11873)).

> Every listed paper retains its arXiv identifier, primary autonomy level, and updated-object classification.

RSI is the capability of an intelligent system to transform acquired experience and feedback into persistent changes to itself across interaction rounds, such that those changes can affect how later improvements are generated, evaluated, selected, and consolidated. The updated object may be model weights, prompts, code, memory, skills, task distributions, or the improvement mechanism itself. Levels capture autonomy over what is changed, how it is changed, and where later learning experience comes from; they are not paper-quality rankings.

<div align="center">
  <img src="./rsi-overview.png" width="96%" alt="RSI autonomy taxonomy overview: from in-task iteration and execution automation, through strategy search and experience acquisition, to deployment automation and meta-level improvement.">
  <br>
  <em><b>Figure 1.</b> RSI autonomy overview: from in-task iteration and execution automation, through strategy search and experience acquisition, to deployment automation and meta-level improvement.</em>
</div>

---

<a id="latest-updates"></a>

## Latest Updates <sub><a href="#readme-top">↑ top</a></sub>

This section logs material updates to this repository, including new source-verified research, industry coverage, and curation. It is editorially separate from the 521-paper taxonomy, so a release, project page, or repository update is never presented as a peer-reviewed paper by default.

1. **2026-09-24 — Paper and industry coverage expanded:** Added [GPTSwarm](https://arxiv.org/abs/2402.16823) to [L2](#2-l2---autonomy-over-improvement-strategies) and [Dream-RSI](https://arxiv.org/abs/2609.14858) to [L5](#5-l5---from-environmental-adaptation-to-meta-improvement), added two [industry cases](#industry-practices), and linked a related agent-focused survey in [Reading Paths](#reading-paths) after checking their primary sources.
   ![](https://img.shields.io/badge/-Repository-475569) ![](https://img.shields.io/badge/-Research-2563eb) ![](https://img.shields.io/badge/-Industry-0f766e)

1. **2026-09-19 — Public Industry Practices added:** A new [source-verified timeline](#industry-practices) launched with **11** publicly disclosed cases in which AI systems contribute to AI R&D, training or inference infrastructure, or retained self-improvement loops. Each entry distinguishes the reported result from the limits of its RSI claim. [[Browse the timeline](#industry-practices)]
   ![](https://img.shields.io/badge/-Repository-475569) ![](https://img.shields.io/badge/-Industry-0f766e) ![](https://img.shields.io/badge/-Curation-7c3aed)

1. **2026-09-10 — Companion survey released:** [*The Last AI Built by Humans: Toward Genuine Recursive Self-Improvement*](https://arxiv.org/abs/2609.11873) introduces HCI and the L1-L5 RSI roadmap used by this repository. [[Paper](https://arxiv.org/abs/2609.11873)]
   ![](https://img.shields.io/badge/-Research-2563eb) ![](https://img.shields.io/badge/-Survey-7c3aed) ![](https://img.shields.io/badge/-arXiv-b31b1b)

<details>
<summary><strong>Update policy</strong></summary>

- Include a repository update only when it adds or materially revises source-verified coverage; sources remain limited to primary research, official organization posts, technical reports, release notes, or maintained project pages.
- Tag source items as `Research` or `Industry` and state their material type (`Paper`, `Survey`, `Technical Report`, `Official Blog`, `Release`, or `Project`); tag repository-maintenance entries as `Repository` and state the affected coverage. State the update date and a neutral, one-sentence explanation of RSI relevance.
- Link research to an official proceedings page, DOI, or arXiv record; link industry items to the organization's original publication, never to a repost or social-media summary; link repository updates to the affected section.
- An update is not automatically an in-scope taxonomy paper. It enters the L1-L5 catalog only after the same paper-level relevance review.

</details>

<a id="industry-practices"></a>

## Public Industry Practices <sub><a href="#readme-top">↑ top</a></sub>

This timeline records **publicly disclosed cases in which AI systems participate in their organization's AI R&D, training or inference infrastructure, or a retained self-improvement loop**. It is deliberately separate from the paper catalog: each item is linked to a primary organization source and is **not** evidence that the system autonomously trained a successor frontier model. Results below are organization-reported, not independently reproduced.

Entries are ordered by publication date (newest first). “Boundary” names the most important limitation on the RSI claim rather than treating all feedback-driven optimization as equivalent.

| Date | Organization / primary source | Publicly disclosed practice | Reported result and boundary |
| --- | --- | --- | --- |
| 2026-09-17 | [Z.ai — *How GLM Built Its Own Inference Infrastructure*](https://z.ai/blog/glm-built-its-inference-infrastructure) | GLM-5.3 proposed and validated optimizations for the production inference infrastructure serving GLM-5.3-Flash, using correctness checks, execution traces, microbenchmarks, and end-to-end measurements. | Production-ready in under two weeks; end-to-end throughput reached about **3×** the initial version. This improves serving infrastructure, not GLM's own weights. |
| 2026-09-17 | [Anthropic — *Measurements for Understanding the Pace of AI Development Inside Frontier Labs*](https://www.anthropic.com/institute/measuring-pace-of-ai-development) | Anthropic measured Claude's participation across its internal AI-development work. | As of August 2026, Claude was reported to lead about **26%** of measured AI-R&D work and to collaborate on over **90%**; no measured task category was fully autonomous. |
| 2026-09-06 | [OpenAI — *Research Acceleration: The View Inside OpenAI*](https://openai.com/index/research-acceleration-view-inside-openai/) | OpenAI researchers used coding agents for research code, experiment support, and infrastructure troubleshooting; the organization measured their use across the AI R&D workflow. | By mid-August, agent runtime amounted to **3.1 eight-hour agent-days per human workday** across the research organization. This measures activity, not research productivity; over half of successful tasks estimated at 4–8 human hours still involved human intervention. |
| 2026-08-28 | [Tencent Hunyuan — *Tencent Releases and Open-Sources Tencent Hy4 Preview*](https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/) | Hy4 preview participated in its own R&D, including training methods, data strategy, evaluation, and low-level operator optimization; it also iterated on inference-system bottlenecks using experimental feedback. | Tencent reports **31.8%** end-to-end inference-throughput improvement. The objectives and acceptance process remain externally defined. |
| 2026-07-29 | [OpenAI — *How GPT-5.6 Fuses Frontier Intelligence with Frontier Efficiency*](https://openai.com/index/gpt-5-6-frontier-intelligence-efficiency/) | GPT-5.6 Sol analyzed production workloads, tested routing and forward-pass changes, rewrote production Triton/Gluon operators, and ran architecture experiments for speculative-decoding models. | OpenAI reports **20%** lower end-to-end serving cost and over **15%** token-generation efficiency improvement for speculative decoding. Neither figure means the base model retrained itself. |
| 2026-07-16 | [Moonshot AI — *Kimi K3: Open Frontier Intelligence*](https://www.kimi.com/en/blog/kimi-k3) | Early K3 versions performed most of the team's operator-optimization work late in K3 development, including attention-kernel work and a MiniTriton compiler demonstration. | This is model-assisted development of the software stack; the post does not establish a corresponding whole-training speedup or autonomous model development. |
| 2026-06-23 | [ByteDance Seed — *Seed2.1 Officially Released: Advancing AI Productivity*](https://seed.bytedance.com/en/blog/seed2-1-officially-released-advancing-ai-productivity) | Through “Seed for Seed,” Seed2.1 entered internal model R&D for evaluation, diagnosis, SFT data, RL-framework optimization, paper reproduction, and experiment validation, with multi-round use of intermediate artifacts and feedback. | Some tasks reportedly run for hours to tens of days. The post does not quantify an independent contribution to the final model or claim end-to-end autonomy. |
| 2026-06-11 | [Recursive — *First Steps Toward Automated AI Research*](https://www.recursive.com/articles/first-steps-toward-automated-ai-research) | An automated research system proposed changes, implemented them, ran and validated experiments, and reused context from earlier runs across small-model training and GPU-kernel benchmarks. | Recursive reports **0.9109** validation BPB on NanoChat Autoresearch versus **0.9372** for its comparison baseline. These are bounded benchmark results, not evidence that a frontier training pipeline is autonomously improving itself. |
| 2026-06 | [Anthropic — *When AI Builds Itself*](https://www.anthropic.com/institute/recursive-self-improvement) | Claude investigated training-cluster failures, modified training code, ran experiments, and reviewed code in Anthropic's development workflow. | Anthropic reports that over **80%** of merged code was attributable to Claude as of May 2026. Controlled training-code experiments should not be read as whole-frontier-training speedups. |
| 2026-05 | [OpenBMB — *ForgeTrain: An LLM Pretraining Framework Built End-to-End by an Autonomous Agent Loop*](https://github.com/OpenBMB/ForgeTrain) | An autonomous coding-agent loop wrote, debugged, and optimized an LLM pretraining framework end-to-end, repeatedly launching training jobs, parsing logs, diagnosing failures, patching code, and passing validation gates. The resulting framework completed MiniCPM4-0.5B pretraining and produced usable model weights. | OpenBMB reports **44.13% MFU** on 64×H100, about **10% above** its Megatron-LM baseline. The coding agent was external to MiniCPM; the harness, gates, objectives, and reference stack remained externally designed. |
| 2026-04-02 | [Meta — *KernelEvolve*](https://engineering.fb.com/2026/04/02/developer-tools/kernelevolve-how-metas-ranking-engineer-agent-optimizes-ai-infrastructure/) | Meta's Ranking Engineer Agent autonomously designed, executed, and analyzed model experiments; KernelEvolve retained a search tree while iterating through code generation, compilation, correctness checks, and performance tests for kernels. | Meta reports over **60%** inference-throughput improvement for an Andromeda advertising model on NVIDIA GPUs and over **25%** training-throughput improvement for an advertising model on MTIA. These are not Llama results. |
| 2026-03-18 | [MiniMax — *M2.7: Early Echoes of Self-Evolution*](https://www.minimax.io/news/minimax-m27-en) | M2.7 participated in RL-team workflows and repeatedly improved its own agent framework, tools, skills, and memory from failed trajectories and evaluation feedback. | MiniMax reports coverage of **30–50%** of selected workflows; one autonomous framework experiment ran for over **100** rounds and improved an internal evaluation by **30%**. These are workflow and internal-evaluation results, not a general base-model gain. |
| 2025-05-14 | [Google DeepMind — *AlphaEvolve*](https://deepmind.google/blog/alphaevolve-a-gemini-powered-coding-agent-for-designing-advanced-algorithms/) | AlphaEvolve used Gemini to generate algorithm candidates that were automatically evaluated and evolved; applications included Google infrastructure and a matrix-multiplication kernel used in Gemini training. | DeepMind reports a **23%** speedup for that training kernel, corresponding to roughly **1%** lower overall Gemini-training time. The search-and-verification harness remains a fixed, externally designed system. |

These cases range from benchmarked research systems to deployed infrastructure. Read each reported gain within the scope stated in its row; none establishes fully autonomous successor-model development.

## Table of Contents

- [Latest Updates](#latest-updates)
- [Public Industry Practices](#industry-practices)
- [Reading Paths](#reading-paths)
- [Companion Survey](#companion-survey)
- [Scope and Relevance Decision](#scope-and-relevance-decision)
- [RSI Improvement-Loop Anatomy](#rsi-improvement-loop-anatomy)
- [How to Read the Tags](#how-to-read-the-tags)
- [Taxonomy at a Glance](#taxonomy-at-a-glance)
- [1. L1 - Autonomy over Improvement Execution](#1-l1---autonomy-over-improvement-execution)
- [2. L2 - Autonomy over Improvement Strategies](#2-l2---autonomy-over-improvement-strategies)
- [3. L3 - Autonomy over Future Learning Experience](#3-l3---autonomy-over-future-learning-experience)
- [4. L4 - Autonomy in Deployment and Environmental Adaptation](#4-l4---autonomy-in-deployment-and-environmental-adaptation)
- [5. L5 - From Environmental Adaptation to Meta-Improvement](#5-l5---from-environmental-adaptation-to-meta-improvement)
- [Contributing](#contributing)
- [Citation](#citation)
- [Data Provenance and Validation](#data-provenance-and-validation)

<a id="reading-paths"></a>

## Reading Paths <sub><a href="#readme-top">↑ top</a></sub>

The full catalog is designed for reference, but these short routes provide a faster entry point:

| Goal | Suggested route |
| --- | --- |
| **Understand the field map** | Start with the [companion survey](https://arxiv.org/abs/2609.11873), then read the [improvement-loop anatomy](#rsi-improvement-loop-anatomy) and the [L1-L5 overview](#taxonomy-at-a-glance). |
| **Study persistent agent improvement** | Read [Voyager](https://arxiv.org/abs/2305.16291) for reusable skills and automatic curricula, then browse [L3](#3-l3---autonomy-over-future-learning-experience) and [L4](#4-l4---autonomy-in-deployment-and-environmental-adaptation). |
| **Study recursive meta-improvement** | Read [Darwin Gödel Machine](https://arxiv.org/abs/2505.22954) and [Gödel Agent](https://arxiv.org/abs/2410.04444), then browse [L5](#5-l5---from-environmental-adaptation-to-meta-improvement). |
| **Compare agent self-improvement surveys** | Read this repository's [companion survey](https://arxiv.org/abs/2609.11873) alongside [*Self-Improvements in Modern Agentic Systems*](https://arxiv.org/abs/2607.13104), which organizes updates to model parameters and agent scaffolds. |

<a id="companion-survey"></a>

## Companion Survey <sub><a href="#readme-top">↑ top</a></sub>

This collection accompanies [**The Last AI Built by Humans: Toward Genuine Recursive Self-Improvement**](https://arxiv.org/abs/2609.11873), by Yi Duan, Ying Liu, Zirui Tang, Haodong Chen, Jun Zhou, Yumou Liu, Bangrui Xu, Yukai Wu, Sidi Chen, Yuhan Zhou, Haoyu Wang, Xiaoyou Yu, Shaokun Han, Xuzhou Zhu, Le Zhou, Bolin Lu, Wei Zhou, Jiachen Liu, Nuozhou Fang, Jiaxin Tian, Ruoyu Chen, Yuxuan Li, Kai Zuo, Kaiyan Zhang, Jiantao Qiu, Conghui He, Guoliang Li, Bowen Zhou, Zhiyuan Liu, Zhoufutu Wen, Jihua Kang, Xuanhe Zhou, and Fan Wu.

The survey introduces the Headroom-Closed Index (HCI), develops the RSI roadmap represented by the L1-L5 taxonomy, and examines RSI in scientific discovery, embodied intelligence, and software engineering. This repository provides the paper-level, auditable companion to that roadmap.

[Read on arXiv](https://arxiv.org/abs/2609.11873) · [PDF](https://arxiv.org/pdf/2609.11873)

<a id="scope-and-relevance-decision"></a>

## Scope and Relevance Decision <sub><a href="#readme-top">↑ top</a></sub>

**The 491 baseline papers, 28 table-derived extensions, and two independently screened additions in this collection are retained as RSI-related under the L1-L5 taxonomy.** The taxonomy intentionally includes bounded forms and precursors:

- **L1 - Autonomy over Improvement Execution:** the system executes a human-defined improvement procedure, and its accepted results persist into later tasks or rounds.
- **L2 - Autonomy over Improvement Strategies:** the system chooses how to improve a specified target, while the objective, evaluation criterion, or acceptance rule remains external.
- **L3 - Autonomy over Future Learning Experience:** the learner's evolving state influences the experience, task, or curriculum acquired next.
- **L4 - Autonomy in Deployment and Environmental Adaptation:** reusable memory, skills, or deployed agent components are retained and alter later behavior within a fixed improvement process.
- **L5 - From Environmental Adaptation to Meta-Improvement:** the system improves the mechanism that produces future improvements, such as search, evaluation, or research-control policies.

Thus, inclusion does not claim that every entry is a fully autonomous or open-ended RSI system. The L1 and L2 labels make their bounded autonomy explicit.

<a id="rsi-improvement-loop-anatomy"></a>

## RSI Improvement-Loop Anatomy <sub><a href="#readme-top">↑ top</a></sub>

Each entry can be interpreted through the same loop: **experience -> candidate modification -> verifier / acceptance rule -> retained improvement -> successor re-entry**. The relevant components are:

| Component | Role in the loop |
| --- | --- |
| **System state** | Persistent state inherited by the next round. |
| **Experience** | Prior interaction outcomes, failures, feedback, or observations that inform an update. |
| **Target** | The object directly modified in the current round. |
| **Improver and strategy** | The mechanism that proposes candidates and decides where or how to search. |
| **Verifier** | The evaluator that applies an acceptance rule, such as tests, rewards, formal checks, or human feedback. |
| **Improvement and successor** | An accepted, retained state change and the next system version that inherits it. |

This anatomy supplies three tests for every claimed RSI loop: **Where does the loop close? What is updated and inherited? Which decisions remain external?**

<div align="center">
  <img src="./assets/rsi-loop-patterns.png" width="100%" alt="Five RSI loop patterns from L1 improvement-execution autonomy to L5 recursive inheritance autonomy. Human-controlled components are shown with gray dashed frames; the agentic loop expands as more improvement responsibilities are internalized.">
  <br>
  <em><b>Figure 2.</b> Loop patterns across L1-L5. The agentic loop expands as AI internalizes more of the improvement process, while human-controlled constraints remain explicit.</em>
</div>

<a id="how-to-read-the-tags"></a>

## How to Read the Tags <sub><a href="#readme-top">↑ top</a></sub>

Each entry has three colored badges:

| Badge | Meaning |
| --- | --- |
| `Level-L1` to `Level-L5` | Autonomy level and locus in the improvement loop |
| `In scope-RSI` | Retained by the source taxonomy's RSI relevance screen |
| `Target-...` | Primary family of the updated or searched object |

Blue, purple, orange, green, and red encode L1 through L5. Target colors distinguish the ten updated-object families. Each paper appears exactly once under its primary level; all available target codes are preserved in the entry.

<a id="taxonomy-at-a-glance"></a>

## Taxonomy at a Glance <sub><a href="#readme-top">↑ top</a></sub>

| Level | Papers | Interpretation |
| --- | ---: | --- |
| L1 | 219 | Autonomy over improvement execution. |
| L2 | 160 | Autonomy over improvement strategies. |
| L3 | 65 | Autonomy over future learning experience. |
| L4 | 45 | Autonomy in deployment and environmental adaptation. |
| L5 | 32 | From environmental adaptation to meta-improvement. |

Each level begins with a small set of **featured representative papers**, selected to cover its defining mechanisms and important research landmarks. They are entry points for reading, not quality rankings; the complete catalog remains available in the expandable section below each level.

### Updated-Object Families

| Code prefix | Family |
| --- | --- |
| 1 | Prompt & Context |
| 2 | Memory & Knowledge |
| 3 | Harness / Workflow |
| 4 | Tools & Skills |
| 5 | Model |
| 6 | Trainer / Optimization |
| 7 | Evaluator & Feedback |
| 8 | Data & Environment |
| 9 | External Artifact |
| 10 | Full-system / Co-evolution |


<a id="paper-catalog"></a>

<a id="1-l1---autonomy-over-improvement-execution"></a>

## 1. L1 - Autonomy over Improvement Execution <sub><a href="#readme-top">↑ top</a></sub>

The system executes a human-defined improvement procedure and retains accepted results for later tasks or rounds. **219 papers.**

### Featured representative papers

| Paper | Representative mechanism |
| --- | --- |
| [STaR](https://arxiv.org/abs/2203.14465) | Bootstraps model-generated rationales into a fixed, correctness-filtered self-training loop. |
| [Constitutional AI](https://arxiv.org/abs/2212.08073) | Establishes critique-and-revision with AI feedback under a human-specified constitution. |
| [ReST](https://arxiv.org/abs/2308.08998) | Generates an offline dataset with the current policy, then improves that policy with offline reinforcement learning. |
| [SPIN](https://arxiv.org/abs/2401.01335) | Generates training data from earlier policy iterations and refines the policy against human-annotated responses. |
| [Self-Rewarding Language Models](https://arxiv.org/abs/2401.10020) | Uses model-generated judgments as a fixed-protocol training signal. |
| [Meta-Rewarding Language Models](https://arxiv.org/abs/2407.19594) | Extends AI-feedback training to iterative refinement of the judging signal. |

<details>
<summary><strong>Browse the full L1 catalog (219 papers)</strong></summary>

### Table-derived extensions

The following additions are explicitly discussed in Table 3 of the survey, which organizes representative L1 systems by AI development pipeline level.

1. **Phi-4-reasoning Technical Report**  
   [[Paper](https://arxiv.org/abs/2504.21318)] · arXiv:2504.21318  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_Environment-ca8a04)  
   *Survey-table rationale:* Training-data selection through LLM evaluation and boundary filtering; selection criteria remain human-defined. *Updated object(s):* 8.1 Training / Experience Data.

1. **NVIDIA Nemotron-4 340B Technical Report**  
   [[Paper](https://arxiv.org/abs/2406.11704)] · arXiv:2406.11704  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_Environment-ca8a04)  
   *Survey-table rationale:* Synthetic supervision is generated and reward-filtered under human-defined quality dimensions. *Updated object(s):* 8.1 Training / Experience Data.

1. **EDIT: Evidence-Diagnosed Intervention Training for Rule-Faithful LLM Grading**  
   [[Paper](https://arxiv.org/abs/2606.06350)] · arXiv:2606.06350  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Trainer_Optimization-c2410c)  
   *Survey-table rationale:* Diagnosed-step revisions refine a training signal while diagnostic criteria remain human-defined. *Updated object(s):* 6.1 Training Objective.

1. **AIPC: Agent-Based Automation for AI Model Deployment with Qualcomm AI Runtime**  
   [[Paper](https://arxiv.org/abs/2604.14661)] · arXiv:2604.14661  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness_Workflow-0f766e)  
   *Survey-table rationale:* Skill-guided deployment adaptation follows a human-defined deployment procedure. *Updated object(s):* 3.6 Harness Implementation / Scaffold Code.


1. **$V_1$: Unifying Generation and Self-Verification for Parallel Reasoners**  
   [[Paper](https://arxiv.org/abs/2603.04304)] · arXiv:2603.04304  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **A Co-Evolving Agentic AI System for Medical Imaging Analysis**  
   [[Paper](https://arxiv.org/abs/2509.20279)] · arXiv:2509.20279  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter; 2.1 Experience Memory; 3.3 Harness / Workflow.

1. **A Context Engineering Framework for Improving Enterprise AI Agents based on Digital-Twin MDP**  
   [[Paper](https://arxiv.org/abs/2603.22083)] · arXiv:2603.22083  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L1. *Updated object(s):* 1.5 Context; 3.1 Workflow.

1. **A Dynamic Self-Evolving Extraction System**  
   [[Paper](https://arxiv.org/abs/2603.06915)] · arXiv:2603.06915  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.2 Knowledge Memory; 1.5 Context.

1. **A Model Can Help Itself: Reward-Free Self-Training for LLM Reasoning**  
   [[Paper](https://arxiv.org/abs/2510.18814)] · arXiv:2510.18814  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **A Self-Improvable Polymer Discovery Framework Based on Conditional Generative Model**  
   [[Paper](https://arxiv.org/abs/2312.04013)] · arXiv:2312.04013  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **ACE: Self-Evolving LLM Coding Framework via Adversarial Unit Test Generation and Preference Optimization**  
   [[Paper](https://arxiv.org/abs/2605.16299)] · arXiv:2605.16299  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **AceSearcher: Bootstrapping Reasoning and Search for LLMs via Reinforced Self-Play**  
   [[Paper](https://arxiv.org/abs/2509.24193)] · arXiv:2509.24193  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Active-GRPO: Adaptive Imitation and Self-Improving Reasoning for Molecular Optimization**  
   [[Paper](https://arxiv.org/abs/2607.00531)] · arXiv:2607.00531  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **AdaExplore: Failure-Driven Adaptation and Diversity-Preserving Search for Efficient Kernel Generation**  
   [[Paper](https://arxiv.org/abs/2604.16625)] · arXiv:2604.16625  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L1. *Updated object(s):* 1.1 Instruction; 2.2 Knowledge Memory.

1. **Agent Hospital: A Simulacrum of Hospital with Evolvable Medical Agents**  
   [[Paper](https://arxiv.org/abs/2405.02957)] · arXiv:2405.02957  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.1 Experience Memory; 2.3 Procedural Memory.

1. **Agent0-VL: Exploring Self-Evolving Agent for Tool-Integrated Vision-Language Reasoning**  
   [[Paper](https://arxiv.org/abs/2511.19900)] · arXiv:2511.19900  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **AgentGym: Evolving Large Language Model-based Agents across Diverse Environments**  
   [[Paper](https://arxiv.org/abs/2406.04151)] · arXiv:2406.04151  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Agentic-Ideation: Sample Efficient Agentic Trajectories Synthesis for Scientific Ideation Agents**  
   [[Paper](https://arxiv.org/abs/2606.31229)] · arXiv:2606.31229  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **AlgoSkill: Learning to Design Algorithms by Scheduling Human-Like Skills**  
   [[Paper](https://arxiv.org/abs/2606.29999)] · arXiv:2606.29999  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **AMR-SD: Asymmetric Meta-Reflective Self-Distillation for Token-Level Credit Assignment**  
   [[Paper](https://arxiv.org/abs/2605.18529)] · arXiv:2605.18529  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Anyprefer: An Agentic Framework for Preference Data Synthesis**  
   [[Paper](https://arxiv.org/abs/2504.19276)] · arXiv:2504.19276  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 1.1 Instruction.

1. **APR: Penalizing Structural Redundancy in Large Reasoning Models via Anchor-based Process Rewards**  
   [[Paper](https://arxiv.org/abs/2602.00760)] · arXiv:2602.00760  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **AutoMalDesc: Large-Scale Script Analysis for Cyber Threat Research**  
   [[Paper](https://arxiv.org/abs/2511.13333)] · arXiv:2511.13333  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **AutoResearchClaw: Self-Reinforcing Autonomous Research with Human-AI Collaboration**  
   [[Paper](https://arxiv.org/abs/2605.20025)] · arXiv:2605.20025  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.1 Experience Memory.

1. **Better, Faster: Harnessing Self-Improvement in Large Reasoning Models**  
   [[Paper](https://arxiv.org/abs/2605.24998)] · arXiv:2605.24998  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Beyond Imitation: Self-Improving Robot Policies via Off-Policy Q-Planning**  
   [[Paper](https://arxiv.org/abs/2608.21204)] · arXiv:2608.21204  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter.

1. **Beyond Self-Play: Hierarchical Reasoning for Continuous Motion in Closed-Loop Traffic Simulation**  
   [[Paper](https://arxiv.org/abs/2605.09153)] · arXiv:2605.09153  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Binary Decompilation LLM with Feedback-Driven Multi-Turn Refinement**  
   [[Paper](https://arxiv.org/abs/2606.16162)] · arXiv:2606.16162  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **BiWM: Advancing Open-Source Interactive Video World Models with Bidirectional Autoregression**  
   [[Paper](https://arxiv.org/abs/2606.10135)] · arXiv:2606.10135  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Breaking the Self-Confirming Loop: Diagnosing and Mitigating Systemic Reward Bias in Self-Rewarding RL**  
   [[Paper](https://arxiv.org/abs/2510.08977)] · arXiv:2510.08977  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Bridging What the Model Thinks and How It Speaks: Expressive Speech Generation via Self-Aware Intent-Realization Alignment**  
   [[Paper](https://arxiv.org/abs/2604.11424)] · arXiv:2604.11424  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Can Large Reasoning Models Self-Train?**  
   [[Paper](https://arxiv.org/abs/2505.21444)] · arXiv:2505.21444  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Can Recommender Systems Teach Themselves? A Recursive Self-Improving Framework with Fidelity Control**  
   [[Paper](https://arxiv.org/abs/2602.15659)] · arXiv:2602.15659  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **CAST: Non-Privileged Clipped Asymmetric Self-Teaching with Advantage Flipping for GRPO**  
   [[Paper](https://arxiv.org/abs/2606.00172)] · arXiv:2606.00172  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **CATPO: Critique-Augmented Tree Policy Optimization**  
   [[Paper](https://arxiv.org/abs/2606.08346)] · arXiv:2606.08346  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.4 Curriculum.

1. **CEPO: RLVR Self-Distillation using Contrastive Evidence Policy Optimization**  
   [[Paper](https://arxiv.org/abs/2605.19436)] · arXiv:2605.19436  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **CIIR@LiveRAG 2025: Optimizing Multi-Agent Retrieval Augmented Generation through Self-Training**  
   [[Paper](https://arxiv.org/abs/2506.10844)] · arXiv:2506.10844  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter.

1. **Cleansing the Artificial Mind: A Self-Reflective Detoxification Framework for Large Language Models**  
   [[Paper](https://arxiv.org/abs/2601.11776)] · arXiv:2601.11776  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Co-rewarding: Stable Self-supervised RL for Eliciting Reasoning in Large Language Models**  
   [[Paper](https://arxiv.org/abs/2508.00410)] · arXiv:2508.00410  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **CoAct: Co-Active LLM Preference Learning with Human-AI Synergy**  
   [[Paper](https://arxiv.org/abs/2604.17501)] · arXiv:2604.17501  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Consistent Paths Lead to Truth: Self-Rewarding Reinforcement Learning for LLM Reasoning**  
   [[Paper](https://arxiv.org/abs/2506.08745)] · arXiv:2506.08745  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Constitutional AI: Harmlessness from AI Feedback**  
   [[Paper](https://arxiv.org/abs/2212.08073)] · arXiv:2212.08073  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 7.2 Reward / Fitness.

1. **Continual Self-Improvement with Lightweight Experiential Latent Memories**  
   [[Paper](https://arxiv.org/abs/2606.17803)] · arXiv:2606.17803  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter; 2.1 Experience Memory.

1. **Continuous Self-Improvement of Large Language Models by Test-time Training with Verifier-Driven Sample Selection**  
   [[Paper](https://arxiv.org/abs/2505.19475)] · arXiv:2505.19475  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter.

1. **CoVerRL: Breaking the Consensus Trap in Label-Free Reasoning via Generator-Verifier Co-Evolution**  
   [[Paper](https://arxiv.org/abs/2603.17775)] · arXiv:2603.17775  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **CREAM: Consistency Regularized Self-Rewarding Language Models**  
   [[Paper](https://arxiv.org/abs/2410.12735)] · arXiv:2410.12735  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **CritiCal: Can Critique Help LLM Uncertainty or Confidence Calibration?**  
   [[Paper](https://arxiv.org/abs/2510.24505)] · arXiv:2510.24505  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Deciphering Scientific Reasoning Steps from Outcome Data for Molecule Optimization**  
   [[Paper](https://arxiv.org/abs/2603.20262)] · arXiv:2603.20262  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Decouple to Generalize: Context-First Self-Evolving Learning for Data-Scarce Vision-Language Reasoning**  
   [[Paper](https://arxiv.org/abs/2512.06835)] · arXiv:2512.06835  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **DeepInnovator: Triggering the Innovative Capabilities of LLMs**  
   [[Paper](https://arxiv.org/abs/2602.18920)] · arXiv:2602.18920  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **DeepSeekMath-V2: Towards Self-Verifiable Mathematical Reasoning**  
   [[Paper](https://arxiv.org/abs/2511.22570)] · arXiv:2511.22570  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 7.3 Verifier.

1. **DemoPSD: Disagreement-Modulated Policy Self-Distillation**  
   [[Paper](https://arxiv.org/abs/2607.02502)] · arXiv:2607.02502  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Depression Diagnosis Dialogue Simulation: Self-improving Psychiatrist with Tertiary Memory**  
   [[Paper](https://arxiv.org/abs/2409.15084)] · arXiv:2409.15084  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.1 Experience Memory; 2.3 Procedural Memory.

1. **DermoGPT: Open Weights and Open Data for Morphology-Grounded Dermatological Reasoning MLLMs**  
   [[Paper](https://arxiv.org/abs/2601.01868)] · arXiv:2601.01868  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Differentiable Mixture-of-Agents Incentivizes Swarm Intelligence of Large Language Models**  
   [[Paper](https://arxiv.org/abs/2605.15706)] · arXiv:2605.15706  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L1. *Updated object(s):* 3.3 Harness / Workflow; 5.2 Adapter.

1. **Distilling LLM Feedback for Lean Theorem Proving**  
   [[Paper](https://arxiv.org/abs/2605.30861)] · arXiv:2605.30861  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Double-Checker: Enhancing Reasoning of Slow-Thinking LLMs via Self-Critical Fine-Tuning**  
   [[Paper](https://arxiv.org/abs/2506.21285)] · arXiv:2506.21285  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **DRIFT: Difficulty Routing Self-DIstillation with Rhythm-Gated Exploration and Success BuFfer Training**  
   [[Paper](https://arxiv.org/abs/2606.30345)] · arXiv:2606.30345  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Dual-Modality Multi-Stage Adversarial Safety Training: Robustifying Multimodal Web Agents Against Cross-Modal Attacks**  
   [[Paper](https://arxiv.org/abs/2603.04364)] · arXiv:2603.04364  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **DuPO: Enabling Reliable LLM Self-Verification via Dual Preference Optimization**  
   [[Paper](https://arxiv.org/abs/2508.14460)] · arXiv:2508.14460  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Dynamic Alignment for Collective Agency: Toward a Scalable Self-Improving Framework for Open-Ended LLM Alignment**  
   [[Paper](https://arxiv.org/abs/2512.05464)] · arXiv:2512.05464  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **EARS: Explanatory Abstention for Reliable Sub-Agent Modeling in Large-scale Multi-Agent Systems**  
   [[Paper](https://arxiv.org/abs/2606.18668)] · arXiv:2606.18668  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Easy Samples Are All You Need: Self-Evolving LLMs via Data-Efficient Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2604.18639)] · arXiv:2604.18639  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Emulating Clinician Cognition via Self-Evolving Deep Clinical Research**  
   [[Paper](https://arxiv.org/abs/2603.10677)] · arXiv:2603.10677  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.1 Experience Memory.

1. **Endless Terminals: Scaling RL Environments for Terminal Agents**  
   [[Paper](https://arxiv.org/abs/2601.16443)] · arXiv:2601.16443  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.3 Environment.

1. **Enhancing Mathematical Reasoning in LLMs with Background Operators**  
   [[Paper](https://arxiv.org/abs/2412.04110)] · arXiv:2412.04110  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **EpiCaR: Knowing What You Don't Know Matters for Better Reasoning in LLMs**  
   [[Paper](https://arxiv.org/abs/2601.06786)] · arXiv:2601.06786  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Evo-MedAgent: Beyond One-Shot Diagnosis with Agents That Remember, Reflect, and Improve**  
   [[Paper](https://arxiv.org/abs/2604.14475)] · arXiv:2604.14475  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.1 Experience Memory; 2.3 Procedural Memory.

1. **EvoDefense: Co-Evolving Black-Box Defense with Large Language Models**  
   [[Paper](https://arxiv.org/abs/2605.31140)] · arXiv:2605.31140  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter; 2.1 Experience Memory.

1. **EVOLVE-VLA: Test-Time Training from Environment Feedback for Vision-Language-Action Models**  
   [[Paper](https://arxiv.org/abs/2512.14666)] · arXiv:2512.14666  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **ExpeL: LLM Agents Are Experiential Learners**  
   [[Paper](https://arxiv.org/abs/2308.10144)] · arXiv:2308.10144  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.1 Experience Memory; 2.2 Knowledge Memory.

1. **Exploring and Exploiting the Inherent Efficiency within Large Reasoning Models for Self-Guided Efficiency Enhancement**  
   [[Paper](https://arxiv.org/abs/2506.15647)] · arXiv:2506.15647  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **ExpRL: Exploratory RL for LLM Mid-Training**  
   [[Paper](https://arxiv.org/abs/2606.17024)] · arXiv:2606.17024  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **FiRe: Fine-grained Multimodal Reasoning for Enhanced Image Generation**  
   [[Paper](https://arxiv.org/abs/2604.13491)] · arXiv:2604.13491  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **First SFT, Second RL, Third UPT: Continual Improving Multi-Modal LLM Reasoning via Unsupervised Post-Training**  
   [[Paper](https://arxiv.org/abs/2505.22453)] · arXiv:2505.22453  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Forward-Free Diffusion Language Models with BPTT-Free Looped Refinement**  
   [[Paper](https://arxiv.org/abs/2606.08357)] · arXiv:2606.08357  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **From Memorization to Creativity: LLM as a Designer of Novel Neural Architectures**  
   [[Paper](https://arxiv.org/abs/2601.02997)] · arXiv:2601.02997  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter; 8.1 Experience Data.

1. **Generating on Generated: An Approach Towards Self-Evolving Diffusion Models**  
   [[Paper](https://arxiv.org/abs/2502.09963)] · arXiv:2502.09963  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **GRAM-R^2: Self-Training Generative Foundation Reward Models for Reward Reasoning**  
   [[Paper](https://arxiv.org/abs/2509.02492)] · arXiv:2509.02492  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **GSEM: Graph-based Self-Evolving Memory for Experience Augmented Clinical Reasoning**  
   [[Paper](https://arxiv.org/abs/2603.22096)] · arXiv:2603.22096  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.1 Experience Memory; 2.4 Memory & Knowledge.

1. **Heterogeneous Self-Play for Realistic Highway Traffic Simulation**  
   [[Paper](https://arxiv.org/abs/2604.16406)] · arXiv:2604.16406  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **How to Train Your Long-Context Visual Document Model**  
   [[Paper](https://arxiv.org/abs/2602.15257)] · arXiv:2602.15257  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 7.1 Judge.

1. **HS-STaR: Hierarchical Sampling for Self-Taught Reasoners via Difficulty Estimation and Budget Reallocation**  
   [[Paper](https://arxiv.org/abs/2505.19866)] · arXiv:2505.19866  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.4 Curriculum.

1. **ICRL: Learning to Internalize Self-Critique with Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2605.15224)] · arXiv:2605.15224  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Improving LLM Code Reasoning via Semantic Equivalence Self-Play with Formal Verification**  
   [[Paper](https://arxiv.org/abs/2604.17010)] · arXiv:2604.17010  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 5.2 Adapter.

1. **Improving Reasoning in Vision-Language Models via Perception Verified Self-Training**  
   [[Paper](https://arxiv.org/abs/2606.22158)] · arXiv:2606.22158  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **IRIS: Interpolative Rényi Iterative Self-play for Large Language Model Fine-Tuning**  
   [[Paper](https://arxiv.org/abs/2604.20933)] · arXiv:2604.20933  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Iterative Compositional Data Generation for Robot Control**  
   [[Paper](https://arxiv.org/abs/2512.10891)] · arXiv:2512.10891  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **JailDAM: Jailbreak Detection with Adaptive Memory for Vision-Language Model**  
   [[Paper](https://arxiv.org/abs/2504.03770)] · arXiv:2504.03770  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.2 Knowledge Memory; 2.5 Memory & Knowledge.

1. **KBSpec: LLM-driven Formal Specification Generation with Evolving Domain Knowledge Base**  
   [[Paper](https://arxiv.org/abs/2606.21339)] · arXiv:2606.21339  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.2 Knowledge Memory; 2.3 Procedural Memory.

1. **Keep Policy Gradient in Charge: Sibling-Guided Credit Distillation for Long-Horizon Tool-Use Agents**  
   [[Paper](https://arxiv.org/abs/2606.12634)] · arXiv:2606.12634  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Know When to Stop: Segment-Level Credit Assignment for Reducing Overthinking**  
   [[Paper](https://arxiv.org/abs/2607.00482)] · arXiv:2607.00482  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **KVerus: Scalable and Resilient Formal Verification Proof Generation for Rust Code**  
   [[Paper](https://arxiv.org/abs/2605.03822)] · arXiv:2605.03822  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L1. *Updated object(s):* 9.1 Program Code; 2.2 Knowledge Memory.

1. **Latent Preference Modeling for Cross-Session Personalized Tool Calling**  
   [[Paper](https://arxiv.org/abs/2604.17886)] · arXiv:2604.17886  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.2 Knowledge Memory.

1. **Learn from Your Mistakes: Tree-like Self-Play for Secure Code LLMs**  
   [[Paper](https://arxiv.org/abs/2606.03489)] · arXiv:2606.03489  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Learn Your Reference Model for Real Good Alignment**  
   [[Paper](https://arxiv.org/abs/2404.09656)] · arXiv:2404.09656  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Learning from Language Feedback via Variational Policy Distillation**  
   [[Paper](https://arxiv.org/abs/2605.15113)] · arXiv:2605.15113  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Learning from Supervision with Semantic and Episodic Memory: A Reflective Approach to Agent Adaptation**  
   [[Paper](https://arxiv.org/abs/2510.19897)] · arXiv:2510.19897  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.1 Experience Memory; 2.2 Knowledge Memory.

1. **Learning from Your Own Mistakes: Constructing Learnable Micro-Reflective Trajectories for Self-Distillation**  
   [[Paper](https://arxiv.org/abs/2606.18844)] · arXiv:2606.18844  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Learning Steerable Clarification Policies with Collaborative Self-play**  
   [[Paper](https://arxiv.org/abs/2512.04068)] · arXiv:2512.04068  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Learning to Better Search with Language Models via Guided Reinforced Self-Training**  
   [[Paper](https://arxiv.org/abs/2410.02992)] · arXiv:2410.02992  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Learning to Plan & Reason for Evaluation with Thinking-LLM-as-a-Judge**  
   [[Paper](https://arxiv.org/abs/2501.18099)] · arXiv:2501.18099  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Learning to Plan Before Answering: Self-Teaching LLMs to Learn Abstract Plans for Problem Solving**  
   [[Paper](https://arxiv.org/abs/2505.00031)] · arXiv:2505.00031  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Learning to Self-Verify Makes Language Models Better Reasoners**  
   [[Paper](https://arxiv.org/abs/2602.07594)] · arXiv:2602.07594  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Learning to Solve and Verify: A Self-Play Framework for Code and Test Generation**  
   [[Paper](https://arxiv.org/abs/2502.14948)] · arXiv:2502.14948  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **LLM-Personalize: Aligning LLM Planners with Human Preferences via Reinforced Self-Training for Housekeeping Robots**  
   [[Paper](https://arxiv.org/abs/2404.14285)] · arXiv:2404.14285  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Meta-Rewarding Language Models: Self-Improving Alignment with LLM-as-a-Meta-Judge**  
   [[Paper](https://arxiv.org/abs/2407.19594)] · arXiv:2407.19594  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **MiGrATe: Mixed-Policy GRPO for Adaptation at Test-Time**  
   [[Paper](https://arxiv.org/abs/2508.08641)] · arXiv:2508.08641  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter.

1. **MobileIPL: Enhancing Mobile Agents Thinking Process via Iterative Preference Learning**  
   [[Paper](https://arxiv.org/abs/2505.12299)] · arXiv:2505.12299  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Monte Carlo Tree Search with Reasoning Path Refinement for Small Language Models in Conversational Text-to-NoSQL**  
   [[Paper](https://arxiv.org/abs/2602.12574)] · arXiv:2602.12574  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Motus2: A Self-Evolving General World Model for Dexterous Manipulation**  
   [[Paper](https://arxiv.org/abs/2608.30237)] · arXiv:2608.30237  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.4 Data & Environment; 7.2 Reward / Fitness.

1. **Not All Synthetic Data Is Yours to Learn From**  
   [[Paper](https://arxiv.org/abs/2605.31126)] · arXiv:2605.31126  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Object-Centric Residual RL for Zero-Shot Sim-to-Real VLA Enhancement**  
   [[Paper](https://arxiv.org/abs/2606.18953)] · arXiv:2606.18953  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 5.2 Adapter.

1. **Observations and Remedies for Large Language Model Bias in Self-Consuming Performative Loop**  
   [[Paper](https://arxiv.org/abs/2601.05184)] · arXiv:2601.05184  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **OmniOPSD: Rationale-Privileged On-Policy Self-Distillation for Affective Computing**  
   [[Paper](https://arxiv.org/abs/2606.15920)] · arXiv:2606.15920  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **OWL: Unsupervised 3D Object Detection by Occupancy Guided Warm-up and Large Model Priors Reasoning**  
   [[Paper](https://arxiv.org/abs/2512.05698)] · arXiv:2512.05698  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **PaperSearchQA: Learning to Search and Reason over Scientific Papers with RLVR**  
   [[Paper](https://arxiv.org/abs/2601.18207)] · arXiv:2601.18207  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **PARNESS: A Paper Harness for End-to-End Automated Scientific Research with Dynamic Workflows, Full-Text Indexing, and Cross-Run Knowledge Accumulation**  
   [[Paper](https://arxiv.org/abs/2605.05258)] · arXiv:2605.05258  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.2 Knowledge Memory; 2.1 Experience Memory.

1. **Paying More Attention to Visual Tokens in Self-Evolving Large Multimodal Models**  
   [[Paper](https://arxiv.org/abs/2606.27373)] · arXiv:2606.27373  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter; 6.1 Objective.

1. **PBSD: Privileged Bayesian Self-Distillation for Long-Horizon Credit Assignment**  
   [[Paper](https://arxiv.org/abs/2606.09348)] · arXiv:2606.09348  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **PEARL: Training Socratic Tutors with Pedagogically Aligned Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2605.29582)] · arXiv:2605.29582  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Peer-Predictive Self-Training for Language Model Reasoning**  
   [[Paper](https://arxiv.org/abs/2604.13356)] · arXiv:2604.13356  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Perception, Verdict, and Evolution: Hindsight-Driven Self-Refining Forensics Agent for AI-Generated Image Detection**  
   [[Paper](https://arxiv.org/abs/2606.26552)] · arXiv:2606.26552  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **PLLM: Pseudo-Labeling Large Language Models for CAD Program Synthesis**  
   [[Paper](https://arxiv.org/abs/2602.12561)] · arXiv:2602.12561  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter.

1. **Policy-Guided Stepwise Model Routing for Cost-Effective Reasoning**  
   [[Paper](https://arxiv.org/abs/2605.06116)] · arXiv:2605.06116  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L1. *Updated object(s):* 3.3 Harness / Workflow.

1. **Post-Training Probability Manifold Correction via Structured SVD Pruning and Self-Referential Distillation**  
   [[Paper](https://arxiv.org/abs/2602.00372)] · arXiv:2602.00372  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Poster: ClawdGo: Endogenous Security Awareness Training for Autonomous AI Agents**  
   [[Paper](https://arxiv.org/abs/2604.24020)] · arXiv:2604.24020  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.3 Procedural Memory; 2.5 Memory & Knowledge; 8.2 Task Generator.

1. **PRefLexOR: Preference-based Recursive Language Modeling for Exploratory Optimization of Reasoning and Agentic Thinking**  
   [[Paper](https://arxiv.org/abs/2410.12375)] · arXiv:2410.12375  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **PRISMA: Preference-Reinforced Self-Training Approach for Interpretable Emotionally Intelligent Negotiation Dialogues**  
   [[Paper](https://arxiv.org/abs/2604.18354)] · arXiv:2604.18354  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Probing Visual Language Priors in VLMs**  
   [[Paper](https://arxiv.org/abs/2501.00569)] · arXiv:2501.00569  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Procedural Memory Distillation: Online Reflection for Self-Improving Language Models**  
   [[Paper](https://arxiv.org/abs/2607.01480)] · arXiv:2607.01480  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Process-based Self-Rewarding Language Models**  
   [[Paper](https://arxiv.org/abs/2503.03746)] · arXiv:2503.03746  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **ProcessThinker: Enhancing Multi-modal Large Language Models Reasoning via Rollout-based Process Reward**  
   [[Paper](https://arxiv.org/abs/2606.11209)] · arXiv:2606.11209  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **PsychAgent: An Experience-Driven Lifelong Learning Agent for Self-Evolving Psychological Counselor**  
   [[Paper](https://arxiv.org/abs/2604.00931)] · arXiv:2604.00931  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 4.4 Skill Library.

1. **Pythagoras-Prover: Advancing Efficient Formal Proving via Augmented Lean Formalisation**  
   [[Paper](https://arxiv.org/abs/2606.12594)] · arXiv:2606.12594  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Quiet-STaR: Language Models Can Teach Themselves to Think Before Speaking**  
   [[Paper](https://arxiv.org/abs/2403.09629)] · arXiv:2403.09629  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Reasoning and Learning a Perceptual Metric for Self-Training of Reflective Objects in Bin-Picking with a Low-cost Camera**  
   [[Paper](https://arxiv.org/abs/2503.20207)] · arXiv:2503.20207  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Reasoning-Enhanced Self-Training for Long-Form Personalized Text Generation**  
   [[Paper](https://arxiv.org/abs/2501.04167)] · arXiv:2501.04167  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **RebuttalAgent: Strategic Persuasion in Academic Rebuttal via Theory of Mind**  
   [[Paper](https://arxiv.org/abs/2601.15715)] · arXiv:2601.15715  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Red-Bandit: Test-Time Adaptation for LLM Red-Teaming via Bandit-Guided LoRA Experts**  
   [[Paper](https://arxiv.org/abs/2510.07239)] · arXiv:2510.07239  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter; 3.3 Harness / Workflow.

1. **ReGuide: From Test-Time Guidance to Self-Improving Diffusion Policies**  
   [[Paper](https://arxiv.org/abs/2606.28939)] · arXiv:2606.28939  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Reinforced Self-Training (ReST) for Language Modeling**  
   [[Paper](https://arxiv.org/abs/2308.08998)] · arXiv:2308.08998  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Reinforcement Learning for Self-Improving Agent with Skill Library**  
   [[Paper](https://arxiv.org/abs/2512.17102)] · arXiv:2512.17102  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 4.4 Skill Library.

1. **Reinforcement Learning from Rich Feedback with Distributional DAgger**  
   [[Paper](https://arxiv.org/abs/2606.05152)] · arXiv:2606.05152  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **ReNIO: Reweighting Negative Trajectory Importance for LLM On-Policy Distillation**  
   [[Paper](https://arxiv.org/abs/2606.23104)] · arXiv:2606.23104  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **ReST-MCTS*: LLM Self-Training via Process Reward Guided Tree Search**  
   [[Paper](https://arxiv.org/abs/2406.03816)] · arXiv:2406.03816  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 7.2 Reward / Fitness.

1. **ReSteer: Quantifying and Refining the Steerability of Multitask Robot Policies**  
   [[Paper](https://arxiv.org/abs/2603.17300)] · arXiv:2603.17300  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Rethinking Reward Supervision: Rubric-Conditioned Self-Distillation**  
   [[Paper](https://arxiv.org/abs/2606.19327)] · arXiv:2606.19327  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **RetroAgent: From Solving to Evolving via Retrospective Dual Intrinsic Feedback**  
   [[Paper](https://arxiv.org/abs/2603.08561)] · arXiv:2603.08561  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 2.1 Experience Memory.

1. **Right in the Right Way: LM Training with Verifiable Rewards and Human Demonstrations**  
   [[Paper](https://arxiv.org/abs/2607.01181)] · arXiv:2607.01181  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective; 5.2 Adapter.

1. **RLSR: Reinforcement Learning from Self Reward**  
   [[Paper](https://arxiv.org/abs/2505.08827)] · arXiv:2505.08827  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Robot Self-Improvement via Human-Video Dynamics Models**  
   [[Paper](https://arxiv.org/abs/2606.21406)] · arXiv:2606.21406  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **ROSD: Reflective On-Policy Self-Distillation for Language Model Reasoning across Domains**  
   [[Paper](https://arxiv.org/abs/2605.28014)] · arXiv:2605.28014  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Route, Retrieve, Reflect, Repair: Self-Improving Agentic Framework for Visual Detection and Linguistic Reasoning in Medical Imaging**  
   [[Paper](https://arxiv.org/abs/2601.08192)] · arXiv:2601.08192  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.1 Experience Memory; 1.4 Prompt & Context.

1. **S-SPPO: Semantic-Calibrated Self-Play Preference Optimization**  
   [[Paper](https://arxiv.org/abs/2606.01561)] · arXiv:2606.01561  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **SAEExplainer: Interpreting SAE Features with Activation-Guided Preference Optimization**  
   [[Paper](https://arxiv.org/abs/2606.08496)] · arXiv:2606.08496  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Safe Autoregressive Image Generation with Iterative Self-Improving Codebooks**  
   [[Paper](https://arxiv.org/abs/2606.27147)] · arXiv:2606.27147  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **SafeCtrl-RL: Inference-Time Adaptive Behaviour Control for LLM Dialogue via RL-Driven Prompt Optimisation**  
   [[Paper](https://arxiv.org/abs/2605.25984)] · arXiv:2605.25984  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter; 3.4 Harness / Workflow.

1. **SafeSteer: Localized On-Policy Distillation for Efficient Safety Alignment**  
   [[Paper](https://arxiv.org/abs/2606.02530)] · arXiv:2606.02530  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **SD-Search: On-Policy Hindsight Self-Distillation for Search-Augmented Reasoning**  
   [[Paper](https://arxiv.org/abs/2605.18299)] · arXiv:2605.18299  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Search-E1: Self-Distillation Drives Self-Evolution in Search-Augmented Reasoning**  
   [[Paper](https://arxiv.org/abs/2605.22511)] · arXiv:2605.22511  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **See, Think, Learn: A Self-Taught Multimodal Reasoner**  
   [[Paper](https://arxiv.org/abs/2512.02456)] · arXiv:2512.02456  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Adapting Improvement Loops for Robotic Learning**  
   [[Paper](https://arxiv.org/abs/2506.06658)] · arXiv:2506.06658  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Alignment with Instruction Backtranslation**  
   [[Paper](https://arxiv.org/abs/2308.06259)] · arXiv:2308.06259  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Consistency of the Internal Reward Models Improves Self-Rewarding Language Models**  
   [[Paper](https://arxiv.org/abs/2502.08922)] · arXiv:2502.08922  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **SELF-EMO: Emotional Self-Evolution from Recognition to Consistent Expression**  
   [[Paper](https://arxiv.org/abs/2604.18003)] · arXiv:2604.18003  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Evolution for Multi-Turn Tool-Calling Agents via Divergence-Point Preference Learning**  
   [[Paper](https://arxiv.org/abs/2606.23112)] · arXiv:2606.23112  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-evolving LLM agents with in-distribution Optimization**  
   [[Paper](https://arxiv.org/abs/2606.07367)] · arXiv:2606.07367  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 5.2 Adapter.

1. **Self-Improving Embodied Foundation Models**  
   [[Paper](https://arxiv.org/abs/2509.15155)] · arXiv:2509.15155  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Improving Tabular Language Models via Iterative Reward-Guided Post-Training**  
   [[Paper](https://arxiv.org/abs/2604.18966)] · arXiv:2604.18966  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Improving VLM Judges Without Human Annotations**  
   [[Paper](https://arxiv.org/abs/2512.05145)] · arXiv:2512.05145  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Play Enhancement via Advantage-Weighted Refinement in Online Federated LLM Fine-Tuning with Real-Time Feedback**  
   [[Paper](https://arxiv.org/abs/2605.07977)] · arXiv:2605.07977  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Self-Play Fine-Tuning Converts Weak Language Models to Strong Language Models (SPIN)**  
   [[Paper](https://arxiv.org/abs/2401.01335)] · arXiv:2401.01335  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Self-playing Adversarial Language Game Enhances LLM Reasoning (SPAG)**  
   [[Paper](https://arxiv.org/abs/2404.10642)] · arXiv:2404.10642  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Policy Distillation via Capability-Selective Subspace Projection**  
   [[Paper](https://arxiv.org/abs/2605.22675)] · arXiv:2605.22675  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Reasoning Language Models: Unfold Hidden Reasoning Chains with Few Reasoning Catalyst**  
   [[Paper](https://arxiv.org/abs/2505.14116)] · arXiv:2505.14116  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Self-rewarding correction for mathematical reasoning**  
   [[Paper](https://arxiv.org/abs/2502.19613)] · arXiv:2502.19613  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Rewarding Language Models**  
   [[Paper](https://arxiv.org/abs/2401.10020)] · arXiv:2401.10020  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Self-Rewarding Large Vision-Language Models for Optimizing Prompts in Text-to-Image Generation**  
   [[Paper](https://arxiv.org/abs/2505.16763)] · arXiv:2505.16763  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Rewarding PPO: Aligning Large Language Models with Demonstrations Only**  
   [[Paper](https://arxiv.org/abs/2510.21090)] · arXiv:2510.21090  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Rewarding Rubric-Based Reinforcement Learning for Open-Ended Reasoning**  
   [[Paper](https://arxiv.org/abs/2509.25534)] · arXiv:2509.25534  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Taught Evaluators**  
   [[Paper](https://arxiv.org/abs/2408.02666)] · arXiv:2408.02666  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Self-Trained Verification for Training- and Test-Time Self-Improvement**  
   [[Paper](https://arxiv.org/abs/2605.30290)] · arXiv:2605.30290  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Self-Training Large Language Models for Improved Visual Program Synthesis With Visual Reinforcement**  
   [[Paper](https://arxiv.org/abs/2404.04627)] · arXiv:2404.04627  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Semi-supervised Instruction Tuning for Large Language Models on Text-Attributed Graphs**  
   [[Paper](https://arxiv.org/abs/2601.12807)] · arXiv:2601.12807  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter.

1. **SeRL: Self-Play Reinforcement Learning for Large Language Models with Limited Data**  
   [[Paper](https://arxiv.org/abs/2505.20347)] · arXiv:2505.20347  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Skill-Conditioned Gated Self-Distillation for LLM Reasoning**  
   [[Paper](https://arxiv.org/abs/2605.28791)] · arXiv:2605.28791  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 2.3 Procedural Memory; 6.1 Objective.

1. **Skill-Guided Continuation Distillation for GUI Agents**  
   [[Paper](https://arxiv.org/abs/2606.18890)] · arXiv:2606.18890  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **SmartSnap: Proactive Evidence Seeking for Self-Verifying Agents**  
   [[Paper](https://arxiv.org/abs/2512.22322)] · arXiv:2512.22322  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **SocraticPO: Policy Optimization via Interactive Guidance**  
   [[Paper](https://arxiv.org/abs/2606.09887)] · arXiv:2606.09887  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Soft-NBCE: Entropy-Weighted Chunk Fusion for Long-Context**  
   [[Paper](https://arxiv.org/abs/2606.01101)] · arXiv:2606.01101  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **SPPD: Self-training with Process Preference Learning Using Dynamic Value Margin**  
   [[Paper](https://arxiv.org/abs/2502.13516)] · arXiv:2502.13516  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **SRPO: Self-Referential Policy Optimization for Vision-Language-Action Models**  
   [[Paper](https://arxiv.org/abs/2511.15605)] · arXiv:2511.15605  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 7.2 Reward / Fitness.

1. **STaR: Self-Taught Reasoner—Bootstrapping Reasoning With Reasoning**  
   [[Paper](https://arxiv.org/abs/2203.14465)] · arXiv:2203.14465  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **STEP: Enhancing Video-LLMs' Compositional Reasoning by Spatio-Temporal Graph-guided Self-Training**  
   [[Paper](https://arxiv.org/abs/2412.00161)] · arXiv:2412.00161  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **StepPRM-RTL: Stepwise Process-Reward Guided LLM Fine-Tuning for Enhanced RTL Synthesis**  
   [[Paper](https://arxiv.org/abs/2606.04246)] · arXiv:2606.04246  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 7.2 Reward / Fitness.

1. **Stratagem: Learning Transferable Reasoning via Trajectory-Modulated Game Self-Play**  
   [[Paper](https://arxiv.org/abs/2604.17696)] · arXiv:2604.17696  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Structured Reasoning for Large Language Models**  
   [[Paper](https://arxiv.org/abs/2601.07180)] · arXiv:2601.07180  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Synergizing Discriminative Exemplars and Self-Refined Experience for MLLM-based In-Context Learning in Medical Diagnosis**  
   [[Paper](https://arxiv.org/abs/2603.27737)] · arXiv:2603.27737  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L1. *Updated object(s):* 1.4 Prompt & Context; 2.3 Procedural Memory.

1. **Synthetic Computers at Scale for Long-Horizon Productivity Simulation**  
   [[Paper](https://arxiv.org/abs/2604.28181)] · arXiv:2604.28181  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L1. *Updated object(s):* 4.4 Skill Library; 8.3 Environment.

1. **Teach-to-Reason: Competition-Guided Reasoning with a Self-Improving Teacher**  
   [[Paper](https://arxiv.org/abs/2606.25407)] · arXiv:2606.25407  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Teaching Large Reasoning Models Effective Reflection**  
   [[Paper](https://arxiv.org/abs/2601.12720)] · arXiv:2601.12720  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Team-Based Self-Play With Dual Adaptive Weighting for Fine-Tuning LLMs**  
   [[Paper](https://arxiv.org/abs/2605.09922)] · arXiv:2605.09922  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Temporal Self-Rewarding Language Models: Decoupling Chosen-Rejected via Past-Future**  
   [[Paper](https://arxiv.org/abs/2508.06026)] · arXiv:2508.06026  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 7.1 Judge.

1. **The Attacker in the Mirror: Breaking Self-Consistency in Safety via Anchored Bipolicy Self-Play**  
   [[Paper](https://arxiv.org/abs/2605.08427)] · arXiv:2605.08427  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Think Longer to Explore Deeper: Learn to Explore In-Context via Length-Incentivized Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2602.11748)] · arXiv:2602.11748  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **Thinking Before Running! Efficient Code Generation with Thorough Exploration and Optimal Refinement**  
   [[Paper](https://arxiv.org/abs/2502.17442)] · arXiv:2502.17442  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **Training-Free Test-Time Contrastive Learning for Large Language Models**  
   [[Paper](https://arxiv.org/abs/2604.13552)] · arXiv:2604.13552  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L1. *Updated object(s):* 2.3 Procedural Memory; 1.5 Context.

1. **Transformers Provably Learn Chain-of-Thought Reasoning with Length Generalization**  
   [[Paper](https://arxiv.org/abs/2511.07378)] · arXiv:2511.07378  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Transitivity Meets Cyclicity: Explicit Preference Decomposition for Dynamic Large Language Model Alignment**  
   [[Paper](https://arxiv.org/abs/2605.17342)] · arXiv:2605.17342  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 7.2 Reward / Fitness.

1. **TRON: Targeted Rule-Verifiable Online Environments for Visual Reasoning RL**  
   [[Paper](https://arxiv.org/abs/2606.01599)] · arXiv:2606.01599  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **Unsupervised Process Reward Models**  
   [[Paper](https://arxiv.org/abs/2605.10158)] · arXiv:2605.10158  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 7.1 Judge.

1. **Utilizing and Calibrating Hindsight Process Rewards via Reinforcement with Mutual Information Self-Evaluation**  
   [[Paper](https://arxiv.org/abs/2604.11611)] · arXiv:2604.11611  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **VeriGate: Verifier-Gated Step-Level Supervision for GRPO**  
   [[Paper](https://arxiv.org/abs/2605.30451)] · arXiv:2605.30451  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **VibeThinker-3B: Exploring the Frontier of Verifiable Reasoning in Small Language Models**  
   [[Paper](https://arxiv.org/abs/2606.16140)] · arXiv:2606.16140  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **VideoSAVi: Self-Aligned Video Language Models without Human Supervision**  
   [[Paper](https://arxiv.org/abs/2412.00624)] · arXiv:2412.00624  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights.

1. **When Good Verifiers Go Bad: Self-Improving VLMs Can Regress on New Tasks**  
   [[Paper](https://arxiv.org/abs/2606.14629)] · arXiv:2606.14629  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.2 Adapter.

1. **World Model Self-Distillation: Training World Models to Solve General Tasks**  
   [[Paper](https://arxiv.org/abs/2606.12072)] · arXiv:2606.12072  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L1. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **ZAS-SQL: Distilling Rules from Failures for Zero-Shot Text-to-SQL**  
   [[Paper](https://arxiv.org/abs/2606.08245)] · arXiv:2606.08245  
   ![](https://img.shields.io/badge/-Level--L1-2563eb) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L1. *Updated object(s):* 1.3 Prompt & Context; 3.4 Harness / Workflow.

</details>

<a id="2-l2---autonomy-over-improvement-strategies"></a>

## 2. L2 - Autonomy over Improvement Strategies <sub><a href="#readme-top">↑ top</a></sub>

The system chooses how to improve a specified target, while the objective, evaluation criterion, or acceptance rule remains externally specified. **160 papers.**

### Featured representative papers

| Paper | Representative mechanism |
| --- | --- |
| [AutoPrompt](https://arxiv.org/abs/2010.15980) | Uses gradient-guided search to generate discrete prompt tokens for a fixed task. |
| [Automatic Prompt Engineer](https://arxiv.org/abs/2211.01910) | Uses an LLM to propose prompt instructions and an external evaluator to select them. |
| [ProTeGi](https://arxiv.org/abs/2305.03495) | Optimizes prompts through textual gradients and beam search. |
| [EvoPrompt](https://arxiv.org/abs/2309.08532) | Treats prompt optimization as evolutionary search. |
| [Eureka](https://arxiv.org/abs/2310.12931) | Uses LLM-guided evolutionary optimization over reward code for externally specified RL tasks. |
| [ADAS](https://arxiv.org/abs/2408.08435) | Proposes, evaluates, and archives improved agentic system designs. |
| [AFlow](https://arxiv.org/abs/2410.10762) | Searches code-represented agent workflows with execution feedback. |

<details>
<summary><strong>Browse the full L2 catalog (160 papers)</strong></summary>

### Table-derived extensions

The following additions are explicitly listed in Table 4, which groups representative L2 systems by the object of improvement-strategy search.

1. **Multimodal Prompt Optimization: Why Not Leverage Multiple Modalities for MLLMs**  
   [[Paper](https://arxiv.org/abs/2510.09201)] · arXiv:2510.09201  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_Context-7c3aed)  
   *Survey-table rationale:* Evaluation-derived semantic feedback guides multimodal prompt candidates under a fixed task metric. *Updated object(s):* 1.1 Instruction; 1.2 Task Prompt / Template.

1. **Agentic Neural Architecture Search**  
   [[Paper](https://arxiv.org/abs/2607.07984)] · arXiv:2607.07984  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Survey-table rationale:* An LLM constructs a task-specific architecture search space, but the validation metric remains fixed. *Updated object(s):* 5.3 Architecture.

1. **Auto Research with Specialist Agents Develops Effective and Non-Trivial Training Recipes**  
   [[Paper](https://arxiv.org/abs/2605.05724)] · arXiv:2605.05724  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Trainer_Optimization-c2410c)  
   *Survey-table rationale:* Specialist agents search over training recipes with a shared lineage under an external evaluator. *Updated object(s):* 6.5 Search / Meta-optimization Procedure.

1. **AutoKernel: Autonomous GPU Kernel Optimization via Iterative Agent-Driven Search**  
   [[Paper](https://arxiv.org/abs/2603.21331)] · arXiv:2603.21331  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Survey-table rationale:* A profile-rewrite-benchmark loop searches kernel implementations under fixed correctness and speed criteria. *Updated object(s):* 9.1 Program / Solution Code.

1. **Adapting AlphaEvolve to Optimize Fully Homomorphic Encryption on TPUs**  
   [[Paper](https://arxiv.org/abs/2605.14718)] · arXiv:2605.14718  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **AI-PROPELLER: Warehouse-Scale Interprocedural Code Layout Optimization with AlphaEvolve**  
   [[Paper](https://arxiv.org/abs/2606.00131)] · arXiv:2606.00131  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm.

1. **Magellan: Autonomous Discovery of Novel Compiler Optimization Heuristics with AlphaEvolve**  
   [[Paper](https://arxiv.org/abs/2601.21096)] · arXiv:2601.21096  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **Scientific Algorithm Discovery by Augmenting AlphaEvolve with Deep Research**  
   [[Paper](https://arxiv.org/abs/2510.06056)] · arXiv:2510.06056  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm; 2.1 Experience Memory.


1. **A Self-Improving Coding Agent**  
   [[Paper](https://arxiv.org/abs/2504.15228)] · arXiv:2504.15228  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.6 Scaffold Code; 4.3 Tool Code; 1.1 Instruction.

1. **Adaptive Self-improvement LLM Agentic System for ML Library Development**  
   [[Paper](https://arxiv.org/abs/2502.02534)] · arXiv:2502.02534  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.4 Prompt & Context; 1.5 Context.

1. **Advanced For-Loop for QML algorithm search**  
   [[Paper](https://arxiv.org/abs/2506.18260)] · arXiv:2506.18260  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm; 9.1 Program Code.

1. **AFlow: Automating Agentic Workflow Generation**  
   [[Paper](https://arxiv.org/abs/2410.10762)] · arXiv:2410.10762  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.6 Scaffold Code; 1.2 Task Prompt.

1. **AgentDisCo: Towards Disentanglement and Collaboration in Open-ended Deep Research Agents**  
   [[Paper](https://arxiv.org/abs/2605.11732)] · arXiv:2605.11732  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction; 3.6 Scaffold Code.

1. **Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models**  
   [[Paper](https://arxiv.org/abs/2510.04618)] · arXiv:2510.04618  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.5 Context; 2.4 Memory & Knowledge.

1. **Agentic Discovery of Neural Architectures: AIRA-Compose and AIRA-Design**  
   [[Paper](https://arxiv.org/abs/2605.15871)] · arXiv:2605.15871  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm; 9.3 External Artifact.

1. **Agentic Harness Engineering: Observability-Driven Automatic Evolution of Coding-Agent Harnesses**  
   [[Paper](https://arxiv.org/abs/2604.25850)] · arXiv:2604.25850  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.6 Scaffold Code; 4.3 Tool Code.

1. **Agentic MIP Research: Accelerated Constraint Handler Generation**  
   [[Paper](https://arxiv.org/abs/2605.09186)] · arXiv:2605.09186  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 9.2 Algorithm.

1. **AgenticRL: Self-Refining Agentic Reinforcement Learning for Vision-Conditioned UAV Navigation**  
   [[Paper](https://arxiv.org/abs/2606.03963)] · arXiv:2606.03963  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Trainer___Optimization-c2410c)  
   *Taxonomy:* L2. *Updated object(s):* 6.1 Objective; 5.1 Model Weights.

1. **Ask, Don't Judge: Binary Questions for Interpretable LLM Evaluation and Self-Improvement**  
   [[Paper](https://arxiv.org/abs/2606.27226)] · arXiv:2606.27226  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction.

1. **ASPIRE: Agentic Skills Discovery for Robotics**  
   [[Paper](https://arxiv.org/abs/2607.00272)] · arXiv:2607.00272  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library; 9.1 Program Code.

1. **Auto-Configuring Scientific Simulators with Lightweight Coding-Agent Adapters**  
   [[Paper](https://arxiv.org/abs/2606.09774)] · arXiv:2606.09774  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.3 Procedural Memory; 1.1 Instruction; 4.4 Skill Library.

1. **Automated Design of Agentic Systems (ADAS)**  
   [[Paper](https://arxiv.org/abs/2408.08435)] · arXiv:2408.08435  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.6 Scaffold Code.

1. **Automated Heuristic Design for Unit Commitment Using Large Language Models**  
   [[Paper](https://arxiv.org/abs/2506.12495)] · arXiv:2506.12495  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm; 9.1 Program Code.

1. **AutoMegaKernel: A Statically-Checked Agent Harness for Self-Retargeting Megakernel Synthesis**  
   [[Paper](https://arxiv.org/abs/2606.09682)] · arXiv:2606.09682  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **AutoPass: Evidence-Guided LLM Agents for Compiler Performance Tuning**  
   [[Paper](https://arxiv.org/abs/2606.20373)] · arXiv:2606.20373  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm.

1. **AutoPrompt: Eliciting Knowledge from Language Models with Automatically Generated Prompts**  
   [[Paper](https://arxiv.org/abs/2010.15980)] · arXiv:2010.15980  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt.

1. **AutoPyVerifier: Learning Compact Executable Verifiers for Large Language Model Outputs**  
   [[Paper](https://arxiv.org/abs/2604.22937)] · arXiv:2604.22937  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L2. *Updated object(s):* 7.3 Verifier; 7.1 Judge.

1. **AutoVQA-G: Self-Improving Agentic Framework for Automated Visual Question Answering and Grounding Annotation**  
   [[Paper](https://arxiv.org/abs/2604.17488)] · arXiv:2604.17488  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt; 1.1 Instruction.

1. **Beyond Algorithm Evolution: An LLM-Driven Framework for the Co-Evolution of Swarm Intelligence Optimization Algorithms and Prompts**  
   [[Paper](https://arxiv.org/abs/2512.09209)] · arXiv:2512.09209  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm; 1.1 Instruction.

1. **Beyond Scalar Rewards: Dense Feedback for LLM Policy Synthesis in Sequential Social Dilemmas**  
   [[Paper](https://arxiv.org/abs/2603.19453)] · arXiv:2603.19453  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **Beyond Static Tools: Test-Time Tool Evolution for Scientific Reasoning**  
   [[Paper](https://arxiv.org/abs/2601.07641)] · arXiv:2601.07641  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.1 Tool Set; 4.2 Tool Interface.

1. **BT-APE: A Computationally Light Backtracking Approach to Automatic Prompt Engineering for Requirements Classification**  
   [[Paper](https://arxiv.org/abs/2607.00427)] · arXiv:2607.00427  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt.

1. **CausalEvolve: Towards Open-Ended Discovery with Causal Scratchpad**  
   [[Paper](https://arxiv.org/abs/2603.14575)] · arXiv:2603.14575  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 2.1 Experience Memory.

1. **CHIA: An open-source framework for principled, agentic AI-driven hardware/software co-design research**  
   [[Paper](https://arxiv.org/abs/2606.27350)] · arXiv:2606.27350  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **Co-evolving Agent Architectures and Interpretable Reasoning for Automated Optimization**  
   [[Paper](https://arxiv.org/abs/2604.17708)] · arXiv:2604.17708  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.1 Workflow; 2.2 Knowledge Memory.

1. **CodeEvolve: an open source evolutionary coding agent for algorithmic discovery and optimization**  
   [[Paper](https://arxiv.org/abs/2510.14150)] · arXiv:2510.14150  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 1.2 Task Prompt.

1. **CoEvoSkills: Self-Evolving Agent Skills via Co-Evolutionary Verification**  
   [[Paper](https://arxiv.org/abs/2604.01687)] · arXiv:2604.01687  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library.

1. **Combee: Scaling Prompt Learning for Self-Improving Language Model Agents**  
   [[Paper](https://arxiv.org/abs/2604.04247)] · arXiv:2604.04247  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction; 1.5 Context.

1. **Combining Large Language Models and Gradient-Free Optimization for Automatic Control Policy Synthesis**  
   [[Paper](https://arxiv.org/abs/2510.00373)] · arXiv:2510.00373  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **Competing with AI Scientists: Agent-Driven Approach to Astrophysics Research**  
   [[Paper](https://arxiv.org/abs/2604.09621)] · arXiv:2604.09621  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **Continually self-improving AI**  
   [[Paper](https://arxiv.org/abs/2603.18073)] · arXiv:2603.18073  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Trainer___Optimization-c2410c)  
   *Taxonomy:* L2. *Updated object(s):* 6.5 Meta-optimization; 6.1 Objective; 5.1 Model Weights.

1. **CORAL: Towards Autonomous Multi-Agent Evolution for Open-Ended Discovery**  
   [[Paper](https://arxiv.org/abs/2604.01658)] · arXiv:2604.01658  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 4.4 Skill Library.

1. **DataEvolver: Automatic Data Preparation for Large Language Models through Multi-Level Self-Evolving**  
   [[Paper](https://arxiv.org/abs/2606.07001)] · arXiv:2606.07001  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L2. *Updated object(s):* 8.1 Experience Data; 9.1 Program Code.

1. **Defining Cost Function of Steganography with Large Language Models**  
   [[Paper](https://arxiv.org/abs/2512.09769)] · arXiv:2512.09769  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm.

1. **DeltaEvolve: Accelerating Scientific Discovery through Momentum-Driven Evolution**  
   [[Paper](https://arxiv.org/abs/2602.02919)] · arXiv:2602.02919  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **Discovering Multiagent Learning Algorithms with Large Language Models**  
   [[Paper](https://arxiv.org/abs/2602.16928)] · arXiv:2602.16928  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm.

1. **DrugSAGE: Self-evolving Agent Experience for Efficient State-of-the-Art Drug Discovery**  
   [[Paper](https://arxiv.org/abs/2605.15461)] · arXiv:2605.15461  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library; 2.2 Knowledge Memory.

1. **Each Judge Its Own Yardstick: Discovering Per-VLM Taxonomies for Physical Video Evaluation**  
   [[Paper](https://arxiv.org/abs/2606.22918)] · arXiv:2606.22918  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L2. *Updated object(s):* 7.1 Judge.

1. **EEVEE: Towards Test-time Prompt Learning in the Real World for Self-Improving Agents**  
   [[Paper](https://arxiv.org/abs/2606.11182)] · arXiv:2606.11182  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction; 3.3 Harness / Workflow.

1. **Effective Harness Engineering for Algorithm Discovery with Coding Agents**  
   [[Paper](https://arxiv.org/abs/2605.15221)] · arXiv:2605.15221  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 9.2 Algorithm.

1. **ELMES+: Automated Construction of Fine-Grained Evaluation Rubrics for Large Language Models in Long-Tail Educational Scenarios**  
   [[Paper](https://arxiv.org/abs/2606.06546)] · arXiv:2606.06546  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L2. *Updated object(s):* 7.1 Judge; 8.2 Task Generator.

1. **EmbodiSkill: Skill-Aware Reflection for Self-Evolving Embodied Agents**  
   [[Paper](https://arxiv.org/abs/2605.10332)] · arXiv:2605.10332  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library.

1. **Enhancing Operational Safety via Agentic Dialogue Hazard Identification Analysis**  
   [[Paper](https://arxiv.org/abs/2606.03812)] · arXiv:2606.03812  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.5 Multi-agent; 1.1 Instruction.

1. **Environment-Grounded Automated Prompt Optimization for LLM Game Agents**  
   [[Paper](https://arxiv.org/abs/2606.17838)] · arXiv:2606.17838  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction; 1.2 Task Prompt.

1. **EpiAgent: An Agent-Centric System for Ancient Inscription Restoration**  
   [[Paper](https://arxiv.org/abs/2604.09367)] · arXiv:2604.09367  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.1 Experience Memory; 2.3 Procedural Memory.

1. **Eureka: Human-Level Reward Design via Coding Large Language Models**  
   [[Paper](https://arxiv.org/abs/2310.12931)] · arXiv:2310.12931  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L2. *Updated object(s):* 7.2 Reward / Fitness.

1. **Eureka: Intelligent Feature Engineering for Enterprise AI Cloud Resource Demand Prediction**  
   [[Paper](https://arxiv.org/abs/2605.25297)] · arXiv:2605.25297  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 5.1 Model Weights.

1. **EvoClinician: A Self-Evolving Agent for Multi-Turn Medical Diagnosis via Test-Time Evolutionary Learning**  
   [[Paper](https://arxiv.org/abs/2601.22964)] · arXiv:2601.22964  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction; 2.1 Experience Memory.

1. **EvoLattice: Persistent Internal-Population Evolution through Multi-Alternative Quality-Diversity Graph Representations for LLM-Guided Program Discovery**  
   [[Paper](https://arxiv.org/abs/2512.13857)] · arXiv:2512.13857  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 9.2 Algorithm.

1. **Evolution of Heuristics: Towards Efficient Automatic Algorithm Design Using Large Language Model**  
   [[Paper](https://arxiv.org/abs/2401.02051)] · arXiv:2401.02051  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm; 9.1 Program Code.

1. **EvolveSignal: A Large Language Model Powered Coding Agent for Discovering Traffic Signal Control Strategies**  
   [[Paper](https://arxiv.org/abs/2509.03335)] · arXiv:2509.03335  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **Evolving Deception: When Agents Evolve, Deception Wins**  
   [[Paper](https://arxiv.org/abs/2603.05872)] · arXiv:2603.05872  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction.

1. **Evolving Medical Imaging Agents via Experience-Driven Self-Skill Discovery**  
   [[Paper](https://arxiv.org/abs/2603.05860)] · arXiv:2603.05860  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library; 5.1 Model Weights; 2.1 Experience Memory.

1. **EVOM: Agentic Meta-Evolution of Actor-Critic Architectures for Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2606.26327)] · arXiv:2606.26327  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L2. *Updated object(s):* 5.3 Architecture.

1. **EvoPrompt: Connecting LLMs with Evolutionary Algorithms Yields Powerful Prompt Optimizers**  
   [[Paper](https://arxiv.org/abs/2309.08532)] · arXiv:2309.08532  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt.

1. **EvoScientist: Towards Multi-Agent Evolving AI Scientists for End-to-End Scientific Discovery**  
   [[Paper](https://arxiv.org/abs/2603.08127)] · arXiv:2603.08127  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.2 Knowledge Memory; 1.5 Context.

1. **EvoTest: Evolutionary Test-Time Learning for Self-Improving Agentic Systems**  
   [[Paper](https://arxiv.org/abs/2510.13220)] · arXiv:2510.13220  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction; 2.1 Experience Memory; 5.4 Model.

1. **Experience Graphs: The Data Foundation for Self-Improving Agents**  
   [[Paper](https://arxiv.org/abs/2606.29823)] · arXiv:2606.29823  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.1 Experience Memory; 2.4 Memory & Knowledge.

1. **Experience Makes Skillful: Enabling Generalizable Medical Agent Reasoning via Self-Evolving Skill Memory**  
   [[Paper](https://arxiv.org/abs/2606.09365)] · arXiv:2606.09365  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.3 Procedural Memory; 2.5 Memory & Knowledge.

1. **ExpGraph: Model-Agnostic Experience Learning with Graph-Structured Memory for LLM Agents**  
   [[Paper](https://arxiv.org/abs/2605.30712)] · arXiv:2605.30712  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.1 Experience Memory; 2.4 Memory & Knowledge; 5.2 Adapter.

1. **FederatedSkill: Federated Learning for Agentic Skill Evolution**  
   [[Paper](https://arxiv.org/abs/2606.03143)] · arXiv:2606.03143  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library; 2.2 Knowledge Memory.

1. **Feedback Over Form: Why Execution Feedback Matters More Than Pipeline Topology in 1-3B Code Generation**  
   [[Paper](https://arxiv.org/abs/2604.21950)] · arXiv:2604.21950  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.1 Workflow.

1. **Feedback-to-Rubrics: Can We Learn Expert Criteria from Inline Comments?**  
   [[Paper](https://arxiv.org/abs/2605.29857)] · arXiv:2605.29857  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L2. *Updated object(s):* 7.1 Judge; 1.1 Instruction.

1. **From AI Assistant to AI Scientist: Autonomous Discovery of LLM-RL Algorithms with LLM Agents**  
   [[Paper](https://arxiv.org/abs/2603.23951)] · arXiv:2603.23951  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Trainer___Optimization-c2410c)  
   *Taxonomy:* L2. *Updated object(s):* 6.1 Objective; 6.2 Trainer / Optimization.

1. **From Failed Trajectories to Reliable LLM Agents: Diagnosing and Repairing Harness Flaws**  
   [[Paper](https://arxiv.org/abs/2606.06324)] · arXiv:2606.06324  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.6 Scaffold Code; 1.2 Task Prompt; 4.2 Tool Interface.

1. **From Self-Evolving Synthetic Data to Verifiable-Reward RL: Post-Training Multi-turn Interactive Tool-Using Agents**  
   [[Paper](https://arxiv.org/abs/2601.22607)] · arXiv:2601.22607  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L2. *Updated object(s):* 8.1 Experience Data; 5.1 Model Weights.

1. **From Understanding to Excelling: Template-Free Algorithm Design through Structural-Functional Co-Evolution**  
   [[Paper](https://arxiv.org/abs/2503.10721)] · arXiv:2503.10721  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 9.2 Algorithm; 6.5 Meta-optimization.

1. **From User Interface to Agent Interface: Efficiency Optimization of UI Representations for LLM Agents**  
   [[Paper](https://arxiv.org/abs/2512.13438)] · arXiv:2512.13438  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **FuzzAgent: Multi-Agent System for Evolutionary Library Fuzzing**  
   [[Paper](https://arxiv.org/abs/2605.14431)] · arXiv:2605.14431  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **GeoEvolve: Automating Geospatial Model Discovery via Multi-Agent Large Language Models**  
   [[Paper](https://arxiv.org/abs/2509.21593)] · arXiv:2509.21593  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm.

1. **GEPA: Reflective Prompt Evolution Can Outperform Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2507.19457)] · arXiv:2507.19457  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction.

1. **GigaEvo: An Open Source Optimization Framework Powered By LLMs And Evolution Algorithms**  
   [[Paper](https://arxiv.org/abs/2511.17592)] · arXiv:2511.17592  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm; 9.1 Program Code; 1.1 Instruction.

1. **Hardening Agent Benchmarks with Adversarial Hacker-Fixer Loops**  
   [[Paper](https://arxiv.org/abs/2606.08960)] · arXiv:2606.08960  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L2. *Updated object(s):* 7.3 Verifier; 8.3 Environment.

1. **Healthcare Mechanisms from Policy-as-Code Search under Strategic Provider Response**  
   [[Paper](https://arxiv.org/abs/2605.30680)] · arXiv:2605.30680  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm.

1. **Heuresis: Search Strategies for Autonomous AI Research Agents Across Quality, Diversity and Novelty**  
   [[Paper](https://arxiv.org/abs/2606.25198)] · arXiv:2606.25198  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 9.2 Algorithm.

1. **Hierarchical Experimentalist Agents**  
   [[Paper](https://arxiv.org/abs/2606.29315)] · arXiv:2606.29315  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library.

1. **HSEvo: Elevating Automatic Heuristic Design with Diversity-Driven Harmony Search and Genetic Algorithm Using LLMs**  
   [[Paper](https://arxiv.org/abs/2412.14995)] · arXiv:2412.14995  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 6.5 Meta-optimization.

1. **HypoForge: A Self-Improving Multi-Agent Framework for Automated Hypothesis Generation and Testing via Scientific Skill Learning**  
   [[Paper](https://arxiv.org/abs/2608.25770)] · arXiv:2608.25770  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library.

1. **ImprovEvolve: Basin-Hopping Meets LLM-Guided Evolutionary Search**  
   [[Paper](https://arxiv.org/abs/2602.10233)] · arXiv:2602.10233  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 9.2 Algorithm.

1. **InvEvolve: Evolving White-Box Inventory Policies via Large Language Models with Performance Guarantees**  
   [[Paper](https://arxiv.org/abs/2605.00369)] · arXiv:2605.00369  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 5.1 Model Weights.

1. **ISM: Self-Improving Strategy Memory for Continual Mathematical Reasoning**  
   [[Paper](https://arxiv.org/abs/2606.31191)] · arXiv:2606.31191  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.3 Procedural Memory; 2.4 Memory & Knowledge.

1. **IterInject: Indirect Prompt Injection Against LLM Agents via Feedback-Guided Iterative Optimization**  
   [[Paper](https://arxiv.org/abs/2605.24659)] · arXiv:2605.24659  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt.

1. **Kernel Foundry: A Diagnosis-driven Evolutionary Kernel Optimizer with Multi-Experts**  
   [[Paper](https://arxiv.org/abs/2605.30359)] · arXiv:2605.30359  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 2.3 Procedural Memory.

1. **Large Language Models Are Human-Level Prompt Engineers (Automatic Prompt Engineer, APE)**  
   [[Paper](https://arxiv.org/abs/2211.01910)] · arXiv:2211.01910  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction.

1. **Large Language Models as Optimizers**  
   [[Paper](https://arxiv.org/abs/2309.03409)] · arXiv:2309.03409  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt.

1. **Learning from Failure: Inference-Time Self-Improvement for Computer-Use Agents**  
   [[Paper](https://arxiv.org/abs/2606.31270)] · arXiv:2606.31270  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.6 Scaffold Code; 4.1 Tool Set; 3.4 Harness / Workflow.

1. **Learning to Choose: An Empowerment-Guided Multi-Agent System with semantic communication for Adaptive Method Selection**  
   [[Paper](https://arxiv.org/abs/2605.30042)] · arXiv:2605.30042  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.3 Harness / Workflow; 2.1 Experience Memory.

1. **LEVI: Stronger Search Architectures Can Substitute for Larger LLMs in Evolutionary Search**  
   [[Paper](https://arxiv.org/abs/2605.09764)] · arXiv:2605.09764  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 1.2 Task Prompt.

1. **Libra: Training the Environment for Agentic Information Retrieval**  
   [[Paper](https://arxiv.org/abs/2607.00016)] · arXiv:2607.00016  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.2 Knowledge Memory; 8.3 Environment.

1. **LLaMEA-BO: A Large Language Model Evolutionary Algorithm for Automatically Generating Bayesian Optimization Algorithms**  
   [[Paper](https://arxiv.org/abs/2505.21034)] · arXiv:2505.21034  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm; 9.1 Program Code.

1. **LLM as a Tool, Not an Agent: Code-Mined Tree Transformations for Neural Architecture Search**  
   [[Paper](https://arxiv.org/abs/2604.16555)] · arXiv:2604.16555  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.3 External Artifact.

1. **LLM-Evolved Pattern Generators for Optimal Classical Planning**  
   [[Paper](https://arxiv.org/abs/2606.02438)] · arXiv:2606.02438  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **LLM-Guided Evolutionary Program Synthesis for Quasi-Monte Carlo Design**  
   [[Paper](https://arxiv.org/abs/2510.03650)] · arXiv:2510.03650  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm.

1. **LLM-Guided Search for Deletion-Correcting Codes**  
   [[Paper](https://arxiv.org/abs/2504.00613)] · arXiv:2504.00613  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm.

1. **LoongFlow: Directed Evolutionary Search via a Cognitive Plan-Execute-Summarize Paradigm**  
   [[Paper](https://arxiv.org/abs/2512.24077)] · arXiv:2512.24077  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm; 9.1 Program Code.

1. **Mathematical exploration and discovery at scale**  
   [[Paper](https://arxiv.org/abs/2511.02864)] · arXiv:2511.02864  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 9.2 Algorithm.

1. **Mechanistically Eliciting Latent Behaviors in Language Models**  
   [[Paper](https://arxiv.org/abs/2606.29604)] · arXiv:2606.29604  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L2. *Updated object(s):* 5.2 Adapter.

1. **Medical Heuristic Learning: An LLM-Driven Framework for Interpretable and Auditable Clinical Decision Rules**  
   [[Paper](https://arxiv.org/abs/2606.16337)] · arXiv:2606.16337  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **MEMENTO: Leveraging Web as a Learning Signal for Low-Data Domains**  
   [[Paper](https://arxiv.org/abs/2605.29795)] · arXiv:2605.29795  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.3 Procedural Memory; 2.2 Knowledge Memory.

1. **MEMO: Memory-Augmented Model Context Optimization for Robust Multi-Turn Multi-Agent LLM Games**  
   [[Paper](https://arxiv.org/abs/2603.09022)] · arXiv:2603.09022  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt; 2.2 Knowledge Memory.

1. **Meta-Harness: End-to-End Optimization of Model Harnesses**  
   [[Paper](https://arxiv.org/abs/2603.28052)] · arXiv:2603.28052  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.6 Scaffold Code.

1. **Middo: Model-Informed Dynamic Data Optimization for Enhanced LLM Fine-Tuning via Closed-Loop Learning**  
   [[Paper](https://arxiv.org/abs/2508.21589)] · arXiv:2508.21589  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L2. *Updated object(s):* 8.1 Experience Data; 5.1 Model Weights.

1. **Mining Generalizable Activation Functions**  
   [[Paper](https://arxiv.org/abs/2602.05688)] · arXiv:2602.05688  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm.

1. **MLEvolve: A Self-Evolving Framework for Automated Machine Learning Algorithm Discovery**  
   [[Paper](https://arxiv.org/abs/2606.06473)] · arXiv:2606.06473  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 9.2 Algorithm.

1. **MobEvolve: An Agentic Self-Evolving Heuristic System for Interpretable Human Mobility Generation**  
   [[Paper](https://arxiv.org/abs/2606.01640)] · arXiv:2606.01640  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 2.1 Experience Memory.

1. **OpenComputer: Verifiable Software Worlds for Computer-Use Agents**  
   [[Paper](https://arxiv.org/abs/2605.19769)] · arXiv:2605.19769  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L2. *Updated object(s):* 7.3 Verifier; 8.1 Experience Data; 8.3 Environment.

1. **Organize then Retrieve: Hierarchical Memory Navigation for Efficient Agents**  
   [[Paper](https://arxiv.org/abs/2606.11680)] · arXiv:2606.11680  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library; 5.1 Model Weights.

1. **PACEvolve++: Improving Test-time Learning for Evolutionary Search Agents**  
   [[Paper](https://arxiv.org/abs/2605.07039)] · arXiv:2605.07039  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L2. *Updated object(s):* 5.1 Model Weights; 9.1 Program Code.

1. **Persona Generators: Generating Diverse Synthetic Personas for Arbitrary Contexts**  
   [[Paper](https://arxiv.org/abs/2602.03545)] · arXiv:2602.03545  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **Polaris: A Gödel Agent Framework for Small Language Models through Experience-Abstracted Policy Repair**  
   [[Paper](https://arxiv.org/abs/2603.23129)] · arXiv:2603.23129  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.6 Scaffold Code; 2.3 Procedural Memory.

1. **ProfiLLM: Utility-Aligned Agentic User Profiling for Industrial Ride-Hailing Dispatch**  
   [[Paper](https://arxiv.org/abs/2606.18803)] · arXiv:2606.18803  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L2. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **PromptAgent: Strategic Planning with Language Models Enables Expert-level Prompt Optimization**  
   [[Paper](https://arxiv.org/abs/2310.16427)] · arXiv:2310.16427  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt.

1. **PromptWizard: Task-Aware Prompt Optimization Framework**  
   [[Paper](https://arxiv.org/abs/2405.18369)] · arXiv:2405.18369  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction; 1.4 Prompt & Context.

1. **ProTeGi: Automatic Prompt Optimization with 'Gradient Descent' and Beam Search**  
   [[Paper](https://arxiv.org/abs/2305.03495)] · arXiv:2305.03495  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt.

1. **PYTHALAB-MERA: Validation-Grounded Memory, Retrieval, and Acceptance Control for Frozen-LLM Coding Agents**  
   [[Paper](https://arxiv.org/abs/2605.08468)] · arXiv:2605.08468  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.1 Experience Memory; 1.5 Context; 4.4 Skill Library.

1. **QUBE: Enhancing Automatic Heuristic Design via Quality-Uncertainty Balanced Evolution**  
   [[Paper](https://arxiv.org/abs/2412.20694)] · arXiv:2412.20694  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 6.5 Meta-optimization.

1. **QueenBee Planner: Skill-Evolving Communication Topologies for Token-Efficient LLM Multi-Agent Systems**  
   [[Paper](https://arxiv.org/abs/2606.27492)] · arXiv:2606.27492  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.3 Procedural Memory; 3.5 Multi-agent.

1. **RankEvolve: Automating the Discovery of Retrieval Algorithms via LLM-Driven Evolution**  
   [[Paper](https://arxiv.org/abs/2602.16932)] · arXiv:2602.16932  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.2 Algorithm.

1. **Recursive Harness Self-Improvement**  
   [[Paper](https://arxiv.org/abs/2607.15524)] · arXiv:2607.15524  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.1 Workflow; 3.5 Multi-agent.

1. **Reflection-Based Task Adaptation for Self-Improving VLA**  
   [[Paper](https://arxiv.org/abs/2510.12710)] · arXiv:2510.12710  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L2. *Updated object(s):* 5.1 Model Weights; 7.2 Reward / Fitness; 6.4 Curriculum.

1. **REFLEX: Reflective Evolution from LLM Experience**  
   [[Paper](https://arxiv.org/abs/2606.16496)] · arXiv:2606.16496  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 4.4 Skill Library.

1. **Repeated post-training is not Self-improving: Diagnosing Scientific Amnesia in Continual DPO Pipelines**  
   [[Paper](https://arxiv.org/abs/2606.21089)] · arXiv:2606.21089  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L2. *Updated object(s):* 5.1 Model Weights; 6.5 Meta-optimization.

1. **Rethinking Code Similarity for Automated Algorithm Design with LLMs**  
   [[Paper](https://arxiv.org/abs/2603.02787)] · arXiv:2603.02787  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L2. *Updated object(s):* 7.2 Reward / Fitness; 3.6 Scaffold Code.

1. **Revisiting OPRO: The Limitations of Small-Scale LLMs as Optimizers**  
   [[Paper](https://arxiv.org/abs/2405.10276)] · arXiv:2405.10276  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt.

1. **RLPrompt: Optimizing Discrete Text Prompts with Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2205.12548)] · arXiv:2205.12548  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt.

1. **S1-NexusAgent: a Self-Evolving Agent Framework for Multidisciplinary Scientific Research**  
   [[Paper](https://arxiv.org/abs/2602.01550)] · arXiv:2602.01550  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library.

1. **Self-Consolidating Language Models: Continual Knowledge Incorporation from Context**  
   [[Paper](https://arxiv.org/abs/2605.07076)] · arXiv:2605.07076  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L2. *Updated object(s):* 5.1 Model Weights; 5.2 Adapter.

1. **Self-Harness: Harnesses That Improve Themselves**  
   [[Paper](https://arxiv.org/abs/2606.09498)] · arXiv:2606.09498  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L2. *Updated object(s):* 3.6 Scaffold Code; 1.1 Instruction.

1. **Self-Improvement Can Self-Regress: The Rise-and-Collapse Failure Mode of LLM Self-Training**  
   [[Paper](https://arxiv.org/abs/2606.21090)] · arXiv:2606.21090  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L2. *Updated object(s):* 5.1 Model Weights; 6.5 Meta-optimization.

1. **SePO: Self-Evolving Prompt Agent for System Prompt Optimization**  
   [[Paper](https://arxiv.org/abs/2606.04465)] · arXiv:2606.04465  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.2 Task Prompt; 1.1 Instruction.

1. **SGM: A Statistical Godel Machine for Risk-Controlled Recursive Self-Modification**  
   [[Paper](https://arxiv.org/abs/2510.10232)] · arXiv:2510.10232  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Trainer___Optimization-c2410c)  
   *Taxonomy:* L2. *Updated object(s):* 6.3 Train Schedule.

1. **SHARP: A Self-Evolving Human-Auditable Rubric Policy for Financial Trading Agents**  
   [[Paper](https://arxiv.org/abs/2605.06822)] · arXiv:2605.06822  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction.

1. **SIA: Self Improving AI with Harness & Weight Updates**  
   [[Paper](https://arxiv.org/abs/2605.27276)] · arXiv:2605.27276  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Full--system___Co--evolution-be123c)  
   *Taxonomy:* L2. *Updated object(s):* 10.2 Full-system / Co-evolution; 3.6 Scaffold Code; 5.1 Model Weights.

1. **SignalClaw: LLM-Guided Evolutionary Synthesis of Interpretable Traffic Signal Control Skills**  
   [[Paper](https://arxiv.org/abs/2604.05535)] · arXiv:2604.05535  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 4.4 Skill Library.

1. **Skill-R1: Agent Skill Evolution via Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2605.09359)] · arXiv:2605.09359  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library; 5.1 Model Weights.

1. **SkillCoach: Self-Evolving Rubrics for Evaluating and Enhancing Agentic Skill-Use**  
   [[Paper](https://arxiv.org/abs/2607.01874)] · arXiv:2607.01874  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L2. *Updated object(s):* 7.1 Judge; 5.1 Model Weights; 6.4 Curriculum.

1. **SkillMaster: Toward Autonomous Skill Mastery in LLM Agents**  
   [[Paper](https://arxiv.org/abs/2605.08693)] · arXiv:2605.08693  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library; 5.1 Model Weights.

1. **SkillRevise: Improving LLM-Authored Agent Skills via Trace-Conditioned Skill Revision**  
   [[Paper](https://arxiv.org/abs/2606.01139)] · arXiv:2606.01139  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library.

1. **SkillSmith: Co-Evolving Skills and Tools for Self-Improving Agent Systems**  
   [[Paper](https://arxiv.org/abs/2606.01314)] · arXiv:2606.01314  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library; 4.3 Tool Code; 2.1 Experience Memory.

1. **SOCIA-EVO: Automated Simulator Construction via Dual-Anchored Bi-Level Optimization**  
   [[Paper](https://arxiv.org/abs/2604.17351)] · arXiv:2604.17351  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.2 Knowledge Memory; 9.1 Program Code.

1. **Support Vector Rubrics: Closing the Gap Between Self-Generated and Human Rubrics**  
   [[Paper](https://arxiv.org/abs/2606.08077)] · arXiv:2606.08077  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L2. *Updated object(s):* 7.1 Judge; 1.3 Prompt & Context.

1. **Taming I2V models for Image HOI Editing: A Cognitive Benchmark and Agentic Self-Correcting Framework**  
   [[Paper](https://arxiv.org/abs/2606.19073)] · arXiv:2606.19073  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.2 Knowledge Memory; 1.2 Task Prompt.

1. **The Time is Here for Just-in-Time Systems: Challenges and Opportunities**  
   [[Paper](https://arxiv.org/abs/2605.24096)] · arXiv:2605.24096  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

1. **Towards AGI A Pragmatic Approach Towards Self Evolving Agent**  
   [[Paper](https://arxiv.org/abs/2601.11658)] · arXiv:2601.11658  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.1 Tool Set; 5.1 Model Weights.

1. **Trajectory-Informed Memory Generation for Self-Improving Agent Systems**  
   [[Paper](https://arxiv.org/abs/2603.10600)] · arXiv:2603.10600  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L2. *Updated object(s):* 2.3 Procedural Memory; 1.5 Context.

1. **Understanding the Challenges in Iterative Generative Optimization with LLMs**  
   [[Paper](https://arxiv.org/abs/2603.23994)] · arXiv:2603.23994  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code; 1.2 Task Prompt; 3.6 Scaffold Code.

1. **Unifying Temporal and Structural Credit Assignment in LLM-Based Multi-Agent Prompt Optimization**  
   [[Paper](https://arxiv.org/abs/2605.30227)] · arXiv:2605.30227  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L2. *Updated object(s):* 1.1 Instruction.

1. **VASO: Formally Verifiable Self-Evolving Skills for Physical AI Agents**  
   [[Paper](https://arxiv.org/abs/2606.05395)] · arXiv:2606.05395  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L2. *Updated object(s):* 4.4 Skill Library; 4.2 Tool Interface.

1. **When LLM Reward Design Fails: Diagnostic-Driven Refinement for Sparse Structured RL**  
   [[Paper](https://arxiv.org/abs/2605.28918)] · arXiv:2605.28918  
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L2. *Updated object(s):* 9.1 Program Code.

### Independently screened addition (2026-09-24)

1. **Language Agents as Optimizable Graphs (GPTSwarm)**<br>
   [[Paper](https://arxiv.org/abs/2402.16823)] · arXiv:2402.16823<br>
   ![](https://img.shields.io/badge/-Level--L2-7c3aed) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)<br>
   *Editorial rationale:* Task feedback updates agent-graph connections and node prompts across optimization rounds; the task utility and optimization procedures remain externally specified. *Updated object(s):* 3.1 Workflow / Graph; 1.2 Task Prompt / Template.

</details>

<a id="3-l3---autonomy-over-future-learning-experience"></a>

## 3. L3 - Autonomy over Future Learning Experience <sub><a href="#readme-top">↑ top</a></sub>

The learner's evolving state influences the experience, task, or curriculum acquired next. **65 papers.**

### Featured representative papers

| Paper | Representative mechanism |
| --- | --- |
| [POET](https://arxiv.org/abs/1901.01753) | Co-evolves environments and solvers to generate an expanding adaptive curriculum. |
| [Voyager](https://arxiv.org/abs/2305.16291) | Couples automatic curricula with a persistent skill library for open-ended embodied learning. |
| [EnvGen](https://arxiv.org/abs/2403.12014) | Generates and adapts training environments for embodied agents. |
| [Absolute Zero](https://arxiv.org/abs/2505.03335) | Lets a single model propose and solve code-grounded tasks, with a code executor verifying both tasks and answers. |
| [R-Zero](https://arxiv.org/abs/2508.05004) | Co-evolves task proposal and solving to create new learning experience from zero data. |
| [SIMA 2](https://arxiv.org/abs/2512.04797) | Uses Gemini to generate tasks and rewards so the agent can autonomously learn skills in a new virtual environment. |

<details>
<summary><strong>Browse the full L3 catalog (65 papers)</strong></summary>

### Table-derived extension

Table 5 identifies the following learner-conditioned future-experience loop, complementary to the self-play and autonomous-practice systems already in this section.

1. **SIMA 2: A Generalist Embodied Agent for Virtual Worlds**  
   [[Paper](https://arxiv.org/abs/2512.04797)] · arXiv:2512.04797  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_Environment-ca8a04)  
   *Survey-table rationale:* In the full ASKA setting, evaluation feedback directs practice toward weaker skills; later experience is conditioned on the learner's changing capability state. *Updated object(s):* 8.1 Training / Experience Data; 8.2 Task / Curriculum Generator; 8.3 Environment / Simulator.


1. **Absolute Zero: Reinforced Self-play Reasoning with Zero Data**  
   [[Paper](https://arxiv.org/abs/2505.03335)] · arXiv:2505.03335  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **Active Zero: Self-Evolving Vision-Language Models through Active Environment Exploration**  
   [[Paper](https://arxiv.org/abs/2602.11241)] · arXiv:2602.11241  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **Agent0: Unleashing Self-Evolving Agents from Zero Data via Tool-Integrated Reasoning**  
   [[Paper](https://arxiv.org/abs/2511.16043)] · arXiv:2511.16043  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **ANCORA: Learning to Question via Manifold-Anchored Self-Play for Verifiable Reasoning**  
   [[Paper](https://arxiv.org/abs/2604.27644)] · arXiv:2604.27644  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator; 6.4 Curriculum.

1. **ASH: Agents that Self-Hone via Embodied Learning**  
   [[Paper](https://arxiv.org/abs/2605.14211)] · arXiv:2605.14211  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 2.1 Experience Memory.

1. **BenchEvolver: Frontier Task Synthesis via Solution-Centric Evolution**  
   [[Paper](https://arxiv.org/abs/2606.01286)] · arXiv:2606.01286  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **Better LLM Reasoning via Dual-Play**  
   [[Paper](https://arxiv.org/abs/2511.11881)] · arXiv:2511.11881  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **Close the Loop: Synthesizing Infinite Tool-Use Data via Multi-Agent Role-Playing**  
   [[Paper](https://arxiv.org/abs/2512.23611)] · arXiv:2512.23611  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Concordia: Self-Improving Synthetic Tables for Federated LLMs**  
   [[Paper](https://arxiv.org/abs/2605.09855)] · arXiv:2605.09855  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **DISCOVER: Automated Curricula for Sparse-Reward Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2505.19850)] · arXiv:2505.19850  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Disentangling Intent from Role: Adversarial Self-Play for Persona-Invariant Safety Alignment**  
   [[Paper](https://arxiv.org/abs/2605.01899)] · arXiv:2605.01899  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **DUEL: Adversarial Self-Play for Multimodal Reasoning**  
   [[Paper](https://arxiv.org/abs/2605.24794)] · arXiv:2605.24794  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **EnvGen: Generating and Adapting Environments via LLMs for Training Embodied Agents**  
   [[Paper](https://arxiv.org/abs/2403.12014)] · arXiv:2403.12014  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L3. *Updated object(s):* 8.2 Task Generator; 5.1 Model Weights.

1. **EnvHarness: Awakening Static Worlds for Agent Learning**  
   [[Paper](https://arxiv.org/abs/2608.19880)] · arXiv:2608.19880  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L3. *Updated object(s):* 8.3 Environment; 4.4 Skill Library.

1. **EvoCurr: Self-evolving Curriculum with Behavior Code Generation for Complex Decision-making**  
   [[Paper](https://arxiv.org/abs/2508.09586)] · arXiv:2508.09586  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L3. *Updated object(s):* 8.2 Task Generator; 9.1 Program Code.

1. **EvoLMM: Self-Evolving Large Multimodal Models with Continuous Rewards**  
   [[Paper](https://arxiv.org/abs/2511.16672)] · arXiv:2511.16672  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **EvoVid: Temporal-Centric Self-Evolution for Video Large Language Models**  
   [[Paper](https://arxiv.org/abs/2605.21931)] · arXiv:2605.21931  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **From Context to Skills: Can Language Models Learn from Context Skillfully?**  
   [[Paper](https://arxiv.org/abs/2604.27660)] · arXiv:2604.27660  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L3. *Updated object(s):* 4.4 Skill Library; 8.2 Task Generator.

1. **G-Zero: Self-Play for Open-Ended Generation from Zero Data**  
   [[Paper](https://arxiv.org/abs/2605.09959)] · arXiv:2605.09959  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **GASP: Guided Asymmetric Self-Play For Coding LLMs**  
   [[Paper](https://arxiv.org/abs/2603.15957)] · arXiv:2603.15957  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **GenEnv: Difficulty-Aligned Co-Evolution Between LLM Agents and Environment Simulators**  
   [[Paper](https://arxiv.org/abs/2512.19682)] · arXiv:2512.19682  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **GeoX: Mastering Geospatial Reasoning Through Self-Play and Verifiable Rewards**  
   [[Paper](https://arxiv.org/abs/2605.20006)] · arXiv:2605.20006  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **iReasoner: Trajectory-Aware Intrinsic Reasoning Supervision for Self-Evolving Large Multimodal Models**  
   [[Paper](https://arxiv.org/abs/2601.05877)] · arXiv:2601.05877  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.2 Adapter; 6.1 Objective.

1. **Knowledge-Graph Paths as Intermediate Supervision for Self-Evolving Search Agents**  
   [[Paper](https://arxiv.org/abs/2605.05702)] · arXiv:2605.05702  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Language Models Need Sleep: Learning to Self-Modify and Consolidate Memories**  
   [[Paper](https://arxiv.org/abs/2606.03979)] · arXiv:2606.03979  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 5.2 Adapter; 8.2 Task Generator.

1. **Learning to Adapt: Self-Improving Web Agent via Cognitive-Aware Exploration**  
   [[Paper](https://arxiv.org/abs/2605.31365)] · arXiv:2605.31365  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Learning to Build the Environment: Self-Evolving Reasoning RL via Verifiable Environment Synthesis**  
   [[Paper](https://arxiv.org/abs/2605.14392)] · arXiv:2605.14392  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **Lifelong Robot Library Learning: Bootstrapping Composable and Generalizable Skills for Embodied Control with Language Models**  
   [[Paper](https://arxiv.org/abs/2406.18746)] · arXiv:2406.18746  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L3. *Updated object(s):* 4.4 Skill Library; 2.1 Experience Memory.

1. **LLM-as-a-Tutor: Policy-Aware Prompt Adaptation for Non-Verifiable RL**  
   [[Paper](https://arxiv.org/abs/2607.04412)] · arXiv:2607.04412  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data; 7.2 Reward / Fitness.

1. **MM-Zero: Self-Evolving Multi-Model Vision Language Models From Zero Data**  
   [[Paper](https://arxiv.org/abs/2603.09206)] · arXiv:2603.09206  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **Multi-Agent Evolve: LLM Self-Improve through Co-evolution**  
   [[Paper](https://arxiv.org/abs/2510.23595)] · arXiv:2510.23595  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 7.1 Judge; 8.1 Experience Data.

1. **OMNI-EPIC: Open-endedness via Models of Human Notions of Interestingness with Environments Programmed in Code**  
   [[Paper](https://arxiv.org/abs/2405.15568)] · arXiv:2405.15568  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L3. *Updated object(s):* 8.2 Task Generator; 8.3 Environment; 5.1 Model Weights.

1. **Paired Open-Ended Trailblazer (POET): Endlessly Generating Increasingly Complex and Diverse Learning Environments and Their Solutions**  
   [[Paper](https://arxiv.org/abs/1901.01753)] · arXiv:1901.01753  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L3. *Updated object(s):* 8.2 Task Generator; 8.3 Environment.

1. **PopuLoRA: Co-Evolving LLM Populations for Reasoning Self-Play**  
   [[Paper](https://arxiv.org/abs/2605.16727)] · arXiv:2605.16727  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator; 6.5 Meta-optimization.

1. **Project Auto-World: Towards Automated Benchmarking of Neural Relational Reasoners**  
   [[Paper](https://arxiv.org/abs/2606.24965)] · arXiv:2606.24965  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **Propose, Solve, Verify: Self-Play Through Formal Verification**  
   [[Paper](https://arxiv.org/abs/2512.18160)] · arXiv:2512.18160  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **R-Diverse: Mitigating Diversity Illusion in Self-Play LLM Training**  
   [[Paper](https://arxiv.org/abs/2602.13103)] · arXiv:2602.13103  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **R-Zero: Self-Evolving Reasoning LLM from Zero Data**  
   [[Paper](https://arxiv.org/abs/2508.05004)] · arXiv:2508.05004  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **SAGE: Multi-Agent Self-Evolution for LLM Reasoning**  
   [[Paper](https://arxiv.org/abs/2603.15255)] · arXiv:2603.15255  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Scaling Self-Play with Self-Guidance**  
   [[Paper](https://arxiv.org/abs/2604.20209)] · arXiv:2604.20209  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **SEAgent: Self-Evolving Computer Use Agent with Autonomous Learning from Experience**  
   [[Paper](https://arxiv.org/abs/2508.04700)] · arXiv:2508.04700  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **Search Self-play: Pushing the Frontier of Agent Capability without Supervision**  
   [[Paper](https://arxiv.org/abs/2510.18821)] · arXiv:2510.18821  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **SEIF: Self-Evolving Reinforcement Learning for Instruction Following**  
   [[Paper](https://arxiv.org/abs/2605.07465)] · arXiv:2605.07465  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator; 7.1 Judge.

1. **Seirênes: Adversarial Self-Play with Evolving Distractions for LLM Reasoning**  
   [[Paper](https://arxiv.org/abs/2605.11636)] · arXiv:2605.11636  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights.

1. **Self-Play Only Evolves When Self-Synthetic Pipeline Ensures Learnable Information Gain**  
   [[Paper](https://arxiv.org/abs/2603.02218)] · arXiv:2603.02218  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L3. *Updated object(s):* 8.2 Task Generator; 5.1 Model Weights.

1. **Self-Questioning Language Models**  
   [[Paper](https://arxiv.org/abs/2508.03682)] · arXiv:2508.03682  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights.

1. **SEVA: Self-Evolving Verification Agent with Process Reward for Fact Attribution**  
   [[Paper](https://arxiv.org/abs/2606.29713)] · arXiv:2606.29713  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 6.4 Curriculum.

1. **SimWorld Studio: Automatic Environment Generation with Evolving Coding Agent for Embodied Agent Learning**  
   [[Paper](https://arxiv.org/abs/2605.09423)] · arXiv:2605.09423  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L3. *Updated object(s):* 8.3 Environment; 8.2 Task Generator; 4.4 Skill Library.

1. **SKILLFOUNDRY: Building Self-Evolving Agent Skill Libraries from Heterogeneous Scientific Resources**  
   [[Paper](https://arxiv.org/abs/2604.03964)] · arXiv:2604.03964  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L3. *Updated object(s):* 4.4 Skill Library.

1. **SkillHarness: Harnessing Safe Skills for Computer-Use Agents**  
   [[Paper](https://arxiv.org/abs/2606.20636)] · arXiv:2606.20636  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L3. *Updated object(s):* 4.4 Skill Library.

1. **Socratic-SWE: Self-Evolving Coding Agents via Trace-Derived Agent Skills**  
   [[Paper](https://arxiv.org/abs/2606.07412)] · arXiv:2606.07412  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 2.1 Experience Memory; 6.4 Curriculum.

1. **SPARK: Self-Play with Asymmetric Reward from Knowledge Graphs**  
   [[Paper](https://arxiv.org/abs/2605.05546)] · arXiv:2605.05546  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **STELLA: Self-Evolving LLM Agent for Biomedical Research**  
   [[Paper](https://arxiv.org/abs/2507.02004)] · arXiv:2507.02004  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L3. *Updated object(s):* 4.1 Tool Set; 4.4 Skill Library.

1. **Survive or Collapse: The Asymmetric Roles of Data Gating and Reward Grounding in Self-Play RL**  
   [[Paper](https://arxiv.org/abs/2605.22217)] · arXiv:2605.22217  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights.

1. **Tool-R0: Self-Evolving LLM Agents for Tool-Learning from Zero Data**  
   [[Paper](https://arxiv.org/abs/2602.21320)] · arXiv:2602.21320  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_&_Environment-ca8a04)  
   *Taxonomy:* L3. *Updated object(s):* 8.2 Task Generator; 5.1 Model Weights.

1. **Towards Healthy Evolution: Exploring the Role and Mechanisms of Human-Agent Interaction in Self-Evolving Systems**  
   [[Paper](https://arxiv.org/abs/2606.06114)] · arXiv:2606.06114  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator; 1.1 Instruction.

1. **Towards Understanding Self-play for LLM Reasoning**  
   [[Paper](https://arxiv.org/abs/2510.27072)] · arXiv:2510.27072  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 7.2 Reward / Fitness.

1. **TREX: Automating LLM Fine-tuning via Agent-Driven Tree-based Exploration**  
   [[Paper](https://arxiv.org/abs/2604.14116)] · arXiv:2604.14116  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **TTCS: Test-Time Curriculum Synthesis for Self-Evolving**  
   [[Paper](https://arxiv.org/abs/2601.22628)] · arXiv:2601.22628  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 6.1 Objective.

1. **TTSR: Test-Time Self-Evolving via Reflection**  
   [[Paper](https://arxiv.org/abs/2603.03297)] · arXiv:2603.03297  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator; 2.1 Experience Memory.

1. **Verifier-Backed Hard Problem Generation for Mathematical Reasoning**  
   [[Paper](https://arxiv.org/abs/2605.06660)] · arXiv:2605.06660  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.1 Experience Data.

1. **Vocabulary Dropout for Curriculum Diversity in LLM Co-Evolution**  
   [[Paper](https://arxiv.org/abs/2604.03472)] · arXiv:2604.03472  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

1. **Voyager: An Open-Ended Embodied Agent with Large Language Models**  
   [[Paper](https://arxiv.org/abs/2305.16291)] · arXiv:2305.16291  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L3. *Updated object(s):* 4.4 Skill Library; 8.2 Task Generator.

1. **WIST: Web-Grounded Iterative Self-Play Tree for Domain-Targeted Reasoning Improvement**  
   [[Paper](https://arxiv.org/abs/2603.22352)] · arXiv:2603.22352  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L3. *Updated object(s):* 5.1 Model Weights; 8.2 Task Generator.

</details>

<a id="4-l4---autonomy-in-deployment-and-environmental-adaptation"></a>

## 4. L4 - Autonomy in Deployment and Environmental Adaptation <sub><a href="#readme-top">↑ top</a></sub>

Reusable memory, skills, or deployed agent components persistently alter later behavior within a fixed improvement process. **45 papers.**

### Featured representative papers

| Paper | Representative mechanism |
| --- | --- |
| [OS-Copilot](https://arxiv.org/abs/2402.07456) | Accumulates skills from prior computer tasks to improve a generalist OS agent. |
| [Trace2Skill](https://arxiv.org/abs/2603.25158) | Distills trajectory-local lessons into transferable agent skills. |
| [APEX](https://arxiv.org/abs/2605.21240) | Uses autonomous policy exploration to improve deployed agent behavior. |
| [Metis](https://arxiv.org/abs/2606.24151) | Bridges textual and code memory for self-evolving agents. |
| [PRACTICE](https://arxiv.org/abs/2608.30760) | Converts interaction experience into expertise for embodied agents. |
| [ENPIRE](https://arxiv.org/abs/2606.19980) | Applies agentic self-improvement to robot policies in real-world deployment. |

<details>
<summary><strong>Browse the full L4 catalog (45 papers)</strong></summary>

### Table-derived extensions

The following additions are explicitly discussed in Table 6 under trajectory distillation, iterative agent-system revision, or selective retention and deployment of updates.

1. **DecoEvo: Score-Decoupled Co-Evolution of Solver and Rubric-Generator Skills in Text Space**  
   [[Paper](https://arxiv.org/abs/2607.25675)] · arXiv:2607.25675  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_Feedback-a21caf)  
   *Survey-table rationale:* Solver and rubric skills co-evolve across iterative rounds with score-independent audits. *Updated object(s):* 7.1 Evaluator / Judge; 4.4 Skill / Macro Library.

1. **Trace2Skill: Distill Trajectory-Local Lessons into Transferable Agent Skills**  
   [[Paper](https://arxiv.org/abs/2603.25158)] · arXiv:2603.25158  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_Skills-2563eb)  
   *Survey-table rationale:* Error and success analysts merge patches into portable skill documents for later reuse. *Updated object(s):* 4.4 Skill / Macro Library.

1. **Metis: Bridging Text and Code Memory for Self-Evolving Agents**  
   [[Paper](https://arxiv.org/abs/2606.24151)] · arXiv:2606.24151  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_Knowledge-059669)  
   *Survey-table rationale:* Text plans and code tools are retained after completed tasks and validated through reuse and sandbox compilation. *Updated object(s):* 2.3 Procedural Memory; 4.3 Tool Implementation.

1. **Library Drift: Diagnosing and Fixing a Silent Failure Mode in Self-Evolving LLM Skill Libraries**  
   [[Paper](https://arxiv.org/abs/2605.19576)] · arXiv:2605.19576  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_Skills-2563eb)  
   *Survey-table rationale:* Periodic retention retires low-contribution skills and caps the evolving library. *Updated object(s):* 4.4 Skill / Macro Library.

1. **APEX: Autonomous Policy Exploration for Self-Evolving LLM Agents**  
   [[Paper](https://arxiv.org/abs/2605.21240)] · arXiv:2605.21240  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_Knowledge-059669)  
   *Survey-table rationale:* A milestone dependency graph retains episode outcomes and informs later exploration. *Updated object(s):* 2.2 Semantic / Knowledge Memory.

1. **Learning Personalized Agents from Human Feedback**  
   [[Paper](https://arxiv.org/abs/2602.16173)] · arXiv:2602.16173  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_Knowledge-059669)  
   *Survey-table rationale:* User clarification confirms and revises persistent preference entries. *Updated object(s):* 2.2 Semantic / Knowledge Memory.

1. **MemToolAgent: Leveraging Memory for Tool-Using Agents Based on Environment and User Feedback**  
   [[Paper](https://arxiv.org/abs/2606.07909)] · arXiv:2606.07909  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_Knowledge-059669)  
   *Survey-table rationale:* Tool-use critiques and retrieval policy are updated from environment and user feedback. *Updated object(s):* 2.3 Procedural Memory; 2.5 Memory Operations.

1. **PRACTICE: From Experience to Expertise in Self-Evolving Embodied Agents**  
   [[Paper](https://arxiv.org/abs/2608.30760)] · arXiv:2608.30760  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_Skills-2563eb)  
   *Survey-table rationale:* Success/failure contrasts and teacher distillation validate additions to an embodied skill library. *Updated object(s):* 4.4 Skill / Macro Library.

1. **PILOT in the Loop: Live Self-Improvement for Long-Horizon Agents**  
   [[Paper](https://arxiv.org/abs/2608.26530)] · arXiv:2608.26530  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_Knowledge-059669)  
   *Survey-table rationale:* Live-run feedback is distilled into persistent procedures and failure modes. *Updated object(s):* 2.3 Procedural Memory.

1. **Evo-Harness: Context-to-Harness Skill Compilation for Self-Evolving Agents**  
   [[Paper](https://arxiv.org/abs/2608.15071)] · arXiv:2608.15071  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness_Workflow-0f766e)  
   *Survey-table rationale:* Failed or negatively evaluated tasks trigger reflection and edits to retained harness skill tuples. *Updated object(s):* 3.6 Harness Implementation / Scaffold Code; 4.4 Skill / Macro Library.

1. **Self-Evolving Embodied Agents via Skill-Harness Evolution**  
   [[Paper](https://arxiv.org/abs/2608.11350)] · arXiv:2608.11350  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness_Workflow-0f766e)  
   *Survey-table rationale:* Planning guidance and context-selection code are retained and tested through sandbox execution and downstream tasks. *Updated object(s):* 3.1 Workflow / Graph; 1.5 Context Composition.

1. **Evo-Memory: Benchmarking LLM Agent Test-Time Learning with Self-Evolving Memory**  
   [[Paper](https://arxiv.org/abs/2511.20857)] · arXiv:2511.20857  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_Knowledge-059669)  
   *Survey-table rationale:* Accumulated agent memory is evaluated over sequential task streams for long-horizon reuse. *Updated object(s):* 2.1 Episodic / Experience Memory.

1. **S3Gym: Can LLMs Turn Self-Testing and Self-Judging into Self-Improvement?**  
   [[Paper](https://arxiv.org/abs/2608.31100)] · arXiv:2608.31100  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness_Workflow-0f766e)  
   *Survey-table rationale:* The work compares retained history, summaries, and parameter-update pathways across iterative rounds. *Updated object(s):* 3.4 Verification / Reflection Loop; 2.1 Episodic / Experience Memory.

1. **Harness Updating Is Not Harness Benefit: Disentangling Evolution Capabilities in Self-Evolving LLM Agents**  
   [[Paper](https://arxiv.org/abs/2605.30621)] · arXiv:2605.30621  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness_Workflow-0f766e)  
   *Survey-table rationale:* It separates the quality of retained harness updates from their execution benefit in fixed solve-evolve rounds. *Updated object(s):* 3.6 Harness Implementation / Scaffold Code.

1. **Rethinking Self-Evolving Agent Skills: Feedback Dynamics over Multiple Rounds**  
   [[Paper](https://arxiv.org/abs/2608.02636)] · arXiv:2608.02636  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_Skills-2563eb)  
   *Survey-table rationale:* Skill edits are filtered using task outcomes across multiple rounds. *Updated object(s):* 4.4 Skill / Macro Library.

1. **ASPIRE: Can Models Self-Evolve from Vague Goals?**  
   [[Paper](https://arxiv.org/abs/2608.31111)] · arXiv:2608.31111  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness_Workflow-0f766e)  
   *Survey-table rationale:* Verified score improvements determine whether model-weight or harness revisions are retained. *Updated object(s):* 5.1 Model Weights; 3.6 Harness Implementation / Scaffold Code.

1. **Hypothesis-Driven Skill Optimization for LLM Agents**  
   [[Paper](https://arxiv.org/abs/2606.22330)] · arXiv:2606.22330  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_Skills-2563eb)  
   *Survey-table rationale:* Candidate skill packages are retained after paired control-and-treatment executions. *Updated object(s):* 4.4 Skill / Macro Library.


1. **A Self-Evolving AI Agent System for Climate Science**  
   [[Paper](https://arxiv.org/abs/2507.17311)] · arXiv:2507.17311  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L4. *Updated object(s):* 4.4 Skill Library; 2.2 Knowledge Memory.

1. **Adaptive Orchestration: Scalable Self-Evolving Multi-Agent Systems**  
   [[Paper](https://arxiv.org/abs/2601.09742)] · arXiv:2601.09742  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L4. *Updated object(s):* 3.5 Multi-agent; 2.5 Memory & Knowledge.

1. **Agentic Self-Evolutionary Replanning for Embodied Navigation**  
   [[Paper](https://arxiv.org/abs/2603.02772)] · arXiv:2603.02772  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.1 Experience Memory; 5.4 Model.

1. **AgenticDB: Self-Evolving Reconfiguration Framework for Database Workloads**  
   [[Paper](https://arxiv.org/abs/2606.20318)] · arXiv:2606.20318  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.1 Experience Memory; 8.3 Environment.

1. **AgentTrust: A Self-Improving Trust Layer for AI-Agent Actions**  
   [[Paper](https://arxiv.org/abs/2606.08539)] · arXiv:2606.08539  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L4. *Updated object(s):* 3.6 Scaffold Code; 2.1 Experience Memory.

1. **AgentX: Towards Agent-Driven Self-Iteration of Industrial Recommender Systems**  
   [[Paper](https://arxiv.org/abs/2606.26859)] · arXiv:2606.26859  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.2 Knowledge Memory; 1.1 Instruction; 9.1 Program Code.

1. **An Agentic Framework for Autonomous Materials Computation**  
   [[Paper](https://arxiv.org/abs/2512.19458)] · arXiv:2512.19458  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L4. *Updated object(s):* 4.4 Skill Library.

1. **ArtiCAD: Articulated CAD Assembly Design via Multi-Agent Code Generation**  
   [[Paper](https://arxiv.org/abs/2604.10992)] · arXiv:2604.10992  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.2 Knowledge Memory.

1. **Audited Skill-Graph Self-Improvement for Agentic LLMs via Verifiable Rewards, Experience Synthesis, and Continual Memory**  
   [[Paper](https://arxiv.org/abs/2512.23760)] · arXiv:2512.23760  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L4. *Updated object(s):* 4.4 Skill Library; 2.1 Experience Memory.

1. **Autopoiesis: A Self-Evolving System Paradigm for LLM Serving Under Runtime Dynamics**  
   [[Paper](https://arxiv.org/abs/2604.07144)] · arXiv:2604.07144  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L4. *Updated object(s):* 3.6 Scaffold Code.

1. **BloClaw: An Omniscient, Multi-Modal Agentic Workspace for Next-Generation Scientific Discovery**  
   [[Paper](https://arxiv.org/abs/2604.00550)] · arXiv:2604.00550  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L4. *Updated object(s):* 4.1 Tool Set; 4.4 Skill Library.

1. **CASCADE: Cumulative Agentic Skill Creation through Autonomous Development and Evolution**  
   [[Paper](https://arxiv.org/abs/2512.23880)] · arXiv:2512.23880  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.1 Experience Memory; 2.3 Procedural Memory; 2.4 Memory & Knowledge.

1. **Deep Researcher Agent: An Autonomous Framework for 24/7 Deep Learning Experimentation with Zero-Cost Monitoring**  
   [[Paper](https://arxiv.org/abs/2604.05854)] · arXiv:2604.05854  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.1 Experience Memory; 9.1 Program Code.

1. **Enabling Self-Improving Agents to Learn at Test Time With Human-In-The-Loop Guidance**  
   [[Paper](https://arxiv.org/abs/2507.17131)] · arXiv:2507.17131  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.2 Knowledge Memory; 2.1 Experience Memory.

1. **ENPIRE: Agentic Robot Policy Self-Improvement in the Real World**  
   [[Paper](https://arxiv.org/abs/2606.19980)] · arXiv:2606.19980  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L4. *Updated object(s):* 5.1 Model Weights; 9.2 Algorithm.

1. **EvoMaster: A Foundational Evolving Agent Framework for Agentic Science at Scale**  
   [[Paper](https://arxiv.org/abs/2604.17406)] · arXiv:2604.17406  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.2 Knowledge Memory; 4.4 Skill Library.

1. **EXG: Self-Evolving Agents with Experience Graphs**  
   [[Paper](https://arxiv.org/abs/2605.17721)] · arXiv:2605.17721  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.1 Experience Memory; 2.4 Memory & Knowledge.

1. **GRAFT-ATHENA: Self-Improving Agentic Teams for Autonomous Discovery and Evolutionary Numerical Algorithms**  
   [[Paper](https://arxiv.org/abs/2605.11117)] · arXiv:2605.11117  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.2 Knowledge Memory; 2.1 Experience Memory.

1. **GrowLoop: Self-Evolving Conversation Evaluation Seeded by Human**  
   [[Paper](https://arxiv.org/abs/2605.28882)] · arXiv:2605.28882  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L4. *Updated object(s):* 7.1 Judge; 8.1 Experience Data; 8.2 Task Generator.

1. **HiLSVA: Design and Evaluation of a Human-in-the-Loop Agentic System for Scientific Visualization**  
   [[Paper](https://arxiv.org/abs/2606.26614)] · arXiv:2606.26614  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.1 Experience Memory; 2.2 Knowledge Memory.

1. **Learning from Trials and Errors: Reflective Test-Time Planning for Embodied LLMs**  
   [[Paper](https://arxiv.org/abs/2602.21198)] · arXiv:2602.21198  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L4. *Updated object(s):* 5.1 Model Weights; 7.1 Judge.

1. **OS-Copilot: Towards Generalist Computer Agents with Self-Improvement**  
   [[Paper](https://arxiv.org/abs/2402.07456)] · arXiv:2402.07456  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L4. *Updated object(s):* 4.4 Skill Library; 2.2 Knowledge Memory.

1. **Safe and Adaptive Cloud Healing: Verifying LLM-Generated Recovery Plans with a Neural-Symbolic World Model**  
   [[Paper](https://arxiv.org/abs/2607.01595)] · arXiv:2607.01595  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L4. *Updated object(s):* 5.2 Adapter.

1. **SkillAxe: Sharpening LLM-Authored Agent Skills Through Evaluation-Guided Self-Refinement**  
   [[Paper](https://arxiv.org/abs/2606.10546)] · arXiv:2606.10546  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L4. *Updated object(s):* 4.4 Skill Library.

1. **The Station: An Open-World Environment for AI-Driven Discovery**  
   [[Paper](https://arxiv.org/abs/2511.06309)] · arXiv:2511.06309  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L4. *Updated object(s):* 9.1 Program Code; 9.3 External Artifact; 2.1 Experience Memory.

1. **Towards Continuous Intelligence Growth: Self-Training, Continual Learning, and Dual-Scale Memory in SuperIntelliAgent**  
   [[Paper](https://arxiv.org/abs/2511.23436)] · arXiv:2511.23436  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L4. *Updated object(s):* 5.1 Model Weights; 2.1 Experience Memory.

1. **Useful Memories Become Faulty When Continuously Updated by LLMs**  
   [[Paper](https://arxiv.org/abs/2605.12978)] · arXiv:2605.12978  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Memory_&_Knowledge-059669)  
   *Taxonomy:* L4. *Updated object(s):* 2.1 Experience Memory; 2.2 Knowledge Memory.

1. **VizGenie: Toward Self-Refining, Domain-Aware Workflows for Next-Generation Scientific Visualization**  
   [[Paper](https://arxiv.org/abs/2507.21124)] · arXiv:2507.21124  
   ![](https://img.shields.io/badge/-Level--L4-059669) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L4. *Updated object(s):* 4.4 Skill Library; 2.2 Knowledge Memory.

</details>

<a id="5-l5---from-environmental-adaptation-to-meta-improvement"></a>

## 5. L5 - From Environmental Adaptation to Meta-Improvement <sub><a href="#readme-top">↑ top</a></sub>

The system improves the mechanism that produces future improvements, including search, evaluation, and research-control policies. **32 papers.**

<div align="center">
  <img src="./assets/rsi-l4-l5-meta-improvement.png" width="100%" alt="Comparison of L4 environmental adaptation and L5 recursive meta-improvement. L5 revises and validates the improvement process inherited by successor systems under external human mission, safety, evaluation, and acceptance constraints.">
  <br>
  <em><b>Figure 3.</b> From L4 adaptation to L5 recursive meta-improvement. L5 concerns accepted revisions to the process that produces future improvements, not merely adaptation within a fixed process.</em>
</div>

### Featured representative papers

| Paper | Representative mechanism |
| --- | --- |
| [Self-Taught Optimizer](https://arxiv.org/abs/2310.02304) | Recursively improves the code-generation procedure that drives later search rounds. |
| [Gödel Agent](https://arxiv.org/abs/2410.04444) | Provides a self-referential agent framework that can revise its own improvement routines. |
| [Darwin Gödel Machine](https://arxiv.org/abs/2505.22954) | Evolves coding agents through evaluated code modifications and inherited successful descendants. |
| [Dream-RSI](https://arxiv.org/abs/2609.14858) | Replays past discovery trees to select revised exploration policies for later online search. |
| [AIRA2](https://arxiv.org/abs/2603.26499) | Targets AI-research-agent bottlenecks through asynchronous experimentation, hidden-consistent evaluation, and interactive ReAct operators. |
| [MOSS](https://arxiv.org/abs/2605.22794) | Evolves autonomous agents by rewriting source-level system components. |
| [The Red Queen Gödel Machine](https://arxiv.org/abs/2606.26294) | Co-evolves agents and evaluators, making the improvement criterion part of the meta-level loop. |

<details>
<summary><strong>Browse the full L5 catalog (32 papers)</strong></summary>

### Table-derived extensions

The following additions are explicitly listed in Table 7 as L5 mechanisms with identified external controls.

1. **Self-Taught Optimizer (STOP): Recursively Self-Improving Code Generation**  
   [[Paper](https://arxiv.org/abs/2310.02304)] · arXiv:2310.02304  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Full_system_Co-evolution-be123c)  
   *Survey-table rationale:* The current improver receives its own source as an optimization target; selected improver code governs the next program-search round. *Updated object(s):* 10.3 Improvement-loop / Meta-RSI; 9.1 Program / Solution Code.

1. **AIRA2: Overcoming Bottlenecks in AI Research Agents**  
   [[Paper](https://arxiv.org/abs/2603.26499)] · arXiv:2603.26499  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Full_system_Co-evolution-be123c)  
   *Survey-table rationale:* Research artifacts and a search policy are retained to guide later task experiments under an external research harness and evaluation. *Updated object(s):* 10.3 Improvement-loop / Meta-RSI; 6.5 Search / Meta-optimization Procedure.


1. **A-Evolve-Training: Autonomous Post-Training of a 30B Model**  
   [[Paper](https://arxiv.org/abs/2606.20657)] · arXiv:2606.20657  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Trainer___Optimization-c2410c)  
   *Taxonomy:* L5. *Updated object(s):* 6.5 Meta-optimization; 5.1 Model Weights.

1. **Accelerating Scientific Discovery with Autonomous Goal-evolving Agents**  
   [[Paper](https://arxiv.org/abs/2512.21782)] · arXiv:2512.21782  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L5. *Updated object(s):* 7.2 Reward / Fitness; 9.3 External Artifact.

1. **AlgoEvolve: LLM-driven Meta-evolution of Algorithmic Trading Programs**  
   [[Paper](https://arxiv.org/abs/2606.26173)] · arXiv:2606.26173  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Prompt_&_Context-7c3aed)  
   *Taxonomy:* L5. *Updated object(s):* 1.1 Instruction; 6.5 Meta-optimization; 9.1 Program Code.

1. **ARYA: A Physics-Constrained Composable & Deterministic World Model Architecture**  
   [[Paper](https://arxiv.org/abs/2603.21340)] · arXiv:2603.21340  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Full--system___Co--evolution-be123c)  
   *Taxonomy:* L5. *Updated object(s):* 10.3 Meta-RSI; 6.5 Meta-optimization; 5.1 Model Weights.

1. **Autonomous Code Evolution Meets NP-Completeness**  
   [[Paper](https://arxiv.org/abs/2509.07367)] · arXiv:2509.07367  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L5. *Updated object(s):* 9.1 Program Code; 3.6 Scaffold Code; 10.3 Meta-RSI.

1. **Can Large Language Models Invent Algorithms to Improve Themselves?: Algorithm Discovery for Recursive Self-Improvement through Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2410.15639)] · arXiv:2410.15639  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L5. *Updated object(s):* 5.1 Model Weights; 10.3 Meta-RSI.

1. **Code-A1: Adversarial Evolving of Code LLM and Test LLM via Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2603.15611)] · arXiv:2603.15611  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L5. *Updated object(s):* 5.1 Model Weights; 7.3 Verifier; 2.1 Experience Memory.

1. **Darwin Gödel Machine: Open-Ended Evolution of Self-Improving Agents**  
   [[Paper](https://arxiv.org/abs/2505.22954)] · arXiv:2505.22954  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L5. *Updated object(s):* 3.6 Scaffold Code; 4.3 Tool Code.

1. **Differentiable Evolutionary Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2512.13399)] · arXiv:2512.13399  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L5. *Updated object(s):* 5.1 Model Weights; 7.2 Reward / Fitness.

1. **Emotion-Gradient Metacognitive RSI (Part I): Theoretical Foundations and Single-Agent Architecture**  
   [[Paper](https://arxiv.org/abs/2505.07757)] · arXiv:2505.07757  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Full--system___Co--evolution-be123c)  
   *Taxonomy:* L5. *Updated object(s):* 10.3 Meta-RSI.

1. **Escher-Loop: Mutual Evolution by Closed-Loop Self-Referential Optimization**  
   [[Paper](https://arxiv.org/abs/2604.23472)] · arXiv:2604.23472  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Full--system___Co--evolution-be123c)  
   *Taxonomy:* L5. *Updated object(s):* 10.3 Meta-RSI; 9.1 Program Code.

1. **EvoRubric: Self-Evolving Rubric-Driven RL for Open-Ended Generation**  
   [[Paper](https://arxiv.org/abs/2605.29847)] · arXiv:2605.29847  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L5. *Updated object(s):* 5.1 Model Weights; 7.2 Reward / Fitness.

1. **EvoRubrics: Dynamic Rubrics as Rewards via Adversarial Co-Evolution for LLM Reinforcement Learning**  
   [[Paper](https://arxiv.org/abs/2606.23038)] · arXiv:2606.23038  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L5. *Updated object(s):* 5.1 Model Weights; 7.1 Judge.

1. **EvoX: Meta-Evolution for Automated Discovery**  
   [[Paper](https://arxiv.org/abs/2602.23413)] · arXiv:2602.23413  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Full--system___Co--evolution-be123c)  
   *Taxonomy:* L5. *Updated object(s):* 10.3 Meta-RSI; 3.6 Scaffold Code.

1. **GEAR: Genetic AutoResearch for Agentic Code Evolution**  
   [[Paper](https://arxiv.org/abs/2605.13874)] · arXiv:2605.13874  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L5. *Updated object(s):* 9.1 Program Code; 6.5 Meta-optimization.

1. **Gödel Agent: A Self-Referential Agent Framework for Recursive Self-Improvement**  
   [[Paper](https://arxiv.org/abs/2410.04444)] · arXiv:2410.04444  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Full--system___Co--evolution-be123c)  
   *Taxonomy:* L5. *Updated object(s):* 10.3 Meta-RSI; 3.6 Scaffold Code.

1. **Group-Evolving Agents: Open-Ended Self-Improvement via Experience Sharing**  
   [[Paper](https://arxiv.org/abs/2602.04837)] · arXiv:2602.04837  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L5. *Updated object(s):* 3.6 Scaffold Code; 4.3 Tool Code.

1. **Huxley-Gödel Machine: Human-Level Coding Agent Development by an Approximation of the Optimal Self-Improving Machine**  
   [[Paper](https://arxiv.org/abs/2510.21614)] · arXiv:2510.21614  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L5. *Updated object(s):* 3.6 Scaffold Code; 10.3 Meta-RSI.

1. **Hyperagents**  
   [[Paper](https://arxiv.org/abs/2603.19461)] · arXiv:2603.19461  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Full--system___Co--evolution-be123c)  
   *Taxonomy:* L5. *Updated object(s):* 10.3 Meta-RSI; 3.6 Scaffold Code.

1. **MetaSkill-Evolve: Recursive Self-Improvement of LLM Agents via Two-Timescale Meta-Skill Evolution**  
   [[Paper](https://arxiv.org/abs/2607.05297)] · arXiv:2607.05297  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Tools_&_Skills-2563eb)  
   *Taxonomy:* L5. *Updated object(s):* 4.4 Skill Library; 10.3 Meta-RSI.

1. **MOSS: Self-Evolution through Source-Level Rewriting in Autonomous Agent Systems**  
   [[Paper](https://arxiv.org/abs/2605.22794)] · arXiv:2605.22794  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L5. *Updated object(s):* 3.6 Scaffold Code.

1. **Ouroboros: A Self-Developing Frontier Coding Agent with Reviewed Core Evolution**  
   [[Paper](https://arxiv.org/abs/2608.08311)] · arXiv:2608.08311  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Harness___Workflow-0f766e)  
   *Taxonomy:* L5. *Updated object(s):* 3.6 Scaffold Code; 4.1 Tool Set; 1.5 Context.

1. **Scientific discovery as meta-optimization: a combinatorial optimization case study**  
   [[Paper](https://arxiv.org/abs/2606.26728)] · arXiv:2606.26728  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L5. *Updated object(s):* 7.2 Reward / Fitness; 9.2 Algorithm.

1. **Self-Evolving Scientific Agent Designs Physically-Reasoned Whitebox Fluid Control**  
   [[Paper](https://arxiv.org/abs/2606.08405)] · arXiv:2606.08405  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--External_Artifact-4f46e5)  
   *Taxonomy:* L5. *Updated object(s):* 9.2 Algorithm; 10.3 Meta-RSI.

1. **SOLAR: A Self-Optimizing Open-Ended Autonomous Agent for Lifelong Learning and Continual Adaptation**  
   [[Paper](https://arxiv.org/abs/2605.20189)] · arXiv:2605.20189  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Model-1d4ed8)  
   *Taxonomy:* L5. *Updated object(s):* 5.1 Model Weights; 2.1 Experience Memory; 5.2 Adapter.

1. **The Red Queen Gödel Machine: Co-Evolving Agents and Their Evaluators**  
   [[Paper](https://arxiv.org/abs/2606.26294)] · arXiv:2606.26294  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L5. *Updated object(s):* 7.1 Judge; 7.2 Reward / Fitness; 10.3 Meta-RSI.

1. **Towards Agentic Self-Learning LLMs in Search Environment**  
   [[Paper](https://arxiv.org/abs/2510.14253)] · arXiv:2510.14253  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L5. *Updated object(s):* 7.2 Reward / Fitness; 8.2 Task Generator; 5.1 Model Weights.

1. **When Your Own Output Becomes Your Training Data: Noise-to-Meaning Loops and a Formal RSI Trigger**  
   [[Paper](https://arxiv.org/abs/2505.02888)] · arXiv:2505.02888  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Full--system___Co--evolution-be123c)  
   *Taxonomy:* L5. *Updated object(s):* 10.3 Meta-RSI.

1. **Who Grades the Grader? Co-Evolving Evaluation Metrics and Skills for Self-Improving LLM Agents**  
   [[Paper](https://arxiv.org/abs/2607.12790)] · arXiv:2607.12790  
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Evaluator_&_Feedback-a21caf)  
   *Taxonomy:* L5. *Updated object(s):* 7.1 Judge; 4.4 Skill Library.

### Independently screened addition (2026-09-24)

1. **Dream-RSI: Recursive Self-Improvement through Evolving Worlds**<br>
   [[Paper](https://arxiv.org/abs/2609.14858)] · [[Project](https://www.dream-rsi.com/)] · arXiv:2609.14858<br>
   ![](https://img.shields.io/badge/-Level--L5-be123c) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Trainer_Optimization-c2410c)<br>
   *Editorial rationale:* A policy-development agent revises exploration-policy code using feedback from replayed discovery trees; the selected policy guides the next online search and generates new history for later rounds. The coding agent, model weights, evaluator, and task objective remain fixed. *Updated object(s):* 6.5 Search / Meta-optimization Procedure; 2.1 Experience Memory.

</details>

<a id="contributing"></a>

## Contributing <sub><a href="#readme-top">↑ top</a></sub>

To add or revise an entry, keep its evidence auditable. Provide a stable identifier and state the loop as **current state -> proposal/acquisition -> feedback/admission -> persistent update -> later-round effect**. If a paper changes several objects, retain all target codes but place it under the highest-level mechanism actually demonstrated.

```markdown
1. **Paper Title**  
   [[Paper](https://arxiv.org/abs/YYMM.NNNNN)] · arXiv:YYMM.NNNNN  
   ![](https://img.shields.io/badge/-Level--L3-d97706) ![](https://img.shields.io/badge/-In_scope--RSI-16a34a) ![](https://img.shields.io/badge/-Target--Data_Environment-ca8a04)  
    *Taxonomy:* L3. *Updated object(s):* 8.1 Experience Data.
```

<a id="citation"></a>

## Citation <sub><a href="#readme-top">↑ top</a></sub>

If you find this repository or its taxonomy useful, please cite the companion survey:

```bibtex
@misc{duan2026aibuilthumansgenuine,
  title={The Last AI Built by Humans: Toward Genuine Recursive Self-Improvement},
  author={Yi Duan and Ying Liu and Zirui Tang and Haodong Chen and Jun Zhou and Yumou Liu and Bangrui Xu and Yukai Wu and Sidi Chen and Yuhan Zhou and Haoyu Wang and Xiaoyou Yu and Shaokun Han and Xuzhou Zhu and Le Zhou and Bolin Lu and Wei Zhou and Jiachen Liu and Nuozhou Fang and Jiaxin Tian and Ruoyu Chen and Yuxuan Li and Kai Zuo and Kaiyan Zhang and Jiantao Qiu and Conghui He and Guoliang Li and Bowen Zhou and Zhiyuan Liu and Zhoufutu Wen and Jihua Kang and Xuanhe Zhou and Fan Wu},
  year={2026},
  eprint={2609.11873},
  archivePrefix={arXiv},
  primaryClass={cs.LG},
  url={https://arxiv.org/abs/2609.11873}
}
```

<a id="data-provenance-and-validation"></a>

## Data Provenance and Validation <sub><a href="#readme-top">↑ top</a></sub>

This document combines a 491-paper per-paper taxonomy dataset with 28 additional works selected from the survey's representative Tables 3-7 on 2026-09-11, plus two independently screened papers added on 2026-09-24. The baseline dataset records a title, arXiv ID, primary level, boundary classification, detailed rationale, and updated-object code(s) for every paper. The 28 extensions retain the table-derived rationale; the later additions record their editorial rationales separately. Authors and venue metadata are not inferred for catalog entries.

Catalog integrity checks:

- **491 / 491** baseline rows have a title, arXiv ID, and valid primary level `L1` to `L5`; each of the **28** extensions has a stable arXiv identifier.
- The independently screened [GPTSwarm paper](https://arxiv.org/abs/2402.16823) has a stable arXiv identifier and is classified as L2 because it retains feedback-driven changes to agent prompts and graph connectivity under an externally specified task utility.
- The independently screened [Dream-RSI paper](https://arxiv.org/abs/2609.14858) has a stable arXiv identifier and is classified as L5 because it updates the exploration policy used to generate later improvements while keeping the coding agent and evaluator fixed.
- **0** duplicate arXiv IDs and **0** duplicate titles were found across the 521 entries.
- All IDs match the arXiv identifier pattern `YYMM.NNNNN` (or its four-digit predecessor form).
- Baseline source labels are preserved rather than inferred from keyword matching. Keyword-only screening would incorrectly omit lower-level but in-scope work such as automatic prompt search.

The per-paper taxonomy dataset remains the authoritative record for the 491-paper baseline. The 28 extensions came from the survey's chapter tables; GPTSwarm and Dream-RSI were reviewed against the same inclusion and classification criteria using their primary papers. Aggregate visualizations should not be used to reconstruct individual paper metadata.
