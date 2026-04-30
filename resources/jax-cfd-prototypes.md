# JAX-based CFD Prototypes

## JAX immersed-boundary airfoil flap simulation

- Source: shared Slack video/note.
- Type: JAX-based immersed boundary method simulation
- Shared context:
  - Airfoil flap simulation with moving solid boundary.
  - Reported as fast even with about 4 million moving grid points.
  - Physical validation still needed.
- Why it matters:
  - Could be useful for fast prototyping of flow-control problems.
  - Potential connection to reinforcement learning for control.
  - Shows the practical appeal of JAX-based CFD for interactive experimentation.

## JAX CFD GUI prototype

- Source: shared Slack PDF/video note.
- Type: GUI layer around JAX-based simulation
- Shared context:
  - Extends previous JAX-based simulation with a GUI.
  - IBM limits strict physical fidelity, but the workflow is promising for quickly checking qualitative behavior.
- Why it matters:
  - Fast visual feedback can be very useful in early design/control exploration.
  - Good candidate for educational demos or agent-assisted parameter studies.

## Antigravity agent-coded JAX wind turbine prototype

- Source: shared Slack note.
- Type: Agent-assisted JAX simulation prototype
- Shared context:
  - Wind turbine simulation attempted with agent coding.
  - Inspired by JAX-based airfoil simulation.
  - Rotating parts were implemented at toy-problem level, despite being hard in OpenFOAM/AMI workflows.
- Why it matters:
  - Demonstrates how coding agents can lower the barrier to fast CFD prototype creation.
  - Needs physical validation and refinement, but useful for rapid ideation.

## google/jax-cfd

- Link: https://github.com/google/jax-cfd
- Type: JAX-based CFD framework / research prototype
- Why it matters:
  - Representative starting point for JAX-native CFD experiments.
  - Useful for differentiable simulation, ML-CFD prototypes, and educational solver studies.
  - Best treated as a research/prototyping framework rather than a production CFD solver.

## AeroJAX

- Link: https://github.com/arriemeijer-creator/AeroJAX
- Type: Experimental differentiable aerodynamics / JAX flow-simulation project
- Why it matters:
  - Targets real-time flow simulation, control, inverse design, and neural-operator integration.
  - Relevant to aircraft/control-oriented CFD-ML ideation.
  - Experimental and young; keep as a project to watch, not a validated solver baseline.
