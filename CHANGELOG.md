# Changelog

Public record of changes to graphsmith, written from the product page on shipitworks.com. The source is private. Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Release tags exist on the private repository's default branch.

## 2026-11-07 (release v0.3.0)

- The readiness checks are tagged with the NIST AI RMF 1.0 subcategory each relates to (the subcategory text is quoted from NIST; which subcategory a check relates to is a judgement, not measured). Share links now cap rules and clip quoted decision text, fixing a defect found in the proof pack, and the export label, share toast and Privacy page say that exclude fields are removed from scenarios, not replaced. The Privacy page lists the three requests a browser makes at load.
- A new check runs every route at phone size and in dark mode, and fixed a phone tab-row overflow. Recorded runs on one machine in headless Chrome: canvas, inspector, outline and tabs; no off-site request in the demo journey; the live demo served the build checked then; unit tests for simulator, lint, export, share and drafter. Release v0.3.0.

Score 67 / 100 on our own rubric, scored 2026-11-01; no score or proof label changed in this update. Product page: https://shipitworks.com/graphsmith/
