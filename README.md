# Awosome_VA

[한국어 README](README_kor.md)

> Curated resources for **SciML & CFD research**, **graduate-student workflows**, and **AI-assisted productivity**.

This repository is a lightweight knowledge base for papers, tools, repositories, workflows, and technical notes. It started from CFD × Scientific Machine Learning resources, but also tracks useful material for research writing, lab productivity, AI coding agents, document tools, and operational safety.

## Big picture

| Theme | What belongs here | Good entry point |
|---|---|---|
| **SciML & CFD** | CFD solvers, AMR, OpenFOAM, meshing, JAX prototypes, neural operators, optimization, visualization | [SciML & CFD resources](#sciml--cfd) |
| **Graduate research workflow** | paper writing, research automation, presentation/report structure, seminars, academic opportunities | [Graduate research workflow](#graduate-research-workflow) |
| **AI agents & productivity tools** | Claude/Codex/OpenCode, local LLMs, skills/harnesses, voice-to-prompt, Google/agent tooling | [AI agents & productivity](#ai-agents--productivity) |
| **Documents, admin & operations** | HWP tools, events, cloud cost/security, miscellaneous useful utilities | [Documents, admin & operations](#documents-admin--operations) |

## SciML & CFD

| Area | Start here | Representative resources | Use when you want to… |
|---|---|---|---|
| **Differentiable CFD / AMR** | [Differentiable CFD & AMR solvers](resources/differentiable-cfd-amr.md) | JAX-AMR, JANC, geometry-autoencoder PINNs | build or study JAX-based CFD, AMR, differentiable solvers, geometry-varying PINNs |
| **Meshing / HPC CFD** | [Meshing & GPU workflows](resources/meshing-gpu-workflows.md) · [GPU OpenFOAM](resources/gpu-openfoam-hpc.md) | PhysicsNeMo-Mesh, SALOME/Gmsh/Pointwise, OpenFOAM GPU acceleration | connect geometry/mesh generation with GPU CFD workflows |
| **OpenFOAM practice** | [OpenFOAM tips](resources/openfoam-tips.md) | solver reference, square-cylinder notes, `startFrom latestTime` | debug solver choices, continue runs, or explain basic OpenFOAM behavior |
| **JAX CFD prototypes** | [JAX-based CFD prototypes](resources/jax-cfd-prototypes.md) | IBM airfoil flap, GUI prototype, wind turbine toy model | prototype flow simulations quickly with JAX/agents |
| **Visualization** | [Visualization & post-processing](resources/visualization-postprocessing.md) · [Weather/climate visualization](resources/weather-climate-visualization.md) | Omniverse Q-criterion, Earth2Studio, black-hole simulation visualization | turn simulation or ML field outputs into interpretable visuals |
| **CAD / geometry AI** | [CAD, geometry & AI-assisted design](resources/cad-geometry-ai.md) | ForgeCAD, FreeCAD + Claude Code | generate or iterate CFD/CAE geometries with coding agents |
| **Neural operators / architectures** | [Neural operators & tensor methods](resources/neural-operators-tensor-methods.md) · [Optimization for SciML](resources/optimization-sciml.md) | Tensor trains, Mamba-3, SpecMuon, Attention Residuals | track model architectures, optimizers, and compression ideas for SciML |
| **Fluid/AI education** | [Fluid mechanics, turbulence & AI education](resources/education-fluid-ai.md) | VinuesaLab | learn fluid mechanics, turbulence, interpretable ML, and AI-for-science perspectives |
| **Math foundations** | [Mathematical foundations](resources/math-foundations.md) | function representation notes | keep theoretical but potentially relevant math ideas |

## Graduate research workflow

| Area | Start here | Representative resources | Use when you want to… |
|---|---|---|---|
| **Research automation & writing** | [Research automation & writing](resources/research-automation-writing.md) | PaperOrchestra, PaperBanana, Feynman, Overleaf MCP, AI Scientist | automate literature review, draft papers, generate figures, or verify citations |
| **Presentation / report structure** | [Research presentation & report structure](resources/research-presentation-workflow.md) | scenario → metric → data → learning → analysis → application workflow | structure lab seminar slides, reports, and research narratives |
| **Events & opportunities** | [Events & opportunities](resources/events-opportunities.md) | SEMICON, industry/career signals | track time-sensitive academic/industry opportunities |

## AI agents & productivity

| Area | Start here | Representative resources | Use when you want to… |
|---|---|---|---|
| **Agent tools** | [Agent tools & research workflow](resources/agent-tools-workflow.md) | Claude Code tips, Codex/OpenCode, Google Workspace CLI, skills/harnesses | use coding agents effectively for research and software tasks |
| **Lab AI adoption** | [AI coding & lab adoption](resources/ai-coding-lab-adoption.md) | shared Claude/API strategy, lab seminar idea, Codex support program | design a lab-wide AI usage strategy and onboarding flow |
| **Local AI workflow** | [Local AI research workflow](resources/local-ai-workflow.md) | whatcani.run, Gemma/local LLMs | run private/local AI workflows and estimate local model capability |

## Documents, admin & operations

| Area | Start here | Representative resources | Use when you want to… |
|---|---|---|---|
| **Document/admin tools** | [Miscellaneous tools](resources/misc-tools.md) | HOP Open HWP, image/video AI notes | handle useful peripheral tools, especially Korean document workflows |
| **Security / cost / ops** | [Security, cost & operations](resources/security-cost-ops.md) | AWS billing incident, secret/cost reminders | avoid expensive mistakes when using cloud, agents, and credentials |

## Current highlights

- **JAX-AMR / JANC** — accelerator-friendly AMR and differentiable CFD solver references.
- **PhysicsNeMo-Mesh + OpenFOAM GPU acceleration** — two directions for faster CFD pipelines: modern GPU-native mesh/ML tooling and conventional solver acceleration.
- **JAX CFD prototypes** — airfoil flap, wind turbine, and GUI-style quick simulation workflows suggest a practical path for rapid CFD-ML prototyping.
- **ForgeCAD / FreeCAD + Claude Code** — agent-assisted geometry generation may become useful for early CFD/CAE design loops.
- **PaperOrchestra / Feynman / PaperBanana** — early signs of multi-agent research writing, reviewing, figure generation, and source verification workflows.

## Suggested workflows

### Build a CFD-ML prototype

1. Start with [JAX-based CFD prototypes](resources/jax-cfd-prototypes.md).
2. Check solver/AMR ideas in [Differentiable CFD & AMR solvers](resources/differentiable-cfd-amr.md).
3. Use [CAD/geometry AI](resources/cad-geometry-ai.md) or [Meshing & GPU workflows](resources/meshing-gpu-workflows.md) for geometry/mesh ideas.
4. Visualize results with [Visualization & post-processing](resources/visualization-postprocessing.md).

### Prepare a paper or report

1. Structure the story with [Research presentation & report structure](resources/research-presentation-workflow.md).
2. Collect evidence and drafts with [Research automation & writing](resources/research-automation-writing.md).
3. Use [Agent tools & research workflow](resources/agent-tools-workflow.md) for coding-agent practices.
4. Audit claims, citations, figures, and numerical validation manually.

### Set up lab AI usage

1. Start with [AI coding & lab adoption](resources/ai-coding-lab-adoption.md).
2. Compare [Agent tools](resources/agent-tools-workflow.md) and [Local AI workflow](resources/local-ai-workflow.md).
3. Keep [Security, cost & operations](resources/security-cost-ops.md) visible before giving agents credentials or cloud access.

## Curation rules

- Prefer resources useful for SciML/CFD research, graduate research workflow, AI productivity, or lab operations.
- Skip assignments, private lab logistics, and ephemeral Slack chatter unless it contains a reusable resource.
- Keep each entry short: link, why it matters, and possible use.
- Put detailed notes in `resources/*.md`; keep this README as the dashboard.

## Maintainer note

VA_claw can keep this repository updated from shared links, papers, repositories, and notes.
