# SOP — EBOM → MBOM Translation (Portfolio Version)

## Purpose
Convert as-designed structure into as-executed structure with operations, consumption, and records.

## Translation rules (minimum)
- Every produced/assembled item must map to:
  - a routing operation
  - required records (traveler/MES fields)
  - required resources (fixtures/gauges/programs) referenced via `Resources_by_Op`
- Process materials (sealant, wipes, purge gas) appear in MBOM as **Consume**
- Tooling does **not** go into MBOM as parts; it is controlled via `Tooling_BOM` + `Resources_by_Op` + WI headers
- Outsourced parts are controlled by receiving checks + CoC + Revision matching
- In-house IP parts are controlled via IP traveler + QC release records (OP30)
- Fixtures/gauges are controlled via Tooling_BOM + Resources_by_Op, not as MBOM items

## Outputs
- EBOM tab (engineering)
- MBOM tab (manufacturing consumption)
- Routing tab (operation plan + WI links)
- Tooling_BOM and Resources_by_Op tabs (execution resources)
