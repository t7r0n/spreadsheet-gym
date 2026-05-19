# Spreadsheet Gym

An RLVR graded, deterministic Excel and PowerPoint sandbox in which a banker agent must rebuild a real LBO model and pass 47 unit tests - the missing financial services chapter of Westworld, shipped as a drop in westworld.envs.spreadsheet module.

## Why This Exists

Halluminate's public assets (Westworld, WebBench, BrowserBench) all live in web / e commerce / travel task surfaces. But their funded thesis and only open job rec both name financial services knowledge work - Excel, PowerPoint, IB modeling as the wedge. There is currently zero published Halluminate environment for the workflow that actually generates the dollars on a banker's screen: opening an LBO model in Excel, drag filling a debt schedule, and verifying it agrees to the cap table on slide 7 of a PowerPoint.

## What It Builds

- Replays synthetic `halluminate` and `public` cases against the project's evidence rules.
- Scores `halluminate_coverage`, `public_risk`, and `assets_precision` so regressions are visible in CSV and JSON.
- Plants `halluminate drift` and `public gap` failures as negative controls.
- Writes citation-locked decision claims; unsupported claims fail verification.
- Exports a review dashboard and demo pack for `spreadsheet-gym` without hosted services.

## Local Run

```bash
uv sync
uv run spreadsheet-gym all
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/analysis.json`
- `outputs/scenario_report.csv`
- `outputs/decision_report.md`
- `outputs/evidence_packet.md`
- `outputs/dashboard.html`
- `outputs/demo_pack.zip`

## Sources

- https://www.halluminate.ai/blog/westworld
- https://github.com/Halluminate
- https://github.com/Halluminate/westworld
- https://github.com/Halluminate/WebBench
- https://github.com/Halluminate/browserbench
- https://www.ycombinator.com/companies/halluminate
- https://www.ycombinator.com/companies/halluminate/jobs
- https://antigravity.capital/portfolio/halluminate
- https://x.com/Jerr_Wu
- https://github.com/wyatt-halluminate

## Boundary

This repository uses synthetic fixtures only. It has no credentials, no customer data, no outreach data, and no dependency on a hosted API.
