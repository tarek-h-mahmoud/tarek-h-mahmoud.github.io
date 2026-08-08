---
layout: page
title: Agentic AI Investment Research and Reporting Platform
permalink: /projects/agentic-investment-research/
group: Product Development
order: 1
context: Equity and macroeconomic research for a large institutional investment organization
summary: Built production agentic workflows for equity and macroeconomic research, combining hybrid retrieval, metadata filtering, and hierarchical map-reduce synthesis over licensed research and analyst valuation models to produce template-driven reports with claim-level citations.
tech: [RAG, LangChain, LangGraph, LLM Evaluation]
---

### Problem

A large institutional investment organization needed to accelerate research across its equity and macroeconomic teams. Analysts manually synthesized licensed financial research, company fundamentals, and internal valuation models into highly structured reports. The process was slow, difficult to scale, and required every conclusion to remain traceable to its supporting evidence.

### My role

Principal data scientist and technical lead, responsible for client discovery, solution architecture, implementation, evaluation, and production delivery.

I worked directly with investment analysts to understand their research process and translate separate equity and macroeconomic reporting requirements into production agentic workflows. I developed the Python services, APIs, custom tools, LangChain components, LangGraph workflows, document-ingestion pipeline, retrieval architecture, evaluation framework, and grounding controls.

### Approach

Built separate agentic workflows for equity and macroeconomic research. The system processed licensed research reports and analyst-provided valuation models stored on client-side SharePoint.

Documents were indexed using overlapping chunks. A routing workflow interpreted each request, selected the appropriate reporting cadence, and generated structured metadata filters covering ticker, country, sector, analyst, fiscal period, research category, and access permissions.

Retrieval combined full-text and vector search to capture both exact financial terminology and semantic relevance. Custom recency rules selected the appropriate monthly, six-month, or annual research horizon and prioritized the latest applicable report from each provider.

For each request, the system translated the selected report template into a template-specific LangGraph execution plan. Specialized processing steps analyzed individual sections, called retrieval and document-processing tools, and progressively synthesized their outputs through a hierarchical map-reduce process. LangGraph orchestrated shared state, dependencies, parallel branches, and aggregation, while LangChain integrations connected the OpenAI models, retrievers, prompt templates, and tools.

The workflow generated a formatted report containing an executive summary, financial tables, visualizations, and claim-level citations.

Grounding checkpoints and LLM-as-a-judge evaluations assessed generated content for factual support, hallucinations, citation correctness, numerical accuracy, completeness, and relevance. Retrieval was evaluated using Precision@K and Recall@K, with Langfuse used for tracing and analysis. Investment analysts reviewed reports section by section and provided detailed qualitative feedback across multiple iterations.

### Outcome

Delivered a production deployment and secured a commercial contract combining software subscription and professional services within approximately six months of the initial client meeting. Reports were generated in roughly 5–10 minutes, and the client's managing director reported a 7× improvement in analyst productivity.

### Technologies

GPT-5, OpenAI `text-embedding-3-large`, Python, LangChain, LangGraph, Langfuse, retrieval-augmented generation, LLM tool calling, hybrid retrieval, metadata filtering, hierarchical map-reduce synthesis, LLM-as-a-judge, SharePoint, Kubernetes.
