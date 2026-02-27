# TemporalESG: A Trilingual Benchmark for Time-Critical ESG Information Retrieval

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

This repository contains the **TemporalESG benchmark**, introduced in the paper:

> *“Bridging the Temporal-Semantic Gap: A Trilingual Benchmark and Hybrid Retrieval Framework for Time-Critical ESG Information Access”*  
> (Authors, Journal, Year)

The benchmark is designed to evaluate information retrieval systems on **temporal‑aware, entity‑centric** queries in the Environmental, Social, and Governance (ESG) domain. It comprises **40,814 multilingual document chunks** (Vietnamese, English, Arabic) from 43 multinational corporations over 11 years (2015–2025), along with **970 validated temporal queries**.

---

## 📦 Dataset Contents

| File | Description |
|------|-------------|
| `documents/` | Folder containing the document chunks in JSONL format (one file per language). Each line is a JSON object with the following fields: `doc_id`, `text`, `year`, `company`, `lang`. |
| `queries.jsonl` | 970 queries in JSONL format. Each line includes: `query_id`, `text`, `target_year`, `target_company`, `query_type` (point/comparison/temporal/aggregation), `lang`. |
| `splits/` | (Optional) Predefined 5‑fold cross‑validation splits used in the paper. |
| `embeddings/` | (Optional) Precomputed multilingual‑E5‑large embeddings for all document chunks (numpy format). Useful for fast reproduction. |

**Note:** The full text of ESG reports is derived from publicly available disclosures. Redistribution respects the original sources; please cite the original companies if you use the data beyond academic research.

---

## 📁 Repository Structure
