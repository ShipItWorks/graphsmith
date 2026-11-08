# Graphsmith

A design-time environment for graph-based AI and automation workflows.

**Score: 67 / 100** on our own [rubric](https://shipitworks.com/how-we-score/). Stage: Beta. Scored 2026-11-01; this record was updated 2026-11-07 from the [product page](https://shipitworks.com/apps/#graphsmith).

Every number on the product page names the file it came from. The lists below are copied from that page, not rewritten.

**Platform.** Web only.

## What works today

- Simulator, lint/readiness, export, share encoding, drafter (domain logic)

## Not done yet

- A headless Chrome check (check:ui) of the graph canvas, inspector, outline and tabs passed on one machine on 2026-11-07; the read-only share view and other browsers are not covered
- Live demo graphsmith.dev was fetched once on 2026-11-07 and served this build; uptime was not measured
- No dark mode (light theme only)
- npm audit ran from an offline cache, so the 0-vulnerability result is not independently confirmed
- A privacy page exists (#/privacy) and its network and storage sentences are pinned to the app code by tests (2026-11-07); whether it meets a legal privacy-policy requirement was not checked

## What changed

- 2026-11-07: The readiness checks are tagged with the NIST AI RMF 1.0 subcategory each relates to (the subcategory text is quoted from NIST; which subcategory a check relates to is a judgement, not measured). Share links now cap rules and clip quoted decision text, fixing a defect found in the proof pack, and the export label, share toast and Privacy page say that exclude fields are removed from scenarios, not replaced. The Privacy page lists the three requests a browser makes at load.
- 2026-11-07: A new check runs every route at phone size and in dark mode, and fixed a phone tab-row overflow. Recorded runs on one machine in headless Chrome: canvas, inspector, outline and tabs; no off-site request in the demo journey; the live demo served the build checked then; unit tests for simulator, lint, export, share and drafter. Release v0.3.0.

Full list with release tags: [CHANGELOG](CHANGELOG.md).

## Demo

[Transcript of the demo (1:46)](https://shipitworks.com/graphsmith/transcript/) · video on the [product page](https://shipitworks.com/apps/#graphsmith)

The demo voice is AI-generated (ElevenLabs, "Alice") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README and a CHANGELOG, and soon a LICENSE. Until the source is public, the [product page](https://shipitworks.com/apps/#graphsmith) is the source of truth, and the score above is the one to trust.

## How we work

Say only what we can back. Say what is not finished before anyone asks. Name people, companies and tools to give credit. Collect as little data as possible. We use AI and say so: Claude (by Anthropic) helps write the code and wrote this README.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.
