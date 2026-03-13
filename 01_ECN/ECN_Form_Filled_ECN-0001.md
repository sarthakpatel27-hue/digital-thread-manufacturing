# ECN Form — Filled Example

## Header
- ECN ID: **ECN-0001**
- Title: **Improve gimbal weld location control (fixture locator + WI + inspection update)**
- Originator: **Manufacturing Engineering**
- Date Raised: **2025-12-23**
- Priority: **Quality / Rework Reduction**
- Reason: **Variation control + reduce rework due to gimbal mislocation**

## Change Description
- Item(s) changing:
  - **FX-2001 Assembly/Weld/Inspect Fixture — Rev A → Rev B**
  - **WI-OP40 Weld WI — Rev A → Rev B**
  - **CMM-PROG-01 — Rev A → Rev B**
  - **DWG-1000 Drawing Pack — Rev A → Rev B** *(only if drawing needs tighter CTQ callout; otherwise keep as reference update)*
- From → To:
  - From: Rev A setup relies on operator judgment for gimbal position within fixture.
  - To: Rev B adds positive location feature (fixture locator) + explicit WI steps + CMM program CTQ checks.
- Acceptance criteria:
  - Gimbal locations between **Station 1–2** and **Station 2–3** consistently meet CTQ tolerances.
  - First build on Rev B passes inspection without rework attributable to gimbal mislocation.

## Impacted Objects (tick all)
- [ ] EBOM
- [ ] MBOM
- [x] Routing
- [x] Work Instructions
- [x] Tooling / Fixtures
- [x] Gauges / Calibration
- [x] CMM Program
- [x] Inspection plan / FAI
- [ ] Supplier/Purchasing
- [x] Inventory/WIP disposition

## Effectivity Proposal
- Effectivity type: **Date**
- Proposed effective date: **2026-01-15**
- WIP handling plan:
  - WOs released **before 2026-01-15** may complete on Rev A.
  - WOs released **on/after 2026-01-15** must use **Rev B** (FX-2001 Rev B + WI-OP40 Rev B + CMM-PROG-01 Rev B).

## Risk & Verification
- Risks if missed:
  - Continued mislocation → rework/scrap, inspection escapes, schedule impact.
  - Mixed execution definition if WI/tooling/inspection not aligned.
- Verification required:
  - **Fixture re-qualification** report for FX-2001 Rev B
  - **First Article / First Build** inspection on first unit built to Rev B
  - **CMM report** confirming CTQ compliance
- Evidence to attach:
  - Updated fixture drawing/rev record
  - Updated WI-OP40 with revision history
  - Updated CMM program rev record
  - Trial build + inspection record links

## Approvals (Sign-off)
- Engineering: ___________________ Date: ________
- Manufacturing Engineering: ___________________ Date: ________
- Quality: ___________________ Date: ________
- Supply Chain: ___________________ Date: ________
- Change Authority: ___________________ Date: ________
