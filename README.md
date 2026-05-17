# Misconception Intervention Engine

A local education analytics prototype that maps synthetic learner signals to standards-aligned misconceptions and intervention recommendations.

## Features

- Synthetic classroom, assessment, standard, and intervention records.
- Misconception clustering with evidence-backed intervention ranking.
- Static dashboard and verifier for explainable instructional recommendations.

## Run Locally

```bash
uv sync
uv run app init-demo
uv run app ingest fixtures/
uv run app analyze
uv run app verify
uv run app dashboard
uv run app benchmark
uv run app export-demo-pack
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/dashboard.html`
- `outputs/decision_report.md`
- `outputs/evidence_graph.mmd`
- `outputs/risk_or_quality_report.csv`
- `outputs/benchmark.md`
- `outputs/demo_pack.md`

## Data Policy

This project runs fully locally on deterministic synthetic fixtures. It does not require external APIs, credentials, private datasets, network access, or production systems.
