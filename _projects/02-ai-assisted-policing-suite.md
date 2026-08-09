---
layout: page
title: Agentic AI Investigative Intelligence Platform
permalink: /projects/ai-assisted-policing-suite/
group: Product Development
order: 2
context: Law-enforcement investigation and decision support
summary: Built a stateful detective assistant that extracts POLE entities from case evidence into a Neo4j knowledge graph, supporting cross-case correlation, timeline reconstruction, and evidence-grounded hypothesis generation, alongside a legal RAG pipeline and human-in-the-loop approval throughout.
tech: [LangGraph, Neo4j, GraphRAG, Human-in-the-Loop]
---

### Problem

Law-enforcement agencies needed a more effective way to analyze fragmented case data, connect evidence across sources, reconstruct events, and identify investigative gaps. Any AI-generated conclusion or recommended action also needed to remain traceable to its evidence and subject to investigator approval.

### My role

Principal data scientist and technical owner of the AI architecture over a two-year period, from the original executive demonstration through multiple client-data proofs of concept.

I conceptualized the investigative capabilities and personally developed the LangGraph orchestration, LangChain tools, Python APIs, evidence-ingestion pipelines, POLE extraction, Neo4j knowledge graph, entity-resolution logic, legal retrieval system, case-triage and investigator-assignment services, and evaluation pipelines. UI development, infrastructure deployment, and post-POC delivery were handled by dedicated engineering and delivery teams.

### Approach

Built a stateful detective assistant that maintained case context across conversations and used specialized tools to analyze structured and unstructured evidence. An LLM transformed incoming evidence into a POLE representation covering persons, objects, locations, and events.

The extracted entities, relationships, timestamps, and source provenance were stored in a Neo4j knowledge graph. This supported cross-case correlation, suspect profiling, timeline and narrative reconstruction, evidence-grounded hypothesis generation, and confidence-scored analysis while preserving links to the original evidence.

A separate retrieval-augmented generation pipeline grounded legal and procedural analysis in jurisdiction-specific penal codes, criminal-procedure laws, and investigative operating procedures. The assistant cited applicable provisions, explained its reasoning, identified evidence gaps, and recommended investigative actions.

Additional services supported case-intake triage, priority recommendations, and investigator assignment based on specialization, historical experience, and current workload. These capabilities were exposed through APIs for integration into the wider case-management platform. All consequential decisions and actions required human review and approval, with audit logs and provenance retained throughout the workflow.

Major capabilities were benchmarked using curated test cases and refined through client review across multiple proofs of concept.

### Outcome

Advanced the concept from an executive-requested demonstration to multiple proofs of concept using client-provided case data. The resulting AI architecture generated sustained interest from law-enforcement organizations and established the foundation for a production platform, which was subsequently transferred to a dedicated delivery team for implementation.

### Technologies

Python, LangGraph, LangChain, OpenAI models, Neo4j, GraphRAG, retrieval-augmented generation, LLM tool calling, structured extraction, POLE data modeling, knowledge graphs, entity resolution, human-in-the-loop workflows, REST APIs, case-management system integration.
