# Differentiable CFD & AMR Solvers

## JAX-AMR

- Link: https://github.com/Ashwin3919/JAX-amR
- Tech report / test cases: https://github.com/Ashwin3919/JAX-amR/blob/main/tech-report.md
- Type: JAX-based adaptive mesh refinement / differentiable CFD tooling
- Shared feature notes:
  - Adaptive mesh refinement
  - Dimensionless computation
  - Explicit time advancing with RK3
  - High-order spatial reconstruction with WENO-5
  - Lax-Friedrichs Riemann solver
  - Point-implicit chemical source advancing
  - CPU/GPU/TPU capability
  - Parallel computation on GPU/TPU for the core solver in the current version
- Why it matters:
  - Useful reference for AMR implementations in JAX.
  - Potential building block for differentiable CFD workflows.
  - Combines high-order finite-volume ingredients with accelerator-friendly implementation choices.
  - The test cases are useful for comparing solver behavior and AMR design choices.

## JANC

- Link: https://github.com/JA4S/JANC
- Type: Differentiable compressible reacting flow solver with JAX-based AMR
- Description from shared note:
  - “A cost-effective, differentiable compressible reacting flow solver featured with JAX-based adaptive mesh refinement.”
- Why it matters:
  - Directly relevant to compressible/reacting CFD + Scientific ML.
  - Good candidate for studying JAX-based solver design and GPU-friendly AMR.
  - Potential reference for coupling CFD solvers with neural operators or inverse/design workflows.

## Geometry-autoencoder PINN for variable geometry problems

- Source: shared 2022 paper PDF (`s40323-022-00221-z.pdf`) and images.
- Type: PINN with geometry encoded through an autoencoder
- Shared context:
  - Geometry-varying PINN idea was already proposed around 2022.
  - Follow-up suggestion: inspect papers citing this work to find current SOTA for PINNs with geometric variation.
- Why it matters:
  - Important for design optimization workflows where Reynolds number, geometry, or boundary conditions vary.
  - Suggests a path: optimize under a specific application condition, then validate with CFD.
