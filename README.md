# Spreadsheet Gym

An RLVR graded, deterministic Excel and PowerPoint sandbox in which a banker agent must rebuild a real LBO model and pass 47 unit tests — the missing financial services chapter of Westworld, shipped as a drop in westworld.envs.spreadsheet module.

![Spreadsheet Gym working dashboard](outputs/project_working.svg)

## Why it exists

Spreadsheet Gym's public assets (Westworld, WebBench, BrowserBench) all live in web / e commerce / travel task surfaces. But their funded thesis and only open job rec both name financial services knowledge work — Excel, PowerPoint, IB modeling as the wedge. There is currently zero published Spreadsheet Gym environment for the workflow that actually generates the.

The project is intentionally built as a local replay harness instead of a slide. It creates fixtures, plants realistic failure modes, produces citation-locked evidence, and turns the result into a dashboard a reviewer can inspect without credentials or hosted services.

## What is inside

- Deterministic fixture generation for the company-specific risk surface.
- Strategy code in `src/spreadsheet_gym/strategy.py` with project-specific scoring and visual evidence.
- Citation-locked reports where every decision claim points to a generated evidence ID.
- Two regenerated visual artifacts: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, benchmark, and test artifacts.

![Spreadsheet Gym evidence map](outputs/evidence_map.svg)

## Signals it measures

- `Spreadsheet Gym coverage`
- `assets risk`
- `westworld precision`
- `webbench latency`

## Failure modes it plants

- Spreadsheet Gym drift
- assets gap
- westworld misroute
- webbench blindspot

## Run it locally

```bash
uv sync
uv run spreadsheet-gym all
uv run pytest -q
uv run ruff check .
```

## Outputs worth opening

- `outputs/dashboard.html`
- `outputs/project_working.svg`
- `outputs/evidence_map.svg`
- `outputs/operator_brief.md`
- `outputs/decision_report.md`
- `outputs/strategy_model.json`
- `outputs/demo_pack.zip`

## Boundary

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.
