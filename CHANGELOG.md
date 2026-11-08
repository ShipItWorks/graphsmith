# Changelog

Public record of changes to graphsmith, written from the product page on shipitworks.com. The source is private. Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Release tags exist on the private repository's default branch.

## 2026-11-08 (release v0.4.0)

- 2026-11-08: Release v0.4.0 on main head b9aca48. CI moved to the self-hosted runner (PR #107). Recorded browser run of the readiness report, coverage, State map, decision rules and connections: 28/28 on three templates, the control fails (PR #75, proof/readiness-state.log). Lane notes added to FOUND.md (PR #31).
- 2026-11-08: Recorded runs for the three scorecard features: domain logic 107 tests, workspace UI 14/14, live demo build match (PR #8); network capture on graphsmith.dev, 0 requests after load, typed text in no request (PR #7). The three features are now Proven.
- 2026-11-08: Phone-size workspace tab row now wraps; a new check runs every route at phone size and in dark mode, 42/42 (PR #28).
- 2026-11-08: The State tab tags a reviewer decision chosen in Evaluate as user, not mocked, and the second-visit auto-approval as generated; the tab's note explains all four tags (PR #66).
- 2026-11-08: Share links cap rules at 20 per decision and 400 in all, and clip quoted decision text to 80 characters (PR #20). Readiness checks carry the NIST AI RMF 1.0 subcategory each relates to; the mapping is a judgement, not measured (PR #21).
- 2026-11-08: Privacy page and in-app copy pinned to the code: network and storage sentences (PR #10), the three page-load requests (PR #12), exclude fields removed not replaced (PR #27, PR #29); landing page templates and checks lines (PR #9, PR #26).

Score 82 / 100 on our own rubric, scored 2026-11-08. Product page: https://shipitworks.com/apps/#graphsmith

## 2026-11-07 (release v0.3.0)

- The readiness checks are tagged with the NIST AI RMF 1.0 subcategory each relates to (the subcategory text is quoted from NIST; which subcategory a check relates to is a judgement, not measured). Share links now cap rules and clip quoted decision text, fixing a defect found in the proof pack, and the export label, share toast and Privacy page say that exclude fields are removed from scenarios, not replaced. The Privacy page lists the three requests a browser makes at load.
- A new check runs every route at phone size and in dark mode, and fixed a phone tab-row overflow. Recorded runs on one machine in headless Chrome: canvas, inspector, outline and tabs; no off-site request in the demo journey; the live demo served the build checked then; unit tests for simulator, lint, export, share and drafter. Release v0.3.0.

Score 67 / 100 on our own rubric, scored 2026-11-01; no score or proof label changed in this update. Product page: https://shipitworks.com/graphsmith/
