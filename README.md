# Awosome_VA

> Curated resources for **CFD × Scientific Machine Learning × AI-assisted engineering**.

This repository is a lightweight knowledge base for papers, tools, repositories, workflows, and technical notes that may help with CFD-ML research, differentiable simulation, neural operators, meshing, research automation, and safe AI-assisted engineering.

## Quick map

| Area | Start here | Representative resources | Use when you want to… |
|---|---|---|---|
| **Differentiable CFD / AMR** | [Differentiable CFD & AMR solvers](resources/differentiable-cfd-amr.md) | JAX-AMR, JANC, geometry-autoencoder PINNs | build or study JAX-based CFD, AMR, differentiable solvers, geometry-varying PINNs |
| **Meshing / HPC CFD** | [Meshing & GPU workflows](resources/meshing-gpu-workflows.md) · [GPU OpenFOAM](resources/gpu-openfoam-hpc.md) | PhysicsNeMo-Mesh, SALOME/Gmsh/Pointwise, OpenFOAM GPU acceleration | connect geometry/mesh generation with GPU CFD workflows |
| **OpenFOAM practice** | [OpenFOAM tips](resources/openfoam-tips.md) | solver reference, square-cylinder notes, `startFrom latestTime` | debug solver choices, continue runs, or explain basic OpenFOAM behavior |
| **JAX CFD prototypes** | [JAX-based CFD prototypes](resources/jax-cfd-prototypes.md) | IBM airfoil flap, GUI prototype, wind turbine toy model | prototype flow simulations quickly with JAX/agents |
| **Visualization** | [Visualization & post-processing](resources/visualization-postprocessing.md) · [Weather/climate visualization](resources/weather-climate-visualization.md) | Omniverse Q-criterion, Earth2Studio, black-hole simulation visualization | turn simulation or ML field outputs into interpretable visuals |
| **CAD / geometry AI** | [CAD, geometry & AI-assisted design](resources/cad-geometry-ai.md) | ForgeCAD, FreeCAD + Claude Code | generate or iterate CFD/CAE geometries with coding agents |
| **Neural operators / architectures** | [Neural operators & tensor methods](resources/neural-operators-tensor-methods.md) · [Optimization for SciML](resources/optimization-sciml.md) | Tensor trains, Mamba-3, SpecMuon, Attention Residuals | track model architectures, optimizers, and compression ideas for SciML |
| **Research automation** | [Research automation & writing](resources/research-automation-writing.md) | PaperOrchestra, PaperBanana, Feynman, Overleaf MCP, AI Scientist | automate literature review, draft papers, generate figures, or verify citations |
| **Agent workflow** | [Agent tools](resources/agent-tools-workflow.md) · [AI coding & lab adoption](resources/ai-coding-lab-adoption.md) · [Local AI workflow](resources/local-ai-workflow.md) | Claude Code tips, Codex/OpenCode, skills/harnesses, Gemma/local LLMs | set up personal/lab AI coding workflows and share best practices |
| **Education / opportunities / ops** | [Fluid/AI education](resources/education-fluid-ai.md) · [Events](resources/events-opportunities.md) · [Security/cost/ops](resources/security-cost-ops.md) | VinuesaLab, SEMICON, AWS billing incident | learn, find opportunities, and avoid expensive/safety mistakes |
| **Other useful notes** | [Math foundations](resources/math-foundations.md) · [Presentation workflow](resources/research-presentation-workflow.md) · [Misc tools](resources/misc-tools.md) | function representation, report structure, HOP HWP | keep useful peripheral material organized |

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

- Prefer resources directly useful for CFD, Scientific ML, CAE, differentiable simulation, or research automation.
- Skip assignments, private lab logistics, and ephemeral Slack chatter unless it contains a reusable resource.
- Keep each entry short: link, why it matters, and possible use.
- Put detailed notes in `resources/*.md`; keep this README as the dashboard.

## Maintainer note

VA_claw can keep this repository updated from shared links, papers, repositories, and notes.
