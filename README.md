# TemporalESG: Trilingual Benchmark for Time-Critical ESG Retrieval

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

This repository contains the code and query sets for the **TemporalESG benchmark**, introduced in the paper:

> *“Bridging the Temporal-Semantic Gap: A Trilingual Benchmark and Hybrid Retrieval Framework for Time-Critical ESG Information Access”* (Information Processing & Management, 2025).

The benchmark evaluates retrieval systems on **temporal‑aware, entity‑centric** queries in the Environmental, Social, and Governance (ESG) domain. It includes **40,814 multilingual document chunks** (Vietnamese, English, Arabic) from 43 multinational corporations over 11 years (2015–2025) and **970 validated temporal queries**. Due to storage limitations, the full document collection is hosted externally.

---

## Repository Contents

| File | Description |
|------|-------------|
| `200_additional_queries (1).json` | 200 generated queries (before validation) |
| `800_new_queries (1).json` | 800 generated queries (before validation) |
| `temporalesg_pipeline` | Main Python script for hybrid retrieval (BM25 + dense embeddings + temporal decay) |
| `LICENSE` | Creative Commons Attribution 4.0 International license |
| `README.md` | This file |

**Note:** The final **970 validated queries** used in the paper are a subset of the 1,000 generated queries (200 + 800). The validation process (manual review, inter‑annotator agreement) is described in the paper.

---

## Document Collection

The full set of **40,814 document chunks** is available for download at:

🔗 [https://drive.google.com/file/d/1jZMaQoiqUgqyitOzSvaMJuoLR2c5Eh0o/view?usp=sharing](https://drive.google.com/file/d/1jZMaQoiqUgqyitOzSvaMJuoLR2c5Eh0o/view?usp=sharing)

After downloading, extract the contents and update the `DATA_DIR` path in the script.

---

