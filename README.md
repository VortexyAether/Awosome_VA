<div align="center">

# 🌊 Awesome_VA

### A curated **CFD-AI / SciML Research Radar** for engineering research workflows

[![SciML](https://img.shields.io/badge/SciML-CFD-2563eb?style=for-the-badge)](#research-map)
[![CFD AI](https://img.shields.io/badge/CFD--AI-Research%20Radar-0891b2?style=for-the-badge)](#what-belongs-here)
[![Agents](https://img.shields.io/badge/AI%20Agents-Research%20Workflow-7c3aed?style=for-the-badge)](#agentic-workflows)
[![Korean](https://img.shields.io/badge/README-한국어-dc2626?style=for-the-badge)](README_kor.md)

*Selected papers, code, datasets, tools, and workflow notes for a CFD-AI / Scientific Machine Learning graduate researcher.*

</div>

---

## What this repository is

**Awesome_VA is not a bookmark dump.** It is a research radar: a small, opinionated, continuously curated map of resources that may actually help design experiments, understand the SciML frontier, write papers, automate engineering workflows, or connect CFD-AI with nuclear engineering and AI agents.

The guiding rule is simple:

> **It is better to add 3 good resources than 20 mediocre ones.**

---

## What belongs here

A resource should answer at least one of these questions:

1. Does it help design better **CFD-AI / SciML experiments**?
2. Does it clarify the current frontier in **neural operators, differentiable solvers, turbulence surrogates, or generative physics models**?
3. Does it provide a tool, dataset, metric, benchmark, solver, or workflow I may actually use?
4. Does it help with **paper writing, literature review, coding, automation, or graduate research productivity**?
5. Does it connect CFD-AI with **nuclear engineering, digital twins, safety-code automation, or AI agents**?

If the answer is no, it should not be added.

---

## Research map

| Area | Resource file | Focus |
|---|---|---|
| **Differentiable CFD & AMR** | [resources/differentiable-cfd-amr.md](resources/differentiable-cfd-amr.md) | Differentiable solvers, adaptive discretization, JAX/ML-native PDE systems |
| **JAX / Python PDE solvers** | [resources/jax-cfd-prototypes.md](resources/jax-cfd-prototypes.md) · [resources/jax-pde-solvers.md](resources/jax-pde-solvers.md) | JAX-CFD, PhiFlow, FiPy-style prototypes, lightweight CFD backends |
| **Neural operators & tensor methods** | [resources/neural-operators-tensor-methods.md](resources/neural-operators-tensor-methods.md) | FNO, operator learning, tensor methods, QTT, spectral/operator architectures |
| **Turbulence surrogate models** | [resources/turbulence-surrogate-models.md](resources/turbulence-surrogate-models.md) | Turbulence prediction, super-resolution, autoregressive flow prediction |
| **Diffusion & generative physics** | [resources/diffusion-generative-physics.md](resources/diffusion-generative-physics.md) | Diffusion/EDM-style models, deterministic generative models, spectral consistency |
| **OpenFOAM & engineering CFD workflows** | [resources/openfoam-ai-workflows.md](resources/openfoam-ai-workflows.md) · [resources/openfoam-tips.md](resources/openfoam-tips.md) | OpenFOAM automation, safety checks, AI-assisted case setup and post-processing |
| **CAD, meshing & geometry AI** | [resources/cad-geometry-ai.md](resources/cad-geometry-ai.md) · [resources/meshing-gpu-workflows.md](resources/meshing-gpu-workflows.md) | FreeCAD, ForgeCAD, geometry agents, mesh generation, SDF/voxel workflows |
| **Visualization & post-processing** | [resources/visualization-postprocessing.md](resources/visualization-postprocessing.md) | ParaView, PyVista, VTK, scientific visualization, visual debugging |
| **Datasets & benchmarks** | [resources/datasets-benchmarks.md](resources/datasets-benchmarks.md) | Flow datasets, benchmarks, metrics, reproducibility references |
| **Nuclear AI & safety-code agents** | [resources/nuclear-ai-agents.md](resources/nuclear-ai-agents.md) | Nuclear engineering AI, digital twins, safety-code automation, LLM agents |
| **Research productivity agents** | [resources/research-productivity-agents.md](resources/research-productivity-agents.md) · [resources/research-automation-writing.md](resources/research-automation-writing.md) | Literature review, experiment automation, coding assistants, lab workflows |
| **Paper writing tools** | [resources/paper-writing-tools.md](resources/paper-writing-tools.md) | Writing, citation, LaTeX, figure, review, and proposal workflows |
| **Weekly / daily radar** | [resources/weekly-digest.md](resources/weekly-digest.md) · [daily/](daily/) | Daily research finds and weekly synthesis |

---

## Agentic workflows

This repository is designed to be maintained by a careful research-curation agent. The agent should:

- search arXiv, Papers with Code, GitHub, Semantic Scholar, Hugging Face, lab blogs, and conference pages when relevant;
- read at least the abstract, README, or project description before adding anything;
- prefer code-backed, reproducible, technically deep resources;
- mark speculative or immature items as `watchlist` rather than overstating them;
- avoid SEO spam, shallow AI content, vague social posts, and random link hoarding.

Operational details live in [CURATION.md](CURATION.md).

---

## Entry format

Each saved resource should use this structure:

```markdown
## Title of the resource

- Link: URL
- Type: Paper / Code / Dataset / Tool / Blog / Lecture / Benchmark / Workflow
- Keywords: keyword1, keyword2, keyword3
- One-line summary: A concise explanation of what this is.
- Why it matters: Why this matters from a CFD-AI / SciML research perspective.
- Possible use: How it may support research, writing, experiments, or workflow automation.
- Maturity: paper-only / prototype / maintained library / production-ready / watchlist
- Priority: High / Medium / Low
```

---

## Daily digest format

Daily updates should be stored under `daily/YYYY-MM-DD.md` and include:

- 3–5 highlights
- added resources grouped by category
- best find of the day
- 1–3 practical research ideas

See [daily/README.md](daily/README.md) for the template.

---

## Curation principles

- Keep the front page as a dashboard; put detailed notes in `resources/*.md`.
- Add fewer, better resources.
- Be honest about maturity, missing code, weak documentation, and abandoned repositories.
- Prefer concise but meaningful summaries.
- Use English by default; Korean notes are welcome when they capture personal research insight better.

---

<div align="center">

Maintained with 🦞 by **VA_claw** for **VortexyAether**.

</div>
