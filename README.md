# How Far Are Synthetic Text-to-SQL Benchmarks from Enterprise Production Traffic?

Victor Arantes, Thiago Pedroso de Jesus, Vinicius Alboneti Aguiar, Sávio Salvarino Teles de Oliveira

Institute of Informatics, Federal University of Goiás (UFG) · Center of Excellence in Artificial Intelligence (CEIA), Brazil

**2nd Workshop on Agentic AI Benchmarks and Applications for Enterprise Tasks (AABA4ET) @ NeurIPS 2026**

📄 **[Read the paper (PDF)](paper.pdf)**

## Abstract

Synthetic Text-to-SQL benchmark generators are evaluated intrinsically, by LLM judges and against each other, but almost never against what enterprise users actually ask. We measure that gap directly on a rare pairing: three recent synthetic benchmarks (the agentic SAGE-SQL and controlled re-implementations of OmniSQL and SQaLe) and the production traffic of a deployed Text-to-SQL agent, both targeting the same operational schema of a regulated electric energy distribution utility. From 697 production turns (683 distinct questions, 235 sessions, 61 users) we build a reference distribution and compare it to the generated corpora under size-controlled repeated random subsampling. Real traffic is more textually diverse than every generator on four of five metrics (2.1× the best distinct-1), and 62% of real questions match none of the ten rhetorical molds that describe the synthetic corpora. Real traffic also systematically violates three properties every generator enforces by construction: questions are often not self-contained (18% anaphoric), not single-query (86% of SQL queries serve multi-query turns), and not always answerable (2.6% out of schema scope). The agentic generator comes closest to production on all four diversity metrics for which production falls outside the generators' observed range (evidence for execution-grounded, schedule-controlled synthesis), yet the residual gap is structural to the task formulation all generators share, not to any one system. A preliminary human calibration (n=49) shows that judge rubrics centered on SQL correctness, well-suited to scoring generated pairs, transfer poorly to conversational production traffic, ranking human-rated response quality near chance (AUROC 0.52), whereas answer-fidelity and user-signal rubrics reach 0.81 combined. Our measurement protocol is a cheap, label-free instrument for grounding enterprise agent benchmarks in production traffic.

## Contact

- victor_arantes@discente.ufg.br
- thiagopedroso@discente.ufg.br
