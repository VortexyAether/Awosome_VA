<div align="center">

# 🌊 Awesome_VA

### 공학 연구 워크플로우를 위한 **CFD-AI / SciML Research Radar**

[![SciML](https://img.shields.io/badge/SciML-CFD-2563eb?style=for-the-badge)](#research-map)
[![CFD AI](https://img.shields.io/badge/CFD--AI-Research%20Radar-0891b2?style=for-the-badge)](#이-저장소에-들어올-수-있는-것)
[![Agents](https://img.shields.io/badge/AI%20Agents-Research%20Workflow-7c3aed?style=for-the-badge)](#agentic-workflows)
[![English](https://img.shields.io/badge/README-English-dc2626?style=for-the-badge)](README.md)

*CFD-AI / Scientific Machine Learning 대학원 연구자 관점에서 선별한 논문, 코드, 데이터셋, 도구, 워크플로우 노트.*

</div>

---

## 이 저장소는 무엇인가

**Awesome_VA는 단순 북마크 저장소가 아니다.** 이 저장소는 research radar다. CFD-AI 실험 설계, SciML 연구 흐름 파악, 논문 작성, 공학 워크플로우 자동화, nuclear engineering / digital twin / AI agent 연결에 실제로 도움이 될 만한 자료만 선별한다.

가장 중요한 원칙:

> **평범한 자료 20개보다 좋은 자료 3개가 낫다.**

---

## 이 저장소에 들어올 수 있는 것

각 자료는 최소 하나 이상의 질문에 답해야 한다.

1. 더 나은 **CFD-AI / SciML 실험**을 설계하는 데 도움이 되는가?
2. **Neural operator, differentiable solver, turbulence surrogate, generative physics model**의 연구 최전선을 이해하는 데 도움이 되는가?
3. 실제로 쓸 수 있는 tool, dataset, metric, benchmark, solver, workflow를 제공하는가?
4. **논문 작성, 문헌조사, 코딩, 실험 자동화, 대학원 연구 생산성**에 도움이 되는가?
5. CFD-AI를 **nuclear engineering, digital twin, safety-code automation, AI agent**와 연결하는가?

답이 아니라면 추가하지 않는다.

---

## Research map

| 영역 | 문서 | 초점 |
|---|---|---|
| **Differentiable CFD & AMR** | [resources/differentiable-cfd-amr.md](resources/differentiable-cfd-amr.md) | Differentiable solver, adaptive discretization, JAX/ML-native PDE system |
| **JAX / Python PDE solvers** | [resources/jax-cfd-prototypes.md](resources/jax-cfd-prototypes.md) · [resources/jax-pde-solvers.md](resources/jax-pde-solvers.md) | JAX-CFD, PhiFlow, FiPy 계열 prototype, lightweight CFD backend |
| **Neural operators & tensor methods** | [resources/neural-operators-tensor-methods.md](resources/neural-operators-tensor-methods.md) | FNO, operator learning, tensor method, QTT, spectral/operator architecture |
| **Turbulence surrogate models** | [resources/turbulence-surrogate-models.md](resources/turbulence-surrogate-models.md) | Turbulence prediction, super-resolution, autoregressive flow prediction |
| **Diffusion & generative physics** | [resources/diffusion-generative-physics.md](resources/diffusion-generative-physics.md) | Diffusion/EDM-style model, deterministic generative model, spectral consistency |
| **OpenFOAM & engineering CFD workflows** | [resources/openfoam-ai-workflows.md](resources/openfoam-ai-workflows.md) · [resources/openfoam-tips.md](resources/openfoam-tips.md) | OpenFOAM 자동화, safety check, AI-assisted case setup/post-processing |
| **CAD, meshing & geometry AI** | [resources/cad-geometry-ai.md](resources/cad-geometry-ai.md) · [resources/meshing-gpu-workflows.md](resources/meshing-gpu-workflows.md) | FreeCAD, ForgeCAD, geometry agent, mesh generation, SDF/voxel workflow |
| **Visualization & post-processing** | [resources/visualization-postprocessing.md](resources/visualization-postprocessing.md) | ParaView, PyVista, VTK, scientific visualization, visual debugging |
| **Datasets & benchmarks** | [resources/datasets-benchmarks.md](resources/datasets-benchmarks.md) | Flow dataset, benchmark, metric, reproducibility reference |
| **Nuclear AI & safety-code agents** | [resources/nuclear-ai-agents.md](resources/nuclear-ai-agents.md) | Nuclear engineering AI, digital twin, safety-code automation, LLM agent |
| **Research productivity agents** | [resources/research-productivity-agents.md](resources/research-productivity-agents.md) · [resources/research-automation-writing.md](resources/research-automation-writing.md) | Literature review, experiment automation, coding assistant, lab workflow |
| **Paper writing tools** | [resources/paper-writing-tools.md](resources/paper-writing-tools.md) | Writing, citation, LaTeX, figure, review, proposal workflow |
| **Weekly / daily radar** | [resources/weekly-digest.md](resources/weekly-digest.md) · [daily/](daily/) | 매일 수집한 연구 신호와 주간 요약 |

---

## Agentic workflows

이 저장소는 신중한 research-curation agent가 관리할 수 있도록 설계한다. Agent는:

- 필요할 때 arXiv, Papers with Code, GitHub, Semantic Scholar, Hugging Face, 연구실 blog, conference page를 확인한다.
- 자료를 추가하기 전에 최소한 abstract, README, project description을 읽는다.
- code availability, reproducibility, technical depth를 우선한다.
- 아직 미성숙하거나 speculative한 자료는 과장하지 않고 `watchlist`로 표시한다.
- SEO spam, 얕은 AI 글, 모호한 SNS 글, 무작위 링크 수집을 피한다.

운영 규칙은 [CURATION.md](CURATION.md)에 정리한다.

---

## Entry format

각 자료는 다음 형식을 따른다.

```markdown
## Title of the resource

- Link: URL
- Type: Paper / Code / Dataset / Tool / Blog / Lecture / Benchmark / Workflow
- Keywords: keyword1, keyword2, keyword3
- One-line summary: 자료가 무엇인지 한 줄로 설명.
- Why it matters: CFD-AI / SciML 연구 관점에서 중요한 이유.
- Possible use: 연구, 논문, 실험, workflow 자동화에 어떻게 쓸 수 있는지.
- Maturity: paper-only / prototype / maintained library / production-ready / watchlist
- Priority: High / Medium / Low
```

---

## Daily digest format

Daily update는 `daily/YYYY-MM-DD.md`에 저장한다.

- 3–5개 highlights
- category별 added resources
- best find of the day
- 실제 연구로 이어질 수 있는 1–3개 아이디어

Template은 [daily/README.md](daily/README.md)를 참고한다.

---

## Curation principles

- README는 dashboard로 유지하고, 자세한 내용은 `resources/*.md`에 둔다.
- 적게 추가하되 더 좋은 자료를 추가한다.
- code 부재, 낮은 maturity, 부족한 문서화, abandoned repository 여부를 솔직하게 표시한다.
- 요약은 짧지만 구체적으로 쓴다.
- 기본은 영어로 작성하되, 개인 연구 insight는 한국어로 남겨도 된다.

---

<div align="center">

**VortexyAether**를 위해 **VA_claw**가 🦞 집게로 관리합니다.

</div>
