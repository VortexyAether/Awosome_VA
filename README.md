<div align="center">

# 🌊 Awosome_VA

### Curated resources for **SciML · CFD · AI-assisted research workflows**

[![SciML](https://img.shields.io/badge/SciML-CFD-2563eb?style=for-the-badge)](#-sciml--cfd)
[![Agents](https://img.shields.io/badge/AI%20Agents-Productivity-7c3aed?style=for-the-badge)](#-ai-agents--productivity)
[![Graduate](https://img.shields.io/badge/Graduate-Workflow-16a34a?style=for-the-badge)](#-graduate-research-workflow)
[![Korean](https://img.shields.io/badge/README-한국어-dc2626?style=for-the-badge)](README_kor.md)

*A living index for papers, tools, repositories, workflows, and technical notes useful to CFD-ML research and graduate-student productivity.*

</div>

---

## 🧭 Quick navigation

| 🚀 Theme | What it covers | Jump in |
|---|---|---|
| **SciML & CFD** | solvers, AMR, OpenFOAM, meshing, JAX prototypes, neural operators, visualization | [Go](#-sciml--cfd) |
| **Graduate research workflow** | paper writing, research automation, presentation/report structure, academic opportunities | [Go](#-graduate-research-workflow) |
| **AI agents & productivity** | Claude/Codex/OpenCode, local LLMs, skills/harnesses, agent-friendly tooling | [Go](#-ai-agents--productivity) |
| **Documents, admin & operations** | HWP tools, events, security, cloud cost, miscellaneous utilities | [Go](#-documents-admin--operations) |

---

## 🔬 SciML & CFD

| Category | Best starting point | Representative resources |
|---|---|---|
| 🧪 **Differentiable CFD / AMR** | [Differentiable CFD & AMR solvers](resources/differentiable-cfd-amr.md) | JAX-AMR, JANC, geometry-autoencoder PINNs |
| 🧱 **Meshing / HPC CFD** | [Meshing & GPU workflows](resources/meshing-gpu-workflows.md) · [GPU OpenFOAM](resources/gpu-openfoam-hpc.md) | PhysicsNeMo-Mesh, SALOME/Gmsh/Pointwise, OpenFOAM GPU acceleration |
| 🌪️ **OpenFOAM practice** | [OpenFOAM tips](resources/openfoam-tips.md) | solver reference, square-cylinder notes, `startFrom latestTime` |
| ⚡ **JAX CFD prototypes** | [JAX-based CFD prototypes](resources/jax-cfd-prototypes.md) | IBM airfoil flap, GUI prototype, wind turbine toy model |
| 🎞️ **Visualization** | [Visualization & post-processing](resources/visualization-postprocessing.md) · [Weather/climate visualization](resources/weather-climate-visualization.md) | Omniverse Q-criterion, Earth2Studio, black-hole simulation visualization |
| 🧩 **CAD / geometry AI** | [CAD, geometry & AI-assisted design](resources/cad-geometry-ai.md) | ForgeCAD, FreeCAD + Claude Code |
| 🧠 **Neural operators / architectures** | [Neural operators & tensor methods](resources/neural-operators-tensor-methods.md) · [Optimization for SciML](resources/optimization-sciml.md) | Tensor trains, Mamba-3, SpecMuon, Attention Residuals |
| 🎓 **Fluid/AI education** | [Fluid mechanics, turbulence & AI education](resources/education-fluid-ai.md) | VinuesaLab |
| ∑ **Math foundations** | [Mathematical foundations](resources/math-foundations.md) | function representation notes |

---

## 🧑‍🎓 Graduate research workflow

| Category | Best starting point | Representative resources |
|---|---|---|
| ✍️ **Research automation & writing** | [Research automation & writing](resources/research-automation-writing.md) | PaperOrchestra, PaperBanana, Feynman, Overleaf MCP, AI Scientist |
| 🗂️ **Presentation / report structure** | [Research presentation & report structure](resources/research-presentation-workflow.md) | scenario → metric → data → learning → analysis → application workflow |
| 📌 **Events & opportunities** | [Events & opportunities](resources/events-opportunities.md) | SEMICON, industry/career signals |

---

## 🤖 AI agents & productivity

| Category | Best starting point | Representative resources |
|---|---|---|
| 🛠️ **Agent tools** | [Agent tools & research workflow](resources/agent-tools-workflow.md) | Claude Code tips, Codex/OpenCode, Google Workspace CLI, skills/harnesses, 500+ AI agent use cases |
| 🏫 **Lab AI adoption** | [AI coding & lab adoption](resources/ai-coding-lab-adoption.md) | shared Claude/API strategy, lab seminar idea, Codex support program |
| 💻 **Local AI workflow** | [Local AI research workflow](resources/local-ai-workflow.md) | whatcani.run, Gemma/local LLMs |

---

## 📄 Documents, admin & operations

| Category | Best starting point | Representative resources |
|---|---|---|
| 📝 **Document/admin tools** | [Miscellaneous tools](resources/misc-tools.md) | HOP Open HWP, image/video AI notes |
| 🔐 **Security / cost / ops** | [Security, cost & operations](resources/security-cost-ops.md) | AWS billing incident, secret/cost reminders |

---

## ✨ Current highlights

- **JAX-AMR / JANC** — accelerator-friendly AMR and differentiable CFD solver references.
- **PhysicsNeMo-Mesh + OpenFOAM GPU acceleration** — GPU-native mesh/ML tooling and conventional solver acceleration.
- **JAX CFD prototypes** — airfoil flap, wind turbine, and GUI-style simulation workflows for rapid CFD-ML prototyping.
- **ForgeCAD / FreeCAD + Claude Code** — agent-assisted geometry generation for early CFD/CAE design loops.
- **PaperOrchestra / Feynman / PaperBanana** — multi-agent paper writing, reviewing, figure generation, and source verification.

---

## 🧪 Suggested workflows

<details>
<summary><b>Build a CFD-ML prototype</b></summary>

1. Start with [JAX-based CFD prototypes](resources/jax-cfd-prototypes.md).
2. Check solver/AMR ideas in [Differentiable CFD & AMR solvers](resources/differentiable-cfd-amr.md).
3. Use [CAD/geometry AI](resources/cad-geometry-ai.md) or [Meshing & GPU workflows](resources/meshing-gpu-workflows.md) for geometry/mesh ideas.
4. Visualize results with [Visualization & post-processing](resources/visualization-postprocessing.md).

</details>

<details>
<summary><b>Prepare a paper or report</b></summary>

1. Structure the story with [Research presentation & report structure](resources/research-presentation-workflow.md).
2. Collect evidence and drafts with [Research automation & writing](resources/research-automation-writing.md).
3. Use [Agent tools & research workflow](resources/agent-tools-workflow.md) for coding-agent practices.
4. Audit claims, citations, figures, and numerical validation manually.

</details>

<details>
<summary><b>Set up lab AI usage</b></summary>

1. Start with [AI coding & lab adoption](resources/ai-coding-lab-adoption.md).
2. Compare [Agent tools](resources/agent-tools-workflow.md) and [Local AI workflow](resources/local-ai-workflow.md).
3. Keep [Security, cost & operations](resources/security-cost-ops.md) visible before giving agents credentials or cloud access.

</details>

---

## 🧹 Curation rules

- Prefer resources useful for **SciML/CFD research**, **graduate research workflow**, **AI productivity**, or **lab operations**.
- Skip assignments, private lab logistics, and ephemeral Slack chatter unless it contains a reusable resource.
- Keep each entry short: link, why it matters, and possible use.
- Put detailed notes in `resources/*.md`; keep this README as the dashboard.

---

<div align="center">

Maintained with 🦞 by **VA_claw**.

</div>
