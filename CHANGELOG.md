# Changelog

All material changes to Emerson Style are recorded here, newest first. The style follows semver: major for profile rewrites, minor for new gates or rules, patch for wording fixes.

## 1.6.0 — 2026-09-19

Source: Ahmed's corrections on the v1.5.2 daily test (AI coding agents piece) in #ai-writing-voice.

- **Mirrored-clause stem ban.** "Teams that write more specifications, and that treat context as a discipline with its own budget, report the strongest results" — the repeated "that" stem building to a simple win reads as AI scaffolding even when both clauses are concrete (Ahmed: "the repetitive stem that leads to a simple win feels too much like an AI artifact"). Practices are now stated as plain nouns ("clearer briefs before the agent starts, and review funded as a deliverable in its own right"). Notably, this reverses the replacement example v1.4.0 introduced for the in-group tell — that sentence failed in the field; the in-group rule's example was swapped and the reversal is documented inline.
- **Executive-register rule.** Practitioner jargon ("context management," "survives in production," "mergeable," "the review layer") marks a piece as written for engineers; the reader is a business professional or executive, so the argument runs in the executive's ledger — budgets, deliverables, returns, trust. A technical term survives only when it is the unit of measurement (pull requests per author). Root echoes inside one sentence ("how much of the productivity survives in production") are banned as generated-sounding. Gate 3 and Do/Don't updated.

## 1.5.2 — 2026-09-19

- **Knowing-aside ban.** Qualifiers must carry observation, not smugness: "as it usually does," "as always," "predictably," "of course" are banned (Ahmed: "'as it usually does' is not good — it sounds too knowing"). The knowing sage is the fourth persona pose after the casual aside, the helpful assistant, and the hip insider. Gate 3 verdict rule and Do/Don't updated.

## 1.5.1 — 2026-09-19

- **Test-post formatting.** Daily test pieces posted to Slack are now broken into paragraphs of 2–4 sentences — the voice's own paragraph-length profile — instead of one run-on block (Ahmed: "format the paragraphs of the sentences"). Delivery step updated.

## 1.5.0 — 2026-09-19

Source: Ahmed's fourth correction on the v1.3.0 daily test, generalizing the qualified-verdict rule.

- **Connective-tissue rule.** AI copy cuts transition words (however, nevertheless, although, still, yet) for token efficiency, which compresses idea density and removes the pauses a subvocalizing reader needs. These connectives are now expected seasoning: several per piece, mid-sentence and between sentences. Gate 1 gained a connective check (a draft with zero is over-compressed); Gate 2's formal-opener ban was scoped to paragraph scaffolding (Furthermore/Moreover/Therefore opening paragraphs) so it can't be used to strip qualifying connectives; Rhythm profile and Do/Don't updated.

## 1.4.0 — 2026-09-19

Source: Ahmed's corrections on the v1.3.0 daily test (AI coding agents piece) in #ai-writing-voice.

- **Qualified-verdict rule.** Bare short verdicts ("Adoption is the easy part.") pose as casual asides — a reliable AI tell. Every standalone verdict now carries a qualifier or subordinate clause ("Adoption, however, is often the easy part."); verdicts run 6–14 words. The bare fragment survives only as the answer inside the rhetorical-question device ("A potential pitfall? Settling for too little."), where the question carries the setup. Rhythm profile, Gate 1, Gate 3, and Do/Don't updated.
- **Advice-register ban.** The voice is impersonal exposition; it observes and weighs, it does not advise the reader. Reader-directed imperatives ("Fund the review layer as deliberately as you funded the models") shift into helpful-assistant register — an AI giveaway. Closers now end on a sharp observation that states the imbalance and lets the implication sit. Imperatives survive only in dedicated, labeled advice sections with bolded leads. Attitude, structural-habits, Gate 3 closer rule, and Do/Don't updated.
- **In-group tell ban.** Winner-club casualisms ("The teams getting the most from agents…") read as hip insider language — "it's cool to be in the know" — not executive consulting. Evidence is now stated through the practice itself, not the club practicing it. The three rules share one principle: the voice never performs a persona (casual aside, helpful assistant, hip insider). Gate 3, word-choice avoid list, and Do/Don't updated.

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
