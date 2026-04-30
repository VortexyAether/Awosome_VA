# Neural Operators & Tensor Methods

## Adaptive Patching for Tensor Train

- Source: shared PDF `2602.22372v2.pdf`
- Type: Tensor train / adaptive patching method
- Why it matters:
  - Tensor decompositions are relevant for high-dimensional Scientific ML, reduced-order modeling, and efficient operator representations.
  - Adaptive patching may be useful when dealing with localized structure in simulation fields.
- Follow-up:
  - Add arXiv link and summary after the PDF metadata is available.
  - Check whether the method can be connected to neural operator compression, surrogate modeling, or CFD field representation.

## Mamba-3

- Link: https://arxiv.org/abs/2603.15569
- Type: State-space / efficient sequence model
- Why it matters:
  - Mamba-style models are relevant when Transformer inference cost is too high.
  - Scientific ML may benefit from efficient long-context/state-tracking models for time-series simulation data, reduced-order modeling, or trajectory modeling.
- Note:
  - Not directly CFD-specific, but worth tracking for model architecture trends.

## NVIDIA PhysicsNeMo

- Link: https://github.com/NVIDIA/physicsnemo
- Type: Physics-ML framework
- Why it matters:
  - Industrially visible framework for physics-informed learning, neural operators, and surrogate modeling.
  - Useful reference for GPU-oriented SciML workflows and NVIDIA ecosystem integrations.
  - Installation and dependency assumptions should be checked before adopting in a lab workflow.

## neuraloperator

- Link: https://github.com/neuraloperator/neuraloperator
- Type: Neural operator library
- Why it matters:
  - Representative implementation family for Fourier Neural Operator and related operator-learning methods.
  - Useful baseline for PDE surrogate modeling and CFD-ML literature comparisons.
  - Helps keep neural-operator notes tied to a maintained implementation rather than only papers.

## PDEBench

- Link: https://github.com/pdebench/PDEBench
- Type: Scientific ML benchmark suite for PDEs
- Why it matters:
  - Provides benchmark datasets/tasks for comparing PINNs, neural operators, and PDE surrogate models.
  - Useful when deciding whether a CFD-ML method is actually improving over known baselines.
  - Keep distinct from solver resources: it is primarily benchmark/data infrastructure.
