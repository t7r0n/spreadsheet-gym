# Operator Brief: Halluminate

Halluminate gets a local, deterministic pressure test around halluminate, assets, and westworld. The useful part is the repeatable evidence path from fixture to failure to operator action.

## Highest-leverage checks

- halluminate evidence replay -> block release until cited evidence is regenerated (halluminate_coverage, evidence ev_0000).
- webbench operator packet -> accept only if decision claims cite fixture evidence (assets_risk, evidence ev_0011).
- westworld regression harness -> open a regression issue with trace and benchmark delta (westworld_precision, evidence ev_0066).
- assets boundary probe -> route to reviewer with evidence packet (webbench_latency, evidence ev_0121).

## What makes this useful

The workflow is intentionally local and deterministic. A reviewer can run the same fixture set, inspect the evidence IDs, open the dashboard, and see exactly why a recommendation passed, went to review, or blocked.
