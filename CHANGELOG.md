# Changelog

All material changes to Emerson Style are recorded here, newest first. The style follows semver: major for profile rewrites, minor for new gates or rules, patch for wording fixes.

## 1.3.0 — 2026-09-19

Source: first daily test-and-refine cycle run (topic: AI coding agents become the default; 10 standalone sentences posted to #ai-writing-voice with threaded self-assessment).

- **Piece-level verdict cap.** Gate 3's verdict-pairing budget extended: ≤1 per paragraph *and* ≤2 per piece. The first daily run produced three short verdicts in ten sentences — each legal per-paragraph, formulaic across the piece.
- **Evidence-mix rule.** At most one attributed survey per piece; further evidence must be named companies, dated decisions, or observable facts. The run stacked JetBrains and Safeguard surveys and read as report aggregation.
- **Gate 1 format scoping.** The 14–16-word mean applies to paragraph prose; standalone numbered sentences with mid-sentence attribution may run to a mean of ~18 provided the median stays near 14 and the long/short pairing survives. Attribution adds 4–6 words per sentence; the target was chasing the wrong number for the test-voice format.
- Do/Don't list: added the no-survey-stacking rule and the per-piece verdict cap.
- Confirmed the v1.2.0 caps-not-targets fix held: 5 of 10 sentences ran 20–29 words, only 2 of 10 under 8 words — no staccato regression.

## 1.2.0 — 2026-09-19

- **Overcorrection fix.** v1.1.0's density budgets were applied as targets, stripping the voice's signature moves and chopping sentences into staccato fragments (Ahmed: "sentences are too brief and have lost their adherence to the PwC style").
- Gate 1 gained an **overcorrection check**: >30% of sentences under 8 words = punchy-social drift, rebuild with long evidence sentences; every paragraph or two needs a 20–40-word analytical sentence.
- Gate 3 reframed: budgets are **caps, not targets** — the devices are signature moves, budget them don't eliminate them; run Gate 3 first, then re-run Gate 1 to confirm rhythm survived.
- Do/Don't list: added the no-overcorrection rule.

## 1.1.0 — 2026-09-19

- Renamed the skill from `elevated-voice` to **Emerson Style** (Ahmed).
- Added **Gate 3 — Structural AI-tell scan**: word-level bans were passing drafts that still read as AI. New rules:
  - Colon budget: ≤1 per paragraph, ≤2 per piece.
  - Rhetorical-question device: ≤1 per piece.
  - Verdict-sentence pairing: ≤1 per paragraph (signature, not skeleton).
  - Banned negative-reveal openers ("X, and it does not Y").
  - Banned in-line justification ("which is exactly why").
  - Not-X-but-Y pivots banned by structure, not string ("rather than," "less like… more like" count).
  - Three-item escalating lists cut to two specifics.
  - Loose-thread rule: carry doubt in the sentence, leave one thread open.
  - Closers must prescribe, not announce the insight.
- Delivery notes must now state the Emerson Style version used.

Source: Ahmed's feedback on the Jev/TypeSafe piece ("over use of colons, over use of rhetoric questions") plus Emerson's six-point structural diagnosis.

## 1.0.0 — 2026-09-19

- Initial extraction as `elevated-voice` from four PwC / Strategy& insight articles: rhythm profile, openers, word choice, punctuation, attitude, structural habits, Do/Don't list, calibration passages, Gates 1–2 (rhythm + AI-tell vocabulary) and Vale lint gate.
