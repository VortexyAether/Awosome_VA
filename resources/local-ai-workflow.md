# Local AI Research Workflow

## whatcani.run

- Link: https://www.whatcani.run/
- Type: Local LLM capability checker
- Why it matters:
  - Helps estimate which local models can run on a given machine.
  - Useful for planning local AI assistant workflows without relying entirely on cloud APIs.

## Google DeepMind Gemma 4

- Link: https://deepmind.google/models/gemma/gemma-4/
- Type: Open model family
- Why it matters:
  - Small/efficient local LLMs can be useful for private research assistance, document triage, and lightweight coding support.
  - Apple Silicon machines can be attractive for local inference because unified memory is shared between CPU/GPU.
- Possible use:
  - Local LLM + OpenClaw setup for private research assistant workflows.
  - Offline or low-cost summarization/classification of papers, notes, and repository contents.

## Ollama

- Link: https://github.com/ollama/ollama
- Type: Local LLM runtime
- Why it matters:
  - Representative tool for running local models on a workstation or Mac mini.
  - Useful for private, low-latency summarization, document triage, and lightweight assistant workflows.
  - Model quality and memory limits depend strongly on hardware and quantization.

## llama.cpp

- Link: https://github.com/ggml-org/llama.cpp
- Type: C/C++ LLM inference engine
- Why it matters:
  - Foundational local/edge LLM inference project.
  - Useful for understanding quantization, CPU/GPU inference tradeoffs, and deployment below full cloud stacks.
