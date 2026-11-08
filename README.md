# Graphsmith

A design-time environment for graph-based AI and automation workflows.

**Score: 82 / 100** on our own [rubric](https://shipitworks.com/how-we-score/). Stage: Beta. Scored 2026-11-08; this record was updated 2026-11-08 from the [product page](https://shipitworks.com/apps/#graphsmith).

Every number on the product page names the file it came from. The lists below are copied from that page, not rewritten.

**Platform.** Web only.

## What works today

- Simulator, lint/readiness, export, share encoding, drafter (domain logic) (Proven)
- Graph canvas, inspector, outline, tabs UI (Proven)
- Live demo graphsmith.dev (Proven)

## Not done yet

- Headless Chrome checks (check:ui 14/14, check:display 42/42) ran on one machine on 2026-11-07 and 2026-11-08; the read-only share view and other browsers are not covered, and no screen reader has been run
- graphsmith.dev was fetched once on 2026-11-07 and served the build checked then; a 2026-11-08 check:display run against it failed 4 of 42 (phone tab row), fixed on main in PR #28. Whether the live site serves b9aca48 is not yet traced; uptime was not measured
- A request capture of one journey on graphsmith.dev (2026-11-07) saw 0 requests after load and 3 during load; it does not cover browser extensions or other browsers
- npm audit ran from an offline cache, so the 0-vulnerability result is not independently confirmed
- A privacy page exists (#/privacy) and its network, storage and redaction sentences are pinned to the app code by tests; whether it meets a legal privacy-policy requirement was not checked
- CI on main head b9aca48 was queued, not green, when checked on 2026-11-08; last green run is 8b83b34
- package.json says 0.1.0 while the release tag is v0.4.0
- The independent proof pack (proof/proof-pack.json) is from 7c913f0 on 2026-11-02 with verdict STOP; its share-link defect is fixed by PR #20, but the pack was not regenerated, so test counts (153) are from that audit, not from b9aca48
- Proof logs cite the commit they ran on; except the three feature logs (bfa6b4d) those commits are branch tips replaced by squash merges, so they cannot be opened in main's history

## What changed

- 2026-11-08: Release v0.4.0 on main head b9aca48. CI moved to the self-hosted runner (PR #107). Recorded browser run of the readiness report, coverage, State map, decision rules and connections: 28/28 on three templates, the control fails (PR #75, proof/readiness-state.log). Lane notes added to FOUND.md (PR #31).
- 2026-11-08: Recorded runs for the three scorecard features: domain logic 107 tests, workspace UI 14/14, live demo build match (PR #8); network capture on graphsmith.dev, 0 requests after load, typed text in no request (PR #7). The three features are now Proven.
- 2026-11-08: Phone-size workspace tab row now wraps; a new check runs every route at phone size and in dark mode, 42/42 (PR #28).
- 2026-11-08: The State tab tags a reviewer decision chosen in Evaluate as user, not mocked, and the second-visit auto-approval as generated; the tab's note explains all four tags (PR #66).
- 2026-11-08: Share links cap rules at 20 per decision and 400 in all, and clip quoted decision text to 80 characters (PR #20). Readiness checks carry the NIST AI RMF 1.0 subcategory each relates to; the mapping is a judgement, not measured (PR #21).
- 2026-11-08: Privacy page and in-app copy pinned to the code: network and storage sentences (PR #10), the three page-load requests (PR #12), exclude fields removed not replaced (PR #27, PR #29); landing page templates and checks lines (PR #9, PR #26).

See [CHANGELOG](CHANGELOG.md).

## Demo

[Transcript of the demo (2:10)](https://shipitworks.com/graphsmith/transcript/) · video on the [product page](https://shipitworks.com/apps/#graphsmith)

The demo voice is AI-generated (ElevenLabs, "Alice") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README and a CHANGELOG, and soon a LICENSE. Until the source is public, the [product page](https://shipitworks.com/apps/#graphsmith) is the source of truth, and the score above is the one to trust.

## How we work

Say only what we can back. Say what is not finished before anyone asks. Name people, companies and tools to give credit. Collect as little data as possible. We use AI and say so: Claude (by Anthropic) helps write the code and wrote this README.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.
