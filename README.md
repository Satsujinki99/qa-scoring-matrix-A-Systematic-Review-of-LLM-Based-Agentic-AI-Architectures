# Agentic AI for Complex Task Execution — SLR Supplementary Data

This repository hosts the **supplementary data workbook** for the systematic literature review (SLR):

> **"Agentic AI for Complex Task Execution: A Systematic Review of LLM-Based Agentic AI Architectures"**


This repository is that supplementary material.

**Main file:** [`SLR_AgenticAI_Updated_Layering_DataExtraction_Report_UserGuide_CleanOverview.xlsx`](./SLR_AgenticAI_Updated_Layering_DataExtraction_Report_UserGuide_CleanOverview.xlsx)

The workbook documents the **entire study-selection process** — from the initial seed search through inclusion/exclusion screening to the final Quality Assessment (QA) scores for the 33 primary studies — so that the review is fully auditable and reproducible by readers and reviewers.

---

## Table of Contents

- [How to Cite](#how-to-cite)
- [Key Numbers (KPIs)](#key-numbers-kpis)
- [Sheet Structure](#sheet-structure)
- [Review Protocol (Layers 0–6)](#review-protocol-layers-0–6)
- [Scoring Criteria](#scoring-criteria)
- [How to Use the Workbook](#how-to-use-the-workbook)
- [Strict Non-ArXiv Policy](#strict-non-arxiv-policy)
- [The 33 Primary Studies](#the-33-primary-studies)
- [License](#license)

---

## How to Cite

This work has been **presented** at the following conference; the paper is currently pending inclusion in the official conference proceedings (IEEE Xplore).

> F. Aryadana, K. A. Faza, R. M. N. M. Bayuputra, and R. W. Sholikah, "Agentic AI for Complex Task Execution: A Systematic Review of LLM-Based Agentic AI Architectures," presented at the *2026 13th International Conference on Electrical Engineering, Computer Science and Informatics (EECSI 2026)*, 2026.

**Status:** To be presented at EECSI 2026. Final publication details (DOI, page numbers, IEEE Xplore link) will be added here once the proceedings are published—please check back or monitor this repository for updates.

**Authors / affiliation:**
Department of Information Technology, Sepuluh Nopember Institute of Technology (ITS), Surabaya, Indonesia
- Furqon Aryadana — 5027231024@student.its.ac.id
- Kevin Anugerah Faza — 5027231027@student.its.ac.id
- RM. Novian Malcolm Bayuputra — 5027231035@student.its.ac.id
- Rizka Wakhidatus Sholikah — wakhidatus@its.ac.id

If you use or reference this dataset, please cite the paper above and link back to this repository as the data source.

```bibtex
@inproceedings{aryadana2026agentic,
  title     = {Agentic AI for Complex Task Execution: A Systematic Review of LLM-Based Agentic AI Architectures},
  author    = {Aryadana, Furqon and Faza, Kevin Anugerah and Bayuputra, RM. Novian Malcolm and Sholikah, Rizka Wakhidatus},
  booktitle = {2026 13th International Conference on Electrical Engineering, Computer Science and Informatics (EECSI)},
  year      = {2026},
  note      = {Presented at EECSI 2026; proceedings publication pending},
  url       = {<link to this GitHub repository>}
}
```

---

## Key Numbers (KPIs)

| Item | Count | Description |
|---|---|---|
| ScienceDirect seed results | 87,375 | Initial discovery context using the keyword "Agentic AI", Research Articles + Review Articles, 2020–2026 |
| Candidate rows scored | 121 | Candidates consolidated from Elicit / reference-tracing lists |
| Final usable references | 72 | Non-ArXiv references usable as primary or background literature |
| **Main primary synthesis** | **33** | Primary studies used for data extraction and RQ synthesis |
| Background references | 39 | Supporting papers for Introduction / Related Work / Discussion |
| Excluded by ArXiv/URL rule | 44 | Removed due to arXiv venue, arXiv URL, or arXiv DOI policy |
| Excluded by other rules | 5 | Removed by other non-ArXiv Kitchenham exclusion reasons |
| Data extraction rows | 33 | Structured extraction for all Main Primary papers |

This summary is also available in the `Overview` sheet of the workbook, and mirrors the PRISMA flow diagram (Fig. 1) reported in the paper.

---

## Sheet Structure

| Sheet | Contents |
|---|---|
| `Overview` | Navigation dashboard: KPIs, workflow summary (Layers 0–6), and pointers to which sheet to open next |
| `Methodology` | Detailed user guide: definition of each layer, scoring criteria, and quality-control rules |
| `All_Candidates_Detailed` | **Master audit trail** — all 121 candidates with I1–I7 screening scores, ArXiv filter status, exclusion codes, QA1–QA7 scores, and final decision |
| `Final_Usable_All` | 72 non-ArXiv references that passed filtering (primary + background) |
| `Main_Primary_Synthesis` | 33 primary studies (Use_Type = *Main Primary*) — the basis for RQ1–RQ4 synthesis |
| `Data Extraction` | Structured data-extraction table (architecture, method, dataset, metric, findings, limitations, research gap) for the 33 primary studies |
| `Background_References` | 39 supporting papers (surveys, domain reviews, foundational LLM work) — not counted as primary evidence |
| `Excluded_ArXiv_URL` | 44 papers excluded due to arXiv venue/URL/DOI |
| `Excluded_Other` | 5 papers excluded for other non-ArXiv Kitchenham reasons |

---

## Review Protocol (Layers 0–6)

Study selection follows **Kitchenham's SLR guidelines** [Kitchenham & Charters, 2007] combined with **PICOC** scoping [Petticrew & Roberts, 2006] and **PRISMA-style** reporting [Page et al., 2021], applied through the following layered process:

| Layer | Name | Description |
|---|---|---|
| **0** | ScienceDirect seed search | Initial search for the keyword "Agentic AI" (Research + Review Articles, 2020–2026) used to establish topic scope; not a scored study set |
| **1** | Elicit / reference candidate pool | Candidates consolidated from Elicit (AI-assisted discovery) and reference tracing into 121 audited rows |
| **2** | Strict ArXiv venue exclusion | Papers whose venue contains "arXiv" / "arXiv.org" / "arXiv preprint" are removed before QA |
| **3** | Strict non-ArXiv URL enforcement | Papers whose only available DOI/URL is arXiv (e.g. `10.48550/arXiv...`) are removed; final links must point to an official, non-ArXiv venue or publisher record |
| **4** | Kitchenham inclusion screening (I1–I7) | Eligibility screening: topic relevance, task relevance, year, language, peer-reviewed/indexed venue, contribution, and full-text access (score 0–7) |
| **5** | Kitchenham exclusion codes (E1–E7) | Exclusion codes determine the final status: *Main Primary*, *Background Only*, or *Exclude* |
| **6** | Quality Assessment (QA1–QA7) | Methodological quality scoring (0–2 per item, maximum 14); threshold **QA ≥ 10** for *Main Primary* inclusion |

**Final outcomes:**

- **Main Primary** — non-ArXiv & QA ≥ 10 → used in Data Extraction and RQ1–RQ4 synthesis (33 studies)
- **Background Only** — supports Introduction / Related Work / Discussion, not counted as primary evidence (39 studies)
- **Exclude** — not used as a final reference; retained only for audit transparency (49 studies), consistent with PRISMA reporting principles

---

## Scoring Criteria

### Inclusion Screening (I1–I7) — maximum 7

| Code | Criterion | Score |
|---|---|---|
| I1 | Discusses/evaluates an LLM-based agentic AI architecture | 1 = yes, 0 = no |
| I2 | Relevant to complex task execution, multi-step reasoning, planning, or tool use | 1 = yes, 0 = no |
| I3 | Published between 2020–2026 | 1 = in range, 0 = out of range |
| I4 | Written in English | 1 = yes, 0 = no |
| I5 | Published in a peer-reviewed or indexed venue (not preprint-only) | 1 = yes, 0 = no |
| I6 | Substantial contribution (empirical study, architecture proposal, benchmark, or in-depth analysis) | 1 = yes, 0 = no |
| I7 | Full text accessible (open or institutional access) | 1 = yes, 0 = no |

### Quality Assessment (QA1–QA7) — maximum 14

Each item is scored **0–2** (0 = absent, 1 = partially addressed, 2 = fully addressed), covering: clarity of the proposed/evaluated agentic architecture, explicitness of study objective, description of architectural components (planning, memory, tool use, reflection, coordination), use of benchmarks/clearly defined task settings, methodological detail for reproducibility, comparison with baselines, and discussion of limitations.

| Total QA | Decision |
|---|---|
| 10–14 | **Include** as primary evidence (Main Primary) |
| 8–9 | Borderline |
| 0–7 | Excluded from primary synthesis |

### Exclusion codes (E1–E7)

Kitchenham exclusion codes explain why a paper was rejected or limited to background use (e.g., scope mismatch, non-agentic focus, duplication, inaccessible full text, survey/review nature, or arXiv-only record). See the `Updated_Exclusion_Codes` column in `All_Candidates_Detailed`, `Excluded_ArXiv_URL`, and `Excluded_Other` for per-paper detail.

---

## How to Use the Workbook

1. **Start with `Overview`** to understand the KPIs and overall workflow.
2. **Audit all candidates in `All_Candidates_Detailed`** — check I1–I7 scores, exclusion codes, QA scores, and the full decision trail (`Updated_Filtering_Path` records the complete Layer 0–6 path for every candidate).
3. **Use `Main_Primary_Synthesis`** to view the 33 primary studies — filter/sort by QA score, SLR category, or year.
4. **Use `Data Extraction`** for the full structured extraction (architecture, dataset, metrics, findings, limitations, research gaps), mapped directly to RQ1–RQ4.
5. **Use `Background_References`** only for contextual citations (Introduction / Related Work), not as primary evidence.
6. **Check `Excluded_ArXiv_URL` and `Excluded_Other`** to see why specific papers were rejected — useful for responding to reviewer questions about selection transparency.
7. Use Excel's built-in table filters (click the header arrow) to filter by `Use_Type`, `SLR_Category`, `QA_Total_Detail`, `Updated_Exclusion_Codes`, or `Venue`.

---

## Strict Non-ArXiv Policy

This workbook enforces a strict rule: **no arXiv paper (venue, URL, or `10.48550/arXiv...` DOI) may appear in the final reference set** (`Final_Usable_All`, `Main_Primary_Synthesis`, `Data Extraction`). If a paper had both an arXiv version and an official peer-reviewed record, only the official venue/publisher record was retained; if only an arXiv record existed, the paper was moved to `Excluded_ArXiv_URL` and excluded from both primary and background use.

---

## The 33 Primary Studies

These are the 33 studies that passed all filtering layers (non-ArXiv + Kitchenham QA ≥ 10) and form the primary evidence corpus analyzed in `Main_Primary_Synthesis` and `Data Extraction`:

1. S. Yao et al., "ReAct: Synergizing reasoning and acting in language models," ICLR, 2023.
2. N. Shinn et al., "Reflexion: Language agents with verbal reinforcement learning," NeurIPS, 2023.
3. J. S. Park et al., "Generative agents: Interactive simulacra of human behavior," UIST, 2023.
4. Y. Du et al., "Improving factuality and reasoning in language models through multiagent debate," ICML, 2024.
5. A. Zhou et al., "Language agent tree search unifies reasoning, acting, and planning in language models," ICML, 2024.
6. A. Prasad et al., "ADaPT: As-needed decomposition and planning with language models," Findings of ACL: NAACL, 2024.
7. Y. Qin et al., "ToolLLM: Facilitating large language models to master 16000+ real-world APIs," ICLR, 2024.
8. Y. Shen et al., "HuggingGPT: Solving AI tasks with ChatGPT and its friends in Hugging Face," NeurIPS, 2023.
9. J. Yang et al., "SWE-agent: Agent-computer interfaces enable automated software engineering," NeurIPS, 2024.
10. A. Drouin et al., "WorkArena: How capable are web agents at solving common knowledge work tasks?" ICML, 2024.
11. J. Y. Koh et al., "VisualWebArena: Evaluating multimodal agents on realistic visually grounded web tasks," ACL, 2024.
12. X. Liu et al., "AgentBench: Evaluating LLMs as agents," ICLR, 2024.
13. Z. Zhao, W. S. Lee, and D. Hsu, "Large language models as commonsense knowledge for large-scale task planning," NeurIPS, 2023.
14. Z. Chen et al., "When is tree search useful for LLM planning? It depends on the discriminator," ACL, 2024, pp. 13659–13678.
15. Z. Shi et al., "Tool learning in the wild: Empowering language models as automatic tool agents," WWW, 2025.
16. X. Tan et al., "Meta-Agent-Workflow: Streamlining tool usage in LLMs through workflow construction, retrieval, and refinement," WWW Companion, 2025.
17. R. Salama et al., "MemInsight: Autonomous memory augmentation for LLM agents," EMNLP, 2025, pp. 33136–33152.
18. C. Hong and Q. He, "Enhancing memory retrieval in generative agents through LLM-trained cross attention networks," Frontiers in Psychology, vol. 16, Art. no. 1591618, 2025.
19. P. Yu, G. Chen, and J. Wang, "Table-Critic: A multi-agent framework for collaborative criticism and refinement in table reasoning," ACL, 2025, pp. 17432–17451.
20. G. Chen et al., "AutoAgents: A framework for automatic agent generation," IJCAI, 2024.
21. T. Webb, S. S. Mondal, and I. Momennejad, "A brain-inspired agentic architecture to improve planning with LLMs," Nature Communications, vol. 16, Art. no. 8633, 2025.
22. M. Hu et al., "AgentGen: Enhancing planning abilities for large language model based agent via environment and task generation," KDD, 2025.
23. W. Chen et al., "Internet of agents: Weaving a web of heterogeneous agents for collaborative intelligence," ICLR, 2025.
24. H. Zhang et al., "Building cooperative embodied agents modularly with large language models," ICLR, 2024.
25. G. Yin et al., "MMAU: A holistic benchmark of agent capabilities across diverse domains," NAACL, 2025, pp. 4752–4780.
26. D. Roy et al., "Exploring LLM-based agents for root cause analysis," FSE Companion, 2024.
27. T. Birr et al., "AutoGPT+P: Affordance-based task planning using large language models," RSS, 2024.
28. X. Zhu et al., "MultiAgentBench: Evaluating the collaboration of LLM agents," ACL, 2025.
29. Y. Gu et al., "Is your LLM secretly a world model of the Internet? Model-based planning for web agents," TMLR, 2025.
30. J. Liu et al., "Mobile-Bench: An evaluation benchmark for LLM-based mobile agents," ACL, 2025.
31. D. Koh et al., "Tree search for language model agents," ICLR, 2024.
32. H. Cui et al., "LLMind: Orchestrating AI and IoT with LLM for complex task execution," IEEE Communications Magazine, 2025.
33. L. Cross et al., "Hypothetical minds: Scaffolding theory of mind for multi-agent tasks with large language models," ICLR, 2025.

Full details (authors, exact venues, DOIs/links, QA and screening scores, and structured data extraction) for each of these 33 studies are in the `Main_Primary_Synthesis` and `Data Extraction` sheets of the workbook.

---

## License

Add an appropriate license for this dataset (e.g. [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) is common for research supplementary data) and include a `LICENSE` file at the repository root.
