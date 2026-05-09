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

## Mesh Based Simulations with Spatial and Temporal awareness

- Link: https://arxiv.org/abs/2605.01542
- Type: Mesh-based CFD surrogate / GNN-Transformer paper
- Why it matters:
  - Targets a practical bottleneck in mesh-based CFD surrogates: models need awareness of both local spatial structure and temporal rollout context.
  - ICML 2026 signal from the arXiv metadata makes it worth tracking as a higher-visibility learned-simulation direction.
  - Relevant to unstructured CFD meshes where naive frame-to-frame predictors often lose stability or miss long-time behavior.
- Possible use: Compare against MeshGraphNets-style baselines for time-dependent CFD surrogate experiments.
- Maturity: paper-only
- Priority: High

## ALE-Consistent Graph Neural Operator-Transformer for FSI

- Link: https://arxiv.org/abs/2605.00937
- Type: Graph neural operator / Transformer for fluid-structure interaction
- Why it matters:
  - Uses an ALE-consistent framing for long-term FSI prediction on deforming unstructured meshes.
  - Directly relevant to engineering CFD where mesh motion and coupled structures break assumptions of fixed-grid neural operators.
  - Good candidate for tracking whether operator models can survive realistic geometry/motion coupling.
- Possible use: Reference for moving-mesh FSI surrogate modeling and CAD/CAE workflows with deforming boundaries.
- Maturity: paper-only
- Priority: High

## Droplet-LNO

- Link: https://arxiv.org/abs/2604.20993
- Type: Physics-informed Laplace neural operator for droplet spreading
- Why it matters:
  - Focuses on droplet dynamics on complex surfaces, touching microfluidics, spray cooling, inkjet printing, and wetting-driven thermal applications.
  - Laplace/operator formulation is useful to compare against Fourier-style methods when boundaries and surface complexity matter.
  - Strong thermal/heat-transfer adjacency because droplet spreading is central to cooling and phase-change workflows.
- Possible use: Track for surface-aware multiphysics surrogate modeling and spray-cooling literature review.
- Maturity: paper-only
- Priority: Medium

## Neural operator framework for stability and receptivity discovery

- Link: https://arxiv.org/abs/2604.19465
- Type: Neural operator for data-driven stability/receptivity analysis
- Why it matters:
  - Connects operator learning to stability and receptivity, not just field forecasting.
  - Relevant for flow-control and sensitivity-analysis workflows where engineers care about perturbation growth and dominant response modes.
  - Useful bridge between classical resolvent/stability analysis and data-driven surrogates when equations or linearizations are unavailable.
- Possible use: Watch as a possible method for control-oriented CFD-AI projects.
- Maturity: paper-only
- Priority: High

## ZNO: Stable Rational Neural Operators in the Z-Domain

- Link: https://arxiv.org/abs/2605.02356
- Type: Stable rational neural operator for discrete-time dynamics
- Why it matters:
  - Targets discrete-time system-identification and control settings where many continuous-time neural-operator assumptions are awkward.
  - Enforces stability through unit-disk pole constraints and gives interpretable learned poles for long-memory dynamics.
  - Relevant to control-oriented CFD/thermal surrogates, especially when the learned model must remain stable over many steps.
- Possible use: Compare against state-space models and neural operators for long-horizon sensor-to-state forecasting tasks.
- Maturity: paper-only
- Priority: High

## Horizon-agnostic neural operator safety filter

- Link: https://arxiv.org/abs/2605.01069
- Type: Neural operator + control barrier function for safe deformable/fluid manipulation
- Why it matters:
  - Learns boundary input-output PDE dynamics while enforcing explicit task-level safety constraints online.
  - Combines a horizon-agnostic neural operator with a lightweight QP safety filter, making it closer to deployable control than reward-shaped policies.
  - Conceptually relevant to CFD/thermal design campaigns where exploration must avoid unsafe or invalid states.
- Possible use: Use as a reference for safe control layers around learned PDE surrogates.
- Maturity: paper-only
- Priority: Medium

## Physical Fidelity Reconstruction via Consistency-Distilled Flow Matching

- Link: https://arxiv.org/abs/2605.05975
- Type: One-step generative flow reconstruction / consistency distillation
- Why it matters:
  - Distills an optimal-transport flow-matching teacher into a compact one-step model for coarse-to-fine flow reconstruction.
  - Directly targets latency-sensitive workflows such as real-time visualization, ensemble forecasting, and simulation-in-the-loop inference.
  - Evaluated on Smoke Buoyancy, Turbulent Channel Flow, and Kolmogorov Flow, making it more CFD-relevant than generic image diffusion work.
- Possible use: Test as a post-processing accelerator for low-resolution CFD fields or sensor/coarse-grid-to-field reconstruction.
- Maturity: paper-only
- Priority: High

## Do Neural Operators Forget Geometry?

- Link: https://arxiv.org/abs/2605.05862
- Type: Reliability / geometry-awareness analysis for neural operators
- Why it matters:
  - Formalizes “geometric forgetting”: deep operator layers can progressively lose domain-geometry information.
  - Highly relevant to irregular geometry, CAD-to-CFD surrogates, and mesh-aware operator learning where geometry cannot be treated as one-time context.
  - Proposes lightweight geometry memory injection and suggests a practical validation probe for neural-operator architectures.
- Possible use: Add geometry-retention diagnostics when comparing FNO/attention/operator models on CAD or unstructured-mesh CFD data.
- Maturity: paper-only
- Priority: High

## AeroJEPA

- Link: https://arxiv.org/abs/2605.05586
- Type: JEPA-style aerodynamic field surrogate
- Why it matters:
  - Predicts semantic latent representations of 3D aerodynamic fields from geometry and operating-condition context instead of directly predicting huge full-resolution fields.
  - Targets realistic large-field regimes through HiLiftAeroML and broad transonic-wing generalization through SuperWing.
  - Useful direction for design optimization because the latent space is meant to support analysis and optimization, not only reconstruction.
- Possible use: Track as a candidate architecture pattern for scalable 3D aerodynamic design loops.
- Maturity: paper-only
- Priority: High

## MeLISA: One-Step Generative Modeling for Dynamical Forecasting

- Link: https://arxiv.org/abs/2605.05540
- Type: One-step generative surrogate for autoregressive dynamical systems
- Why it matters:
  - Addresses the gap between cheap but drifting neural-operator rollouts and expensive multi-step diffusion/generative surrogates.
  - Uses pixel-space MeanFlow with consistency losses to preserve long-trajectory statistics in turbulent regimes.
  - Relevant to unsteady CFD surrogate modeling where long-horizon statistical fidelity matters more than a single-step RMSE.
- Possible use: Compare against FNO/MENO-style baselines on turbulent-flow rollout benchmarks.
- Maturity: paper-only
- Priority: Medium

## Context Flux Neural Operator

- Link: https://arxiv.org/abs/2605.05488
- Code: https://github.com/xx257xx/CONTEXT_FLUX_NO
- Type: Context-conditioned flux neural operator for conservation laws
- Why it matters:
  - Combines finite-volume-inspired Flux NO with recurrent ViT context injection to infer solution dynamics across conservation-law families.
  - Preserves the solver-assist flavor of flux/operator methods while reducing reliance on explicitly supplied PDE coefficients.
  - Interesting foundation-model direction for conservative systems where robustness and long-time prediction are critical.
- Possible use: Use as a baseline/reference for conservation-law surrogate experiments and solver-in-the-loop SciML designs.
- Maturity: paper + code
- Priority: High

## RETO: Rotary-Enhanced Transformer Operator for automotive aerodynamics

- Link: https://arxiv.org/abs/2605.00062
- Type: Transformer neural operator for aerodynamic field prediction
- Why it matters:
  - Targets high-fidelity automotive aerodynamics on ShapeNet and DrivAerML-like settings.
  - Uses global sinusoidal-cosine references plus RoPE-style relative spatial encoding to improve local gradient and displacement awareness.
  - Relevant to CAD/geometry-conditioned CFD surrogates where spatial correlations matter more than generic image-like field prediction.
- Possible use: Compare against Transolver/FNO/GNO baselines on automotive or external-aero surrogate tasks.
- Maturity: paper-only
- Priority: High

## Real-time HR flow-field estimation from event-based imaging velocimetry

- Link: https://arxiv.org/abs/2605.04186
- Type: Sensor-to-field reconstruction / ROM estimation
- Why it matters:
  - Converts low-resolution real-time EBIV snapshots into high-resolution velocity fields and POD coordinates.
  - Combines LR-to-HR mapping with temporal regularization/Kalman-style estimators, making it relevant to closed-loop flow-control workflows.
  - Good bridge between experimental fluid sensing, reduced-order modeling, and real-time digital twins.
- Possible use: Prototype sparse/coarse measurement → POD-coordinate estimation for a controlled CFD dataset.
- Maturity: paper-only
- Priority: Medium

## Constrained Extreme Gradient Boosting for adapting ROMs

- Link: https://arxiv.org/abs/2605.04130
- Type: Adaptive reduced-order modeling method
- Why it matters:
  - Addresses ROM degradation under parameter variation using a constrained ensemble-learning correction layer.
  - Potentially easier to integrate into parametric CFD/FEA optimization loops than a large end-to-end neural surrogate.
  - Useful reference for lightweight ROM adaptation when simulation data at every operating condition is unavailable.
- Possible use: Test as a basis-adaptation baseline for parametric thermal or fluid surrogate studies.
- Maturity: paper-only
- Priority: Medium

## Control-oriented cluster-based reduced-order modelling

- Link: https://arxiv.org/abs/2604.25474
- Type: Control-oriented reduced-order model
- Why it matters:
  - Generalizes cluster network model transition probabilities and times across unseen control parameters.
  - Directly targets reduced dynamics for operating regimes where no simulation data is available.
  - Relevant to flow-control and aeroelastic-control studies where surrogate behavior under new controls matters.
- Possible use: Compare against POD/DMD-style control surrogates on a simple separated-flow or oscillator dataset.
- Maturity: paper-only
- Priority: Medium

