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
