<div align="center">

# 🌊 Awosome_VA

### **SciML · CFD · AI-assisted research workflow** 큐레이션 저장소

[![SciML](https://img.shields.io/badge/SciML-CFD-2563eb?style=for-the-badge)](#-sciml--cfd)
[![Agents](https://img.shields.io/badge/AI%20Agents-생산성-7c3aed?style=for-the-badge)](#-ai-agent--생산성)
[![Graduate](https://img.shields.io/badge/대학원생-Workflow-16a34a?style=for-the-badge)](#-대학원생-연구-워크플로우)
[![English](https://img.shields.io/badge/README-English-dc2626?style=for-the-badge)](README.md)

*CFD-ML 연구와 대학원생 생산성에 유용한 논문, 도구, 저장소, 워크플로우, 기술 노트 모음.*

</div>

---

## 🧭 빠른 이동

| 🚀 대분류 | 포함되는 것 | 바로가기 |
|---|---|---|
| **SciML & CFD** | CFD solver, AMR, OpenFOAM, meshing, JAX prototype, neural operator, visualization | [이동](#-sciml--cfd) |
| **대학원생 연구 워크플로우** | 논문 작성, 연구 자동화, 발표/보고서 구조, 학술/산업 기회 | [이동](#-대학원생-연구-워크플로우) |
| **AI agent & 생산성** | Claude/Codex/OpenCode, local LLM, skill/harness, agent-friendly tooling | [이동](#-ai-agent--생산성) |
| **문서/행정/운영** | HWP 도구, 행사, cloud cost/security, 기타 유틸리티 | [이동](#-문서행정운영) |

---

## 🔬 SciML & CFD

| 분야 | 먼저 볼 문서 | 대표 자료 |
|---|---|---|
| 🧪 **Differentiable CFD / AMR** | [Differentiable CFD & AMR solvers](resources/differentiable-cfd-amr.md) | JAX-AMR, JANC, geometry-autoencoder PINN |
| 🧱 **Meshing / HPC CFD** | [Meshing & GPU workflows](resources/meshing-gpu-workflows.md) · [GPU OpenFOAM](resources/gpu-openfoam-hpc.md) | PhysicsNeMo-Mesh, SALOME/Gmsh/Pointwise, OpenFOAM GPU acceleration |
| 🌪️ **OpenFOAM 실무** | [OpenFOAM tips](resources/openfoam-tips.md) | solver reference, square-cylinder notes, `startFrom latestTime` |
| ⚡ **JAX CFD 프로토타입** | [JAX-based CFD prototypes](resources/jax-cfd-prototypes.md) | IBM airfoil flap, GUI prototype, wind turbine toy model |
| 🎞️ **시각화** | [Visualization & post-processing](resources/visualization-postprocessing.md) · [Weather/climate visualization](resources/weather-climate-visualization.md) | Omniverse Q-criterion, Earth2Studio, black-hole simulation visualization |
| 🧩 **CAD / geometry AI** | [CAD, geometry & AI-assisted design](resources/cad-geometry-ai.md) | ForgeCAD, FreeCAD + Claude Code |
| 🧠 **Neural operator / architecture** | [Neural operators & tensor methods](resources/neural-operators-tensor-methods.md) · [Optimization for SciML](resources/optimization-sciml.md) | Tensor train, Mamba-3, SpecMuon, Attention Residuals |
| 🎓 **Fluid/AI 교육** | [Fluid mechanics, turbulence & AI education](resources/education-fluid-ai.md) | VinuesaLab |
| ∑ **수학적 기반** | [Mathematical foundations](resources/math-foundations.md) | function representation notes |

---

## 🧑‍🎓 대학원생 연구 워크플로우

| 분야 | 먼저 볼 문서 | 대표 자료 |
|---|---|---|
| ✍️ **연구 자동화 / 글쓰기** | [Research automation & writing](resources/research-automation-writing.md) | PaperOrchestra, PaperBanana, Feynman, Overleaf MCP, AI Scientist |
| 🗂️ **발표 / 보고서 구조** | [Research presentation & report structure](resources/research-presentation-workflow.md) | scenario → metric → data → learning → analysis → application workflow |
| 📌 **행사 / 기회** | [Events & opportunities](resources/events-opportunities.md) | SEMICON, 산업계/커리어 신호 |

---

## 🤖 AI agent & 생산성

| 분야 | 먼저 볼 문서 | 대표 자료 |
|---|---|---|
| 🛠️ **Agent 도구** | [Agent tools & research workflow](resources/agent-tools-workflow.md) | Claude Code tips, Codex/OpenCode, Google Workspace CLI, skills/harnesses, 500+ AI agent use cases |
| 🏫 **연구실 AI 도입** | [AI coding & lab adoption](resources/ai-coding-lab-adoption.md) | 공용 Claude/API 전략, 랩세미나 아이디어, Codex 지원 프로그램 |
| 💻 **Local AI workflow** | [Local AI research workflow](resources/local-ai-workflow.md) | whatcani.run, Gemma/local LLMs |

---

## 📄 문서/행정/운영

| 분야 | 먼저 볼 문서 | 대표 자료 |
|---|---|---|
| 📝 **문서/행정 도구** | [Miscellaneous tools](resources/misc-tools.md) | HOP Open HWP, image/video AI notes |
| 🔐 **보안 / 비용 / 운영** | [Security, cost & operations](resources/security-cost-ops.md) | AWS billing incident, secret/cost reminders |

---

## ✨ 현재 하이라이트

- **JAX-AMR / JANC** — accelerator-friendly AMR 및 differentiable CFD solver 참고 자료.
- **PhysicsNeMo-Mesh + OpenFOAM GPU acceleration** — GPU-native mesh/ML 도구와 기존 solver 가속이라는 두 방향.
- **JAX CFD prototypes** — airfoil flap, wind turbine, GUI-style simulation workflow 등 빠른 CFD-ML 프로토타이핑 가능성.
- **ForgeCAD / FreeCAD + Claude Code** — 초기 CFD/CAE design loop에서 agent-assisted geometry generation의 가능성.
- **PaperOrchestra / Feynman / PaperBanana** — multi-agent 기반 논문 작성, 리뷰, figure 생성, source verification 흐름.

---

## 🧪 추천 워크플로우

<details>
<summary><b>CFD-ML 프로토타입 만들기</b></summary>

1. [JAX-based CFD prototypes](resources/jax-cfd-prototypes.md)부터 본다.
2. solver/AMR 아이디어는 [Differentiable CFD & AMR solvers](resources/differentiable-cfd-amr.md)에서 확인한다.
3. geometry/mesh는 [CAD/geometry AI](resources/cad-geometry-ai.md) 또는 [Meshing & GPU workflows](resources/meshing-gpu-workflows.md)를 참고한다.
4. 결과는 [Visualization & post-processing](resources/visualization-postprocessing.md) 흐름으로 시각화한다.

</details>

<details>
<summary><b>논문/보고서 준비하기</b></summary>

1. [Research presentation & report structure](resources/research-presentation-workflow.md)로 이야기 구조를 잡는다.
2. [Research automation & writing](resources/research-automation-writing.md)로 자료 수집, 초안 작성, figure 생성을 보조한다.
3. coding-agent 사용법은 [Agent tools & research workflow](resources/agent-tools-workflow.md)를 참고한다.
4. 주장, citation, figure, 수치 검증은 반드시 사람이 확인한다.

</details>

<details>
<summary><b>연구실 AI 사용 체계 잡기</b></summary>

1. [AI coding & lab adoption](resources/ai-coding-lab-adoption.md)에서 시작한다.
2. [Agent tools](resources/agent-tools-workflow.md)와 [Local AI workflow](resources/local-ai-workflow.md)를 비교한다.
3. agent에게 credential/cloud access를 주기 전에 [Security, cost & operations](resources/security-cost-ops.md)를 확인한다.

</details>

---

## 🧹 큐레이션 원칙

- **SciML/CFD 연구**, **대학원생 연구 워크플로우**, **AI 생산성**, **연구실 운영**에 유용한 자료를 우선한다.
- 과제, 사적인 연구실 운영 대화, 일시적인 Slack 잡담은 재사용 가능한 자료가 있을 때만 포함한다.
- 각 entry는 짧게 유지한다: 링크, 왜 중요한지, 어디에 쓸 수 있는지.
- 자세한 내용은 `resources/*.md`에 두고, README는 한눈에 보는 대시보드로 유지한다.

---

<div align="center">

**VA_claw**가 🦞 집게로 관리합니다.

</div>
