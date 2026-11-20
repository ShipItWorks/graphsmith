# Graphsmith

A design-time environment for graph-based AI and automation workflows.

Paused since 18 November 2026, while I finish patchowner. See [patchowner](https://shipitworks.com/patchowner/).

**Score: 82 / 100** on my own [rubric](https://shipitworks.com/how-we-score/). Stage: Beta. Scored 2026-11-12; this record was updated 2026-11-18 from the [product page](https://shipitworks.com/graphsmith/).

Every number on the product page names the file it came from. The lists below are copied from that page, not rewritten.

**Platform.** Web only.

## What works today

- Simulator, lint/readiness, export, share encoding, drafter (domain logic) (Proven)
- Graph canvas, inspector, outline, tabs UI (Proven)
- Live demo graphsmith.dev (Proven)

## Not done yet

- Headless Chrome checks ran on one machine: check:ui 18/18 and check:display 42/42 on 2026-11-07 and 2026-11-08, and check:ui 32/32 at commit 8f883bb in a review on 2026-11-18, which included the read-only share view; other browsers are not covered, and no screen reader run at a commit in main's history is recorded (proof/screen-reader.log cites 78539b0, a branch tip)
- graphsmith.dev was fetched on 2026-11-07 (bfa6b4d) and 2026-11-08 (1692e9f) and served the build checked each time (proof/live-demo.log). On 2026-11-18 a review found graphsmith.dev serving the build of commit 8f883bb (check:live --require-build-match); uptime was not measured
- A request capture of one journey on graphsmith.dev (2026-11-07) saw 0 requests after load and 3 during load; it does not cover browser extensions or other browsers
- npm audit ran from an offline cache, so the 0-vulnerability result is not independently confirmed
- A privacy page exists (#/privacy) and its network, storage and redaction sentences are pinned to the app code by tests; whether it meets a legal privacy-policy requirement was not checked
- CI on main runs on one self-hosted runner (PR #107); its result at head f795d64 was read once from `gh run list` on 2026-11-12 and the job logs were not read; the run on the PR #123 merge commit 03b07bb shows cancelled
- package.json says 0.1.0 while the release tag is v0.5.0
- The proof pack on main (proof/proof-pack.json, PR #120) is the auditor's run at e090d60 on 2026-11-08 with verdict STOP and 10 open items; e090d60 is a branch tip outside main's history, and the test count here (153) is from the earlier 7c913f0 audit, not from f795d64
- Proof logs cite the commit they ran on; except the commits the three feature logs cite (bfa6b4d, 1692e9f) those commits are branch tips replaced by squash merges, so they cannot be opened in main's history

## What changed

- 2026-11-18: A review at commit 8f883bb ran 881 tests (881 passed) and check:ui 32/32, and ran the exported files unchanged: 17 of 17 in LangGraph and 15 of 17 in n8n. The n8n export target was removed from Where it's going because the export is built. No feature label or score changed.
- 2026-11-11: Merged into the product, as its own change log describes them: exports you can run from the Export tab, past runs and a test-dataset loader in the Evaluate tab, a History tab, and two more MCP tools. This scorecard round did not run them; no feature label or score changed (PRs #123, #125 and #122).
- 2026-11-10: Land PR #121 merged into main as a13b073 (39 lane PRs included); no feature label changed this round. Tagged v0.5.0 at a13b073.
- 2026-11-08: Release v0.4.0 on main head b9aca48. CI moved to the self-hosted runner (PR #107). Recorded browser run of the readiness report, coverage, State map, decision rules and connections: 28/28 on three templates, the control fails (PR #75, proof/readiness-state.log). Lane notes added to FOUND.md (PR #31).
- 2026-11-08: Recorded runs for the three scorecard features: domain logic 107 tests, workspace UI 14/14, live demo build match (PR #8); network capture on graphsmith.dev, 0 requests after load, typed text in no request (PR #7). The three features are now Proven.
- 2026-11-08: Phone-size workspace tab row now wraps; a new check runs every route at phone size and in dark mode, 42/42 (PR #28).

See [CHANGELOG](CHANGELOG.md).

## Demo

[Transcript of the demo (2:08)](https://shipitworks.com/graphsmith/transcript/) · video on the [product page](https://shipitworks.com/graphsmith/)

The demo voice is AI-generated (ElevenLabs, "Bella") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README and a CHANGELOG, and soon a LICENSE. Until the source is public, the [product page](https://shipitworks.com/graphsmith/) is the source of truth, and the score above is the one to trust.

## How I work

I say only what I can back. I say what is not finished before anyone asks. I name people, companies and tools to give credit. I collect as little data as possible. Built with Claude, by Anthropic: Claude helps write the code and wrote this README. Directed, tested and owned by Robert Sweetman in Stoughton, Massachusetts.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.
