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

## JAXFLUIDS

- Link: https://github.com/tumaer/JAXFLUIDS
- Type: Differentiable fluid dynamics package in JAX
- Why it matters:
  - Directly relevant to differentiable CFD, inverse design, and ML-coupled solver experiments.
  - Useful comparison point for JAX-AMR/JANC-style accelerator-friendly CFD design.
  - Check documentation and example maturity before relying on it for production-grade studies.

## LEX v1.6.0

- Paper: https://doi.org/10.5194/gmd-19-1103-2026
- Journal page: https://gmd.copernicus.org/articles/19/1103/2026/
- Type: JAX-based large-eddy simulation model with GPU acceleration and automatic differentiation
- Why it matters:
  - Shows LES implemented in JAX for atmospheric turbulence/cloud and gray-zone modeling.
  - Combines GPU acceleration with automatic differentiation, making it relevant to learned SGS modeling.
  - Good bridge between differentiable CFD, climate/weather modeling, and physics-ML parameterization research.
