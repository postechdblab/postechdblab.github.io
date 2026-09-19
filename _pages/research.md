---
title: "Database & Data Mining Lab - Research"
layout: textlay
excerpt: "Database & Data Mining Lab - Research"
sitemap: false
permalink: /research/
---

<style>
.demo-row { display: flex; gap: 16px; overflow-x: auto; scroll-snap-type: x mandatory; padding: 4px 0 12px 0; -webkit-overflow-scrolling: touch; }
.demo-card { flex: 0 0 480px; max-width: 90vw; scroll-snap-align: start; }
.demo-card .demo-frame { position: relative; width: 100%; padding-top: 56.25%; background: #000; border-radius: 6px; overflow: hidden; }
.demo-card .demo-frame iframe, .demo-card .demo-frame video { position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0; }
.demo-card .demo-caption { font-size: 0.9em; margin-top: 6px; color: #555; }
.demo-card .demo-caption b { color: #222; }
.area-intro { margin-bottom: 8px; }
</style>

# Research

We build the full stack from data systems to autonomous agents. Our engines make data ultrafast to query; our AI databases let people express intent in natural language; our agents ground large language models in enterprise data across text, tables, images, and graphs; and our embodied agents carry the same ideas into robots that act in the physical world.

<br>
## 1. Enterprise Super Agents & Multi-Modal RAG

<p class="area-intro">Enterprise knowledge is scattered across text, tables, images, and knowledge graphs. We build retrieval-augmented agents that reason over all of these modalities at once: multi-granular retrievers that fuse table and text evidence, late-interaction retrievers that scale to open-domain multimodal corpora, and agentic traversal strategies that learn from their own failures. We also design principled benchmarks so that progress on complex multi-hop question answering can be measured rigorously.</p>

- **TRACE**: Table–Text Relationalization and Completion of Evidence for Coverage-Sensitive QA. *EMNLP 2026*.
- **FAILURE IS FEEDBACK**: History-Aware Backtracking for Agentic Traversal in Multimodal Graphs. *ICML 2026*.
- **SPARTA**: Scalable and Principled Benchmark of Tree-Structured Multi-hop QA over Text and Tables. *ICLR 2026*.
- **LILaC**: Late Interacting in Layered Component Graph for Open-domain Multimodal Multihop Retrieval. *EMNLP 2025*.
- **TRIAL**: Token Relations and Importance Aware Late-interaction for Accurate Text Retrieval. *EMNLP 2025*.
- **SAFE**: Schema-Driven Approximate Distance Join for Efficient Knowledge Graph Querying. *EMNLP 2025*.
- **HELIOS**: Harmonizing Early Fusion, Late Fusion, and LLM Reasoning for Multi-Granular Table-Text Retrieval. *ACL 2025*.
<br>
## 2. AI Database

<p class="area-intro">We are redefining what a database engine is in the era of LLMs. <b>CADENZA</b> compiles natural-language intent into task-specific operator DAGs, turning semantic queries into optimizable plans instead of monolithic LLM calls. <b>TurboLynx</b> is the world's fastest embedded graph DBMS—a schemaless engine for general-purpose analytics over graphs and tables—and <b>Themis</b> executes relational queries on GPUs. Underneath, we keep pushing the core of query optimization: learned cardinality estimation with theoretical guarantees, cost-efficient batching of massive small-query workloads, and cache replacement for direct-access cloud OLAP.</p>

- **CADENZA**: Compiling Natural-Language Intent into Task-Specific Operator DAGs for Semantic Query Processing. *SIGMOD 2027*.
- **CADENZA in Action**: Breaking the Monolith with Intent-Dependent Plan Spaces for Semantic Queries. *VLDB 2026 Demo*.
- **Cache Replacement in Direct-Access Cloud OLAP**: An Experimental Comparison and Practical Guidance. *SIGMOD 2027*.
- **TurboLynx**: Schemaless Graph Engine Strikes Back for General-Purpose Analytics. *VLDB 2026*.
- **TurboLynx in Action**: A Schemaless Graph Engine for General-Purpose Analytics. *VLDB 2026 Demo*.
- **Batcher**: Learning to Construct Cost-Efficient Batches of Small Queries in Big Data Processing Platforms. *ICDE 2026*.
- **Themis**: A GPU-accelerated Relational Query Execution Engine. *VLDB 2025*.
- **ASM**: Harmonizing Autoregressive Model, Sampling, and Multi-dimensional Statistics Merging for Cardinality Estimation. *SIGMOD 2024*.
- **DoppelGanger++**: Towards Fast Dependency Graph Generation for Database Replay. *SIGMOD 2024*.
<div class="demo-row">
  <div class="demo-card">
    <div class="demo-frame"><iframe src="https://www.youtube-nocookie.com/embed/nGlYnVEuqNk?rel=0" allowfullscreen loading="lazy"></iframe></div>
    <div class="demo-caption"><b>CADENZA in Action</b> — semantic queries compiled into intent-dependent operator DAGs (VLDB 2026 Demo)</div>
  </div>
  <div class="demo-card">
    <div class="demo-frame"><iframe src="https://www.youtube-nocookie.com/embed/DwdaBWL3cWs?rel=0" allowfullscreen loading="lazy"></iframe></div>
    <div class="demo-caption"><b>TurboLynx in Action</b> — the world's fastest embedded graph DBMS (VLDB 2026 Demo) · <a href="https://turbolynx.io">turbolynx.io</a></div>
  </div>
</div>

<br>
## 3. Embodied AI & Robot Manipulation

<p class="area-intro">Vision-language-action (VLA) models let robots follow open-ended language instructions, but they struggle with what makes a task <i>yours</i>—"bring <i>my</i> cup." We study how to personalize and ground VLA policies with lightweight visual prompting and in-context adaptation, without retraining the underlying model, and how to connect embodied agents to the knowledge and retrieval infrastructure we build for enterprise agents.</p>

- **Bring My Cup!** Personalizing Vision-Language-Action Models with Visual Attentive Prompting. *ICML 2026*.
<div class="demo-row">
  <div class="demo-card">
    <div class="demo-frame"><video src="https://vap-project.github.io/static/videos/put_my_stuffed_toy_into_the_plastic_bowl/cam_merged.mp4" controls muted loop playsinline preload="metadata"></video></div>
    <div class="demo-caption"><b>"Put my stuffed toy into the plastic bowl"</b> — real-robot personalization with VAP</div>
  </div>
  <div class="demo-card">
    <div class="demo-frame"><video src="https://vap-project.github.io/static/videos/put_my_pouch_into_the_plastic_bowl/cam_merged.mp4" controls muted loop playsinline preload="metadata"></video></div>
    <div class="demo-caption"><b>"Put my pouch into the plastic bowl"</b> — real-robot personalization with VAP</div>
  </div>
  <div class="demo-card">
    <div class="demo-frame"><video src="https://vap-project.github.io/static/videos/put_my_cat_figurine_into_the_plastic_bowl_and_put_my_brother's_owl_figurine_into_the_plastic_bowl/cam_merged.mp4" controls muted loop playsinline preload="metadata"></video></div>
    <div class="demo-caption"><b>Multi-user, multi-object</b> — "put my cat figurine … and my brother's owl figurine into the plastic bowl"</div>
  </div>
</div>

<br>
## 4. Next-Gen LLM Inference & Reasoning Optimization

<p class="area-intro">Serving and reasoning with LLMs is, at its core, a systems problem: memory hierarchies, scheduling, and cost-aware planning. We are bringing our database-engine expertise—query optimization, caching, and workload-aware execution—to LLM inference, and extending it to multi-step reasoning so that agentic workloads run faster and cheaper without sacrificing answer quality. This is where our engines, AI databases, and agents converge, and it is the next direction of the lab.</p>

<br>
### ... and more.
See our full [publication list](/publications/).
