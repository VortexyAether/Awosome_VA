# Neural Operators & Tensor Methods

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

## JetSCI

- Link: https://arxiv.org/abs/2604.22087
- Type: Hybrid JAX-PETSc framework for scalable differentiable simulation
- Why it matters:
  - Connects JAX autodiff workflows with PETSc-scale solvers, a practical bridge for SciML beyond toy PDEs.
  - Relevant to inverse problems, surrogate training loops, and data-driven constitutive models that still need HPC-grade simulation infrastructure.
  - Worth tracking for CFD/heat-transfer groups that want differentiability without abandoning established solver ecosystems.

## MENO: MeanFlow-Enhanced Neural Operators

- Link: https://arxiv.org/abs/2604.06881
- Type: Neural operator architecture for dynamical systems
- Why it matters:
  - Targets the loss of high-frequency/small-scale content in Fourier-style neural operators.
  - Directly relevant to turbulent-flow surrogates, long-rollout stability, and reduced-order CFD modeling.
  - Good candidate for comparison against FNO-style baselines on unsteady flow datasets.

## SIMR-NO

- Link: https://arxiv.org/abs/2603.28073
- Type: Spectrally informed multi-resolution neural operator for turbulent-flow super-resolution
- Why it matters:
  - Focuses on reconstructing high-resolution turbulent fields from under-resolved observations.
  - Useful for LES/DNS data compression, sensor-to-field reconstruction, and CFD post-processing acceleration.
  - Spectral constraints make it more relevant than generic image super-resolution for fluid data.

## Predictivity and Utility of Neural Surrogates of Multiscale PDEs

- Link: https://arxiv.org/abs/2604.20061
- Type: Position/analysis paper on neural PDE surrogates
- Why it matters:
  - Pushes against overclaiming “universal emulator” results for multiscale PDEs.
  - Useful as a sanity-check citation when evaluating neural-operator CFD papers and benchmark claims.
  - Helps frame when surrogates are actually useful versus when they only exploit low-dimensional benchmark structure.


## Hybrid Fourier Neural Operator-Lattice Boltzmann Method

- Link: https://arxiv.org/abs/2604.27158
- Type: Hybrid neural-operator / Lattice Boltzmann CFD acceleration
- Why it matters:
  - Uses FNO initialization and rollout coupling to accelerate LBM for steady and unsteady weakly compressible flows.
  - Reports large convergence-speed gains while preserving final steady-state accuracy, making it more practical than a pure black-box surrogate.
  - Useful pattern for lab CFD: ML as an accelerator inside a trusted solver loop rather than a full solver replacement.

## LESnets for wall-bounded turbulence

- Link: https://arxiv.org/abs/2604.26621
- Type: Physics-informed neural operator for LES-style turbulence prediction
- Why it matters:
  - Targets 3D wall-bounded turbulent flows where limited data, multiscale vortices, and long-rollout stability are hard.
  - Integrates large-eddy-simulation ideas into a physics-informed neural-operator framework.
  - Good candidate for comparison when evaluating neural operators on high-Reynolds-number wall turbulence, not just toy PDEs.

## DeepPropNet

- Link: https://arxiv.org/abs/2604.27298
- Type: Operator-learning predictor for thermal plasma properties
- Why it matters:
  - Learns mappings from operating conditions to thermodynamic and transport properties that are expensive to evaluate repeatedly.
  - Directly relevant to thermal/heat-transfer adjacent simulation loops where material/property calls dominate runtime.
  - The single-property and mixture-of-experts variants are useful references for property-surrogate design.

## GeoFunFlow-3D

- Link: https://arxiv.org/abs/2604.23350
- Type: Physics-guided generative flow matching for 3D aerodynamic inference
- Why it matters:
  - Focuses on high-fidelity aerodynamic fields over complex geometries, with explicit attention to physical consistency and high-frequency features.
  - Combines flow matching, topology-aware spatial modeling, and a high-order discrete engine to reduce physics-gradient issues.
  - Relevant to CAD-to-CFD surrogate workflows where geometry complexity matters as much as field prediction accuracy.

## AI models of unstable flow exhibit hallucination

- Link: https://arxiv.org/abs/2604.20372
- Type: Reliability analysis for AI fluid-dynamics models
- Why it matters:
  - Shows visually plausible but physically impossible predictions in unstable viscous-fingering flows.
  - Useful cautionary citation for CFD-ML papers: field realism is not enough if conservation laws and instability physics fail.
  - Reinforces the need for physics checks, rollout diagnostics, and solver-in-the-loop validation.

## Faster by Design

- Link: https://arxiv.org/abs/2604.18491
- Type: Expert-validated CFD dataset and neural surrogate for interactive aerodynamics
- Why it matters:
  - Uses a parametric LMP2-class CAD model and expert-validated RANS data instead of overly smooth public car datasets.
  - Directly connects CAD complexity, CFD validation, and neural surrogates for fast aerodynamic design iteration.
  - Strong weekly-synthesis candidate for “engineering-grade datasets are the bottleneck for useful CFD surrogates.”

## Fourier Neural Operator for Parametric Partial Differential Equations

- Link: https://arxiv.org/abs/2010.08895
- Code: https://github.com/neuraloperator/neuraloperator
- Type: Paper / neural operator
- Keywords: Fourier neural operator, operator learning, PDE surrogate, spectral methods
- One-line summary: Introduces Fourier Neural Operators for learning mappings between function spaces in parametric PDE problems.
- Why it matters: FNO is one of the core baselines for neural-operator CFD/SciML work, especially for grid-based PDE surrogate modeling and spectral field learning.
- Possible use: Use as a baseline method when comparing neural operators for flow prediction, super-resolution, or parameter-to-field surrogate modeling.
- Maturity: maintained library
- Priority: High

## DeepONet: Learning nonlinear operators via the universal approximation theorem of operators

- Link: https://www.nature.com/articles/s42256-021-00302-5
- Code: https://github.com/lululxvi/deeponet
- Type: Paper / neural operator
- Keywords: DeepONet, operator learning, Scientific Machine Learning, PDE surrogate
- One-line summary: Introduces DeepONet as a neural-network architecture for learning nonlinear operators between function spaces.
- Why it matters: DeepONet is a foundational operator-learning architecture and an important comparison point against FNO-style methods.
- Possible use: Use in literature reviews to explain the operator-learning family and compare branch/trunk operator models against spectral neural operators.
- Maturity: prototype
- Priority: High

## Learning Mesh-Based Simulation with Graph Networks

- Link: https://arxiv.org/abs/2010.03409
- Code: https://github.com/google-deepmind/deepmind-research/tree/master/meshgraphnets
- Type: Paper / graph neural simulation
- Keywords: MeshGraphNets, graph neural networks, unstructured mesh, learned simulation
- One-line summary: Learns simulation dynamics directly on mesh-based physical systems using graph networks.
- Why it matters: Many engineering CFD/CAE problems live on irregular meshes, so MeshGraphNets is a key reference for geometry-aware and mesh-aware learned simulation.
- Possible use: Use as a conceptual baseline for CAD/mesh-to-field surrogate modeling and for thinking about learned simulators on unstructured CFD domains.
- Maturity: prototype
- Priority: High
