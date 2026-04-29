# Awosome_VA

[![SciML](https://img.shields.io/badge/SciML-CFD-blue)](#sciml--cfd)
[![AI Agents](https://img.shields.io/badge/AI%20Agents-생산성-purple)](#ai-agent--생산성)
[![Graduate Workflow](https://img.shields.io/badge/대학원생-Workflow-green)](#대학원생-연구-워크플로우)
[![English README](https://img.shields.io/badge/README-English-red)](README.md)

> **SciML & CFD 연구**, **대학원생 연구 워크플로우**, **AI 생산성 도구**를 위한 큐레이션 저장소.

이 저장소는 논문, 도구, GitHub 저장소, 워크플로우, 기술 노트를 가볍게 정리하는 지식 베이스입니다. 시작은 CFD × Scientific Machine Learning 자료였지만, 연구 글쓰기, 랩 생산성, AI coding agent, 문서 도구, 운영/보안 팁까지 함께 정리합니다.

## 목차

- [큰 그림](#큰-그림)
- [SciML & CFD](#sciml--cfd)
- [대학원생 연구 워크플로우](#대학원생-연구-워크플로우)
- [AI agent & 생산성](#ai-agent--생산성)
- [문서/행정/운영](#문서행정운영)
- [현재 하이라이트](#현재-하이라이트)
- [추천 워크플로우](#추천-워크플로우)
- [큐레이션 원칙](#큐레이션-원칙)

## 큰 그림

| 대분류 | 포함되는 것 | 시작점 |
|---|---|---|
| **SciML & CFD** | CFD solver, AMR, OpenFOAM, meshing, JAX prototype, neural operator, optimizer, visualization | [SciML & CFD](#sciml--cfd) |
| **대학원생 연구 워크플로우** | 논문 작성, 연구 자동화, 발표/보고서 구조, 세미나, 학술/산업 기회 | [대학원생 연구 워크플로우](#대학원생-연구-워크플로우) |
| **AI agent & 생산성 도구** | Claude/Codex/OpenCode, local LLM, skill/harness, voice-to-prompt, Google/agent tooling | [AI agent & 생산성](#ai-agent--생산성) |
| **문서/행정/운영** | HWP 도구, 행사, cloud cost/security, 기타 유틸리티 | [문서/행정/운영](#문서행정운영) |

## SciML & CFD

| 분야 | 먼저 볼 문서 | 대표 자료 | 이런 때 유용함 |
|---|---|---|---|
| **Differentiable CFD / AMR** | [Differentiable CFD & AMR solvers](resources/differentiable-cfd-amr.md) | JAX-AMR, JANC, geometry-autoencoder PINN | JAX 기반 CFD, AMR, differentiable solver, geometry-varying PINN을 공부하거나 구현할 때 |
| **Meshing / HPC CFD** | [Meshing & GPU workflows](resources/meshing-gpu-workflows.md) · [GPU OpenFOAM](resources/gpu-openfoam-hpc.md) | PhysicsNeMo-Mesh, SALOME/Gmsh/Pointwise, OpenFOAM GPU acceleration | geometry/mesh 생성과 GPU CFD 워크플로우를 연결하고 싶을 때 |
| **OpenFOAM 실무** | [OpenFOAM tips](resources/openfoam-tips.md) | solver reference, square-cylinder notes, `startFrom latestTime` | solver 선택, 계산 재시작, OpenFOAM 기본 동작을 정리할 때 |
| **JAX CFD 프로토타입** | [JAX-based CFD prototypes](resources/jax-cfd-prototypes.md) | IBM airfoil flap, GUI prototype, wind turbine toy model | JAX/agent로 빠르게 유동 시뮬레이션 프로토타입을 만들 때 |
| **시각화** | [Visualization & post-processing](resources/visualization-postprocessing.md) · [Weather/climate visualization](resources/weather-climate-visualization.md) | Omniverse Q-criterion, Earth2Studio, black-hole simulation visualization | simulation/ML field output을 해석 가능한 그림으로 만들 때 |
| **CAD / geometry AI** | [CAD, geometry & AI-assisted design](resources/cad-geometry-ai.md) | ForgeCAD, FreeCAD + Claude Code | CFD/CAE geometry를 coding agent로 생성하거나 반복 수정할 때 |
| **Neural operator / architecture** | [Neural operators & tensor methods](resources/neural-operators-tensor-methods.md) · [Optimization for SciML](resources/optimization-sciml.md) | Tensor train, Mamba-3, SpecMuon, Attention Residuals | SciML용 모델 구조, optimizer, compression 아이디어를 추적할 때 |
| **Fluid/AI 교육** | [Fluid mechanics, turbulence & AI education](resources/education-fluid-ai.md) | VinuesaLab | fluid mechanics, turbulence, interpretable ML, AI-for-science 관점을 공부할 때 |
| **수학적 기반** | [Mathematical foundations](resources/math-foundations.md) | function representation notes | 이론적이지만 잠재적으로 관련 있는 수학 아이디어를 보관할 때 |

## 대학원생 연구 워크플로우

| 분야 | 먼저 볼 문서 | 대표 자료 | 이런 때 유용함 |
|---|---|---|---|
| **연구 자동화 / 글쓰기** | [Research automation & writing](resources/research-automation-writing.md) | PaperOrchestra, PaperBanana, Feynman, Overleaf MCP, AI Scientist | literature review, 논문 초안, figure 생성, citation 검증을 자동화하고 싶을 때 |
| **발표 / 보고서 구조** | [Research presentation & report structure](resources/research-presentation-workflow.md) | scenario → metric → data → learning → analysis → application workflow | 랩세미나 발표, 기술 보고서, 연구 스토리라인을 구조화할 때 |
| **행사 / 기회** | [Events & opportunities](resources/events-opportunities.md) | SEMICON, 산업계/커리어 신호 | 시간 민감한 학술/산업 기회를 기록할 때 |

## AI agent & 생산성

| 분야 | 먼저 볼 문서 | 대표 자료 | 이런 때 유용함 |
|---|---|---|---|
| **Agent 도구** | [Agent tools & research workflow](resources/agent-tools-workflow.md) | Claude Code tips, Codex/OpenCode, Google Workspace CLI, skills/harnesses | coding agent를 연구/소프트웨어 작업에 잘 쓰고 싶을 때 |
| **연구실 AI 도입** | [AI coding & lab adoption](resources/ai-coding-lab-adoption.md) | 공용 Claude/API 전략, 랩세미나 아이디어, Codex 지원 프로그램 | 연구실 단위 AI 사용 전략과 온보딩을 설계할 때 |
| **Local AI workflow** | [Local AI research workflow](resources/local-ai-workflow.md) | whatcani.run, Gemma/local LLMs | 개인/로컬 AI workflow를 만들고 local model 가능성을 볼 때 |

## 문서/행정/운영

| 분야 | 먼저 볼 문서 | 대표 자료 | 이런 때 유용함 |
|---|---|---|---|
| **문서/행정 도구** | [Miscellaneous tools](resources/misc-tools.md) | HOP Open HWP, image/video AI notes | HWP 등 한국 문서 업무와 주변 유틸리티를 정리할 때 |
| **보안 / 비용 / 운영** | [Security, cost & operations](resources/security-cost-ops.md) | AWS billing incident, secret/cost reminders | cloud, agent, credential 사용 중 비싼 실수를 피하고 싶을 때 |

## 현재 하이라이트

- **JAX-AMR / JANC** — accelerator-friendly AMR 및 differentiable CFD solver 참고 자료.
- **PhysicsNeMo-Mesh + OpenFOAM GPU acceleration** — 더 빠른 CFD pipeline을 위한 두 방향: GPU-native mesh/ML 도구와 기존 solver 가속.
- **JAX CFD prototypes** — airfoil flap, wind turbine, GUI-style simulation workflow 등 빠른 CFD-ML 프로토타이핑 가능성.
- **ForgeCAD / FreeCAD + Claude Code** — 초기 CFD/CAE design loop에서 agent-assisted geometry generation의 가능성.
- **PaperOrchestra / Feynman / PaperBanana** — multi-agent 기반 논문 작성, 리뷰, figure 생성, source verification 흐름.

## 추천 워크플로우

### CFD-ML 프로토타입 만들기

1. [JAX-based CFD prototypes](resources/jax-cfd-prototypes.md)부터 본다.
2. solver/AMR 아이디어는 [Differentiable CFD & AMR solvers](resources/differentiable-cfd-amr.md)에서 확인한다.
3. geometry/mesh는 [CAD/geometry AI](resources/cad-geometry-ai.md) 또는 [Meshing & GPU workflows](resources/meshing-gpu-workflows.md)를 참고한다.
4. 결과는 [Visualization & post-processing](resources/visualization-postprocessing.md) 흐름으로 시각화한다.

### 논문/보고서 준비하기

1. [Research presentation & report structure](resources/research-presentation-workflow.md)로 이야기 구조를 잡는다.
2. [Research automation & writing](resources/research-automation-writing.md)로 자료 수집, 초안 작성, figure 생성을 보조한다.
3. coding-agent 사용법은 [Agent tools & research workflow](resources/agent-tools-workflow.md)를 참고한다.
4. 주장, citation, figure, 수치 검증은 반드시 사람이 확인한다.

### 연구실 AI 사용 체계 잡기

1. [AI coding & lab adoption](resources/ai-coding-lab-adoption.md)에서 시작한다.
2. [Agent tools](resources/agent-tools-workflow.md)와 [Local AI workflow](resources/local-ai-workflow.md)를 비교한다.
3. agent에게 credential/cloud access를 주기 전에 [Security, cost & operations](resources/security-cost-ops.md)를 확인한다.

## 큐레이션 원칙

- SciML/CFD 연구, 대학원생 연구 워크플로우, AI 생산성, 연구실 운영에 유용한 자료를 우선한다.
- 과제, 사적인 연구실 운영 대화, 일시적인 Slack 잡담은 재사용 가능한 자료가 있을 때만 포함한다.
- 각 entry는 짧게 유지한다: 링크, 왜 중요한지, 어디에 쓸 수 있는지.
- 자세한 내용은 `resources/*.md`에 두고, README는 한눈에 보는 대시보드로 유지한다.

## Maintainer note

VA_claw가 공유된 링크, 논문, 저장소, 노트를 바탕으로 이 저장소를 계속 업데이트할 수 있습니다.
