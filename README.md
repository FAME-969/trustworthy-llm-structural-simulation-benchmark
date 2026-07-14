# Toward Trustworthy LLM-Assisted Structural Simulation Benchmark

This repository contains the benchmark materials associated with the paper:

**Toward Trustworthy LLM-Assisted Structural Simulation: A Reproducible Benchmark and Mechanics-Aware Failure-Mode Analysis**

## Overview

Large language models (LLMs) are increasingly used for code generation and engineering automation. In structural mechanics, however, executable code and visually plausible outputs do not necessarily imply physically correct simulation.

This repository provides a **controlled and reproducible benchmark** for evaluating LLM-assisted structural simulation from a **mechanics-aware correctness** perspective. The benchmark includes five representative problems spanning elasticity, dynamics, and frame analysis, together with reference solutions, generated implementations, execution logs, and evaluation scripts.

The goal of this repository is **not** to maintain a permanent leaderboard of commercial models. Instead, it is intended to support:

- reproducible evaluation of LLM-assisted structural simulation,
- mechanics-aware failure-mode analysis,
- development of verification modules for trustworthy LLM-assisted or agentic workflows,
- future benchmark extension and comparison.

## Benchmark Problems

The benchmark consists of the following five problems:

1. **2D elasticity panel**
2. **3D elasticity cube**
3. **Timoshenko beam forced vibration**
4. **2D plane frame**
5. **3D spatial frame**

These five problems collectively expose several mechanics-sensitive issues, including:

- boundary condition interpretation,
- traction-free / free-surface treatment,
- boundary-adjacent stencil handling,
- numerical stability,
- modeling-assumption mismatch,
- local-axis definition and transformation,
- load projection,
- constraint enforcement,
- field recovery / interpolation.

## Repository Structure

Repository structure is organized as follows. Relevant files are currently being organized and will be updated gradually.

.
├── README.md
├── prompts/
├── generated_code/
├── logs/
├── reference_solutions/
├── evaluation/
├── environment.yml
└── requirements.txt
