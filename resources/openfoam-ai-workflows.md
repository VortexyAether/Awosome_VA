# OpenFOAM AI Workflows

AI-assisted OpenFOAM setup, automation, case validation, post-processing, and engineering workflow orchestration.

## OpenFOAM MCP Server

- Link: https://github.com/webworn/openfoam-mcp-server
- Type: Tool / MCP server
- Keywords: OpenFOAM, MCP, CFD education, error resolution, LLM agents
- One-line summary: An LLM-powered MCP server for OpenFOAM that focuses on CFD education, Socratic questioning, and expert-style error resolution.
- Why it matters: OpenFOAM has a steep setup/debugging curve; an MCP layer can expose solver diagnostics and case reasoning to AI assistants without relying on brittle terminal-only prompting.
- Possible use: Evaluate as a reference for agent-assisted OpenFOAM case setup, log diagnosis, educational tutoring, and future CAD→CFD workflow automation.
- Maturity: prototype
- Priority: High

## MetaOpenFOAM: an LLM-based multi-agent framework for CFD

- Link: https://arxiv.org/abs/2407.21320
- Code: https://github.com/Terry-cyx/MetaOpenFOAM
- Type: Paper / engineering AI agent workflow
- Keywords: OpenFOAM, LLM agents, multi-agent framework, CFD automation
- One-line summary: Proposes a multi-agent LLM framework for automating parts of OpenFOAM-based CFD workflows.
- Why it matters: Directly relevant to agentic CFD workflow automation, especially case setup, execution, debugging, and post-processing around existing solvers.
- Possible use: Use as a reference when designing CAD→CFD→visualization orchestration agents or comparing MCP-based OpenFOAM automation approaches.
- Maturity: prototype
- Priority: High

## AI CFD Scientist

- Link: https://arxiv.org/abs/2605.06607
- Code: https://github.com/csml-rpi/AI-CFD-Scientist
- Type: Agentic CFD research pipeline / OpenFOAM workflow
- Why it matters:
  - Connects literature-grounded ideation, OpenFOAM execution, mesh-independence checks, diagnostic interpretation, source-code modification, figure generation, and LaTeX drafting in one inspectable workflow.
  - The repository exposes both a LangGraph orchestrator and skill-driven artifact contracts such as `lit.json`, `requirements.json`, `selected_mesh_spec.json`, and `analysis.json`.
  - Useful reference for VA-style intelligent engineering workflows because it treats solver artifacts and physics checks as first-class outputs, not just chat responses.
- Possible use: Compare its artifact schema and mesh/diagnostic gates against sim-benchmark/FoamPilot when designing a safer OpenFOAM agent harness.
- Maturity: early open-source research prototype
- Priority: High
