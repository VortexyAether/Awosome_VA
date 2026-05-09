# Turbulence & Generative Flow Models

Resources for turbulence prediction, reduced-order modeling, super-resolution, autoregressive flow prediction, learned closures, and generative modeling of physical fields.

## Turbulence Modeling in the Age of Data

- Link: https://arxiv.org/abs/1804.00183
- Type: Paper / review
- Keywords: turbulence modeling, data-driven modeling, RANS, LES, closure models
- One-line summary: A review focused on how data-driven methods interact with turbulence modeling and closure problems.
- Why it matters: Turbulence closure is one of the most important and failure-prone targets for CFD-AI, so this is a key grounding reference before proposing learned turbulence models.
- Possible use: Use to frame turbulence-surrogate work, RANS/LES closure discussions, and the limitations of purely data-driven turbulence modeling.
- Maturity: paper-only
- Priority: High

## Watchlist themes

- Turbulent-flow super-resolution and spectral consistency metrics
- Autoregressive flow-field prediction and rollout stability
- Learned RANS/LES closure models
- Generative models for physical fields
- Sensor-to-field reconstruction and sparse observation assimilation

## LESnets for wall-bounded turbulence

- Link: https://arxiv.org/abs/2604.26621
- Type: Physics-informed neural operator for LES-style wall turbulence prediction
- Why it matters:
  - Focuses on 3D wall-bounded turbulent flows where multiscale vortices and long-rollout stability are difficult for generic PINO models.
  - Brings LES intuition into neural-operator design rather than treating turbulence as only a high-dimensional image sequence.
  - Useful candidate for evaluating high-Reynolds-number surrogate claims beyond low-dimensional benchmark PDEs.
- Possible use: Track as a comparison point for wall-bounded turbulence datasets and PINO variants.
- Maturity: paper-only
- Priority: High

