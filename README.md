# Saeed Asadzadeh

I build working software with AI agents. I take an unfamiliar problem, write a spec with clear acceptance criteria, and direct coding agents (**Claude Code** and **OpenAI Codex**) through staged delivery, independent review and automated testing. Where it fits, I make the agents check each other's work.

The projects below cover finance, economics, physiology, mechanical engineering and 3D. Each repository explains what was built, how the agents were used and how to run it.

## Agentic AI and financial data

| Project | What it shows |
|---|---|
| [**civilization-infrastructure-markets**](https://github.com/sesasa/civilization-infrastructure-markets) | A multi-agent research debate (Codex ↔ Claude) tested against five years of global market data, with a data pipeline and an auto-generated PDF report. |
| [**financial-ontology-lab**](https://github.com/sesasa/financial-ontology-lab) | An RDF/SPARQL knowledge graph over SEC filings, with full provenance and a grounded context packet for LLM agents. |
| [**nvidia-earnings-cli**](https://github.com/sesasa/nvidia-earnings-cli) | SEC EDGAR → SQLite with deterministic financial Q&A, plus an LLM mode that cites its evidence and never runs model-generated SQL. |

## Simulation and modelling

| Project | What it shows |
|---|---|
| [**city-economy-simulator**](https://github.com/sesasa/city-economy-simulator) | An 11-stage, stock-flow-consistent economy simulator built with Claude Code from a spec. Plugin layers, 178 tests and an animated town twin. |
| [**money-lab**](https://github.com/sesasa/money-lab) | An interactive monetary-economy lab (React and TypeScript). Built with Codex, with the architecture reviewed by Claude. |
| [**human-energy-flow**](https://github.com/sesasa/human-energy-flow) | A metabolism, exercise and adaptation simulator based on real food data, with more than ten test suites and independent agent reviews. |

## Interactive 3D and engineering

| Project | What it shows |
|---|---|
| [**3d-house-walkthrough**](https://github.com/sesasa/3d-house-walkthrough) | A Danish villa rebuilt from photos into a walkable Three.js house with GPU-baked lighting (Blender on RunPod), Unreal scenes and an OpenFOAM winter heating study. |
| [**forklift-explained**](https://github.com/sesasa/forklift-explained) | A narrated, physics-backed explainer of a forklift powertrain, with CI deployment to GitHub Pages. |

## How I work with agents

- **Spec first.** I write a brief with phases and acceptance criteria. The agent builds one phase, then stops for review.
- **Independent review.** A second agent (or model) reviews architecture and results, and its findings and decisions are kept in the repo.
- **Verifiable output.** Invariants, golden regressions, unit tests and Playwright tests, plus a documented source for every model assumption.
- **Provenance.** Sourced data, pinned snapshots and recorded design decisions (`DECISIONS.md`).
