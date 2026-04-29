# Optimization for Scientific Machine Learning

## SpecMuon: Muon with Spectral Guidance

- Link: https://arxiv.org/abs/2602.16167
- Type: Optimizer for Scientific ML
- Shared note:
  - Adapts the Muon optimizer idea for scientific computing / physics-informed learning.
  - Introduces spectral-aware guidance to handle ill-conditioned gradients, multi-scale spectral behavior, and stiffness.
- Why it matters:
  - PINNs and neural operators often fail because optimization is poorly conditioned, not because the architecture is impossible.
  - CFD applications frequently involve stiffness, multi-scale spectra, and hard physical constraints.
  - Since CFD-specific applications may still be sparse, this could be a good early exploration topic.
- Possible follow-up:
  - Test on PINN benchmarks, operator-learning problems, or differentiable CFD inverse problems.
  - Compare against AdamW, L-BFGS, Shampoo-like second-order-ish optimizers, and baseline Muon.
