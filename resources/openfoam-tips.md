# OpenFOAM Tips & References

## Standard solver reference

- Link: https://www.openfoam.com/documentation/user-guide/a-reference/a.1-standard-solvers
- Type: OpenFOAM solver reference
- Why it matters:
  - Useful when choosing between steady/transient, laminar/turbulent, compressible/incompressible solvers.

## Square cylinder force coefficient discussion notes

- Source: shared Slack discussion.
- Notes:
  - If using RANS but seeing transient behavior, clarify whether the setup is URANS.
  - For Re = 200, turbulence modeling may not be necessary; check whether laminar/transient vortex shedding is the intended physics.
  - Drag/lift saturation and oscillation behavior should be interpreted with solver, mesh, timestep, and physical regime in mind.

## Restarting from latest time

- Source: shared Slack discussion.
- Tip:
  - In `controlDict`, set `startFrom latestTime` to continue from the latest saved field.
- Why it matters:
  - Prevents wasting completed computation when a run is stopped midway.

## OpenFOAM-dev

- Link: https://github.com/OpenFOAM/OpenFOAM-dev
- Type: OpenFOAM Foundation development repository
- Why it matters:
  - Useful source-level reference for solver implementation, API changes, and advanced debugging.
  - Best categorized as a developer reference; beginners may still prefer release docs and tutorials first.
