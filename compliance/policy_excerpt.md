# Third-Party License Policy (Excerpt)

This policy applies to every model and dataset registered in
`compliance/asset_registry.json`.

## Decisions

| Decision | License families | Required action |
|---|---|---|
| `approved` | Apache-2.0, MIT, BSD-2-Clause, BSD-3-Clause, CC0-1.0 | None. Record the asset in the audit report. |
| `attribution_required` | CC-BY-3.0, CC-BY-4.0, CC-BY-SA-3.0, CC-BY-SA-4.0, GFDL | Open a review issue with label `license-attribution`. The owning team must publish the required attribution and honour any ShareAlike obligation. |
| `restricted` | Llama 3.x community license, Gemma license, BigCode OpenRAIL-M, any CC-BY-NC variant | Open a review issue with label `license-restricted`. Legal must review the terms before the asset can ship. |
| `unknown_license` | license missing, identified as "other", or an unrecognized identifier | Open a review issue with label `license-unknown`. The owning team must provide the license terms. |

## Issue conventions

- Title: `[License Review] <hub_repo>` where `<hub_repo>` is the asset's hub
  repository id exactly as registered.
- Body: state the asset key, the hub repo id, the observed license, the decision,
  and the next action for the owner.
- A review issue is opened only for assets that are not `approved`.

## Reporting

The completed per-asset decisions are reported in
`compliance/reports/audit_report_2026Q4.json` and summarised as a comment on the
quarterly tracking issue.
