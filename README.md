# Saeed Asadzadeh

I build working software with AI agents. I take an unfamiliar problem, write a spec with clear acceptance criteria, and direct coding agents (**Claude Code** and **OpenAI Codex**) through staged delivery, independent review and automated testing. Where it fits, I make the agents check each other's work.

The projects below cover robotics, finance, economics, physiology, mechanical engineering and 3D. Each repository explains what was built, how the agents were used and how to run it.

## Featured

| Project | What it shows |
|---|---|
| [**cad-operations-atlas**](https://github.com/sesasa/cad-operations-atlas) | An interactive Three.js atlas of 44 CAD modeling operations, from extrude and loft to zebra stripes and mold splits, plus a 6'0" shortboard built step by step from those operations. [**Live demo**](https://sesasa.github.io/cad-operations-atlas/) |

## Robotics

| Project | What it shows |
|---|---|
| [**soarm-mujoco-mirror**](https://github.com/sesasa/soarm-mujoco-mirror) | A real SO-101 arm with a calibrated MuJoCo twin. Say "pick and place the biscuit": GPT picks the object from the camera image, then SciPy/MuJoCo IK plans the motion and the real arm executes it. Videos: [GPT pick-and-place](https://github.com/sesasa/soarm-mujoco-mirror/blob/main/media/gpt-pick-and-place.mp4), [sim-to-real grasp](https://github.com/sesasa/soarm-mujoco-mirror/blob/main/media/sim-to-real-grasp.mp4). |

## Simulation and modelling

| Project | What it shows |
|---|---|
| [**human-energy-flow**](https://github.com/sesasa/human-energy-flow) | A metabolism, exercise and adaptation simulator based on real food data, with more than ten test suites and independent agent reviews. [**Live demo**](https://sesasa.github.io/human-energy-flow/) |
| [**city-economy-simulator**](https://github.com/sesasa/city-economy-simulator) | An 11-stage, stock-flow-consistent economy simulator built with Claude Code from a spec. Plugin layers, 178 tests and an animated town twin. |
| [**money-lab**](https://github.com/sesasa/money-lab) | An interactive monetary-economy lab (React and TypeScript). Built with Codex, with the architecture reviewed by Claude. |

## Interactive 3D and engineering

| Project | What it shows |
|---|---|
| [**3d-house-walkthrough**](https://github.com/sesasa/3d-house-walkthrough) | A Danish villa rebuilt from photos into a walkable Three.js house with GPU-baked lighting (Blender on RunPod), Unreal scenes and an OpenFOAM winter heating study. |
| [**forklift-explained**](https://github.com/sesasa/forklift-explained) | A narrated, physics-backed explainer of a forklift powertrain, with CI deployment to GitHub Pages. |

## Agentic AI and financial data

| Project | What it shows |
|---|---|
| [**civilization-infrastructure-markets**](https://github.com/sesasa/civilization-infrastructure-markets) | A multi-agent research debate (Codex ↔ Claude) tested against five years of global market data, with a data pipeline and an auto-generated PDF report. |
| [**financial-ontology-lab**](https://github.com/sesasa/financial-ontology-lab) | An RDF/SPARQL knowledge graph over SEC filings, with full provenance and a grounded context packet for LLM agents. |
| [**nvidia-earnings-cli**](https://github.com/sesasa/nvidia-earnings-cli) | SEC EDGAR → SQLite with deterministic financial Q&A, plus an LLM mode that cites its evidence and never runs model-generated SQL. |

## How I work with agents

- **Spec first.** I write a brief with phases and acceptance criteria. The agent builds one phase, then stops for review.
- **Independent review.** One agent builds and the other reviews. Codex usually builds with Claude Code consulting, or Claude Code builds with Codex consulting. Their reviews and decisions are kept in the repo.
- **Verifiable output.** Invariants, golden regressions, unit tests and Playwright tests, plus a documented source for every model assumption.
- **Provenance.** Sourced data, pinned snapshots and recorded design decisions (`DECISIONS.md`).
