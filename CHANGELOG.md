# Changelog

All material changes to Emerson Style are recorded here, newest first. The style follows semver: major for profile rewrites, minor for new gates or rules, patch for wording fixes.

## 1.16.0 — 2026-09-21

Daily test on the Anthropic September 2026 threat report (DeepSeek silently rerouting third-party harness traffic to Claude Opus — 12.1M exchanges in 14 days). Three rule changes from the self-assessment:

- Gate 1: format scoping extended to standalone demonstration pieces — under ~15 sentences, a mean up to ~17 is acceptable when the median stays ≤16 and the long/short pairing survives (evidence density, not padding, is what pushes a demonstration over the 14–16 band).
- Gate 3: verdict symmetry check added — a verdict whose nouns mirror each other ("the vendor's vendors") gets a plainness test; if it would fit on a poster, rewrite the grammar and keep the point.
- Gate 6: sound trips now include stressed s/r clusters across adjacent words ("silently rerouted requests") — trips the ear without tripping the eye.

## 1.15.0 — 2026-09-20

Source: self-assessment of the daily test on the read-vs-ship divide (Theo Browne's July question, Hashimoto's "agent psychosis"). Three additions, all from the run's own proposals: (1) Evidence-mix rule now explicitly blesses named practitioners carrying dated actions as first-class evidence, alongside named companies and dated decisions. (2) New Gate 3 check — deferred-payoff opener: an opener that names a frame must cash it out by the final third of the piece; loose threads may stay open, unpaid frames may not. (3) New Openers device — quoted-question evidence: a real, dated question from a named practitioner carried inside em-dashes grounds the era framing in a verifiable moment.

## 1.14.0 — 2026-09-19

Source: Ahmed's thread feedback on the v1.13.0 redo of the agentic-code-review test. Two corrections: (1) "And yes root out that shape of sentence" — the mirror-negation ban now covers the affirm/negate *shape* itself, not just the bare "is not"; the v1.13.0 fix sentence ("The productivity is real; the capacity to review the work, however, never grew with it.") still fails. (2) "The thing I want you to keep refining is the culling of advice baked into the language" — Ahmed flagged "Dismissal carries its own risk" from the redo as counsel disguised as observation: "rather than being a plain spoken narrator of what's occurring."

- **Mirror-negation ban hardened (Gate 3).** The ban now covers the shape, not the string: a balanced rhetorical unit built from an affirmation and its mirror negation reads generated even when the negative half carries its own verb. Narrate the facts plainly — "and"-joined or as separate observations ("The productivity gains are real, and the review capacity never grew to meet them.") — or cut the half that adds nothing. Gate 3 and Do/Don't updated.
- **Counsel baked into the language (Gate 3, extends the v1.4.0 advice-register ban).** Advice arrives dressed as observation: warning nouns ("dismissal carries its own risk," "the danger is," "a common mistake") and should-shaped statements ("the vendor data deserves skepticism") steer the reader's response without an imperative in sight — the helpful assistant managing the reader. The voice is a plain-spoken narrator of what's occurring: state the conflict of interest as fact ("the data comes from vendors selling the remedy") and let the reader reach the caution on their own. Test: does the sentence report what is happening, or manage what the reader should do or feel about it? Gate 3 and Do/Don't updated.

## 1.13.0 — 2026-09-19

Source: Ahmed's thread feedback on the v1.11.3 daily test (agentic code review piece): "'The X is true, but blank is not' is an AI trope. Be wary of using it." The flagged shape was the piece's own verdict pairing — "The productivity is real; the review capacity, however, is not." Same message confirmed the three v1.12.0 proposals ("Apply the rule change").

- **Mirror-negation trope (Gate 3).** A clause affirmed, then its mirror dismissed with a bare negation, contributes symmetry rather than information — and the tidy symmetry is the tell. The affirm-then-negate sibling of the not-X-but-Y pivot; hides inside the signature verdict pairing, so verdict sentences get scanned for it specifically. The contrast survives; the bare mirrored negation does not — the negative half needs its own verb and fact ("the capacity to review the work, however, never grew with it"). Gate 3 and Do/Don't updated.

## 1.12.0 — 2026-09-19

Source: Emerson self-assessment from the daily test on agentic code review (Faros AI / GitHub Copilot review data); three proposals implemented by Emerson per the daily refinement cycle.

- **Orphaned-comparative ban (Gate 3).** A comparative must carry its referent in the same sentence — "hit just as hard as everyone else," not "hit just as hard." Found when the v1.9.0 semicolon split divided a sentence and the second half lost the comparison's referent. Gate 3 and Do/Don't updated.
- **Flat-patch check (Gate 1).** Extends the v1.2.0 overcorrection check: flag any run of 3+ consecutive sentences under ~13 words in analytical prose. The cadence alternates long evidence and short verdict; a plateau at medium-short is neither. Gate 1 and Do/Don't updated.
- **Statistic-stacking note (Gate 6).** Two figures in one sentence on the same direction word ("churn up 861% and review time up 441%") trip the ear where the eye sees no problem — vary the verb or split the figures. Gate 6 and Do/Don't updated.

## 1.11.3 — 2026-09-19

Source: Ahmed's TTS policy for Gate 6, after Dexter supplied an ElevenLabs skill.

- **TTS policy replaces the v1.11.1 fallback.** Default is now skip-TTS: the read-aloud gate runs manually (read aloud or analytic breath/sound-trip pass) unless audio is requested. When audio is requested: ElevenLabs if an ElevenLabs API key is configured, else edge TTS, else skip TTS entirely and run the manual gate. Standing exception: the daily Emerson test always runs the TTS gate and delivers the audio to Ahmed. Gate 6 and Do/Don't updated; daily-test cron job updated to match.

## 1.11.2 — 2026-09-19

Source: Ahmed's approval of the two rule proposals from the v1.11.0 validation test (self-assessment thread in #ai-writing-voice).

- **Audible-collision extension to the sound-trip scan.** Banned phrases are now judged by ear, not by string: a word boundary doesn't neutralize a banned sound. "Service was always a trust business" is not the literal "as always," but a subvocalizing reader hears the banned knowing-aside anyway — it counts as a hit. Found in the v1.11.0 test closer; rewritten to "a trust business all along." Gate 6 updated.
- **Passive-detector fix.** The v1.11.0 passive scan matched only -ed/-en participles and missed irregulars ("were never built" slipped through the mechanical check in the test; only a manual pass caught it). Now: be-verb + optional adverb + any past participle, irregulars included. Gate 3 updated.

## 1.11.1 — 2026-09-19

Source: Ahmed's portability note for outside users of the skill.

- **No-TTS fallback for Gate 6.** The read-aloud gate no longer assumes a TTS provider: if no provider or API key is configured, skip the audio and run the gate manually (read aloud yourself, or do the analytic breath/sound-trip pass silently). TTS is a convenience, never a delivery blocker. Gate 6 and Do/Don't updated.

## 1.11.0 — 2026-09-19

Source: subvocalization research commissioned by Ahmed (`workspace/subvocalization-research-2026-09-19.md` — phonological loop, cognitive load theory, write-for-the-ear speechwriting craft). All six proposed rules approved by Ahmed and implemented.

- **Read-aloud gate (new Gate 6).** Read the draft aloud at speaking pace (or through TTS) before delivery — the subvocalizing reader performs this prose, so the ear is the final gate. Any sentence where the breath runs out gets split.
- **Breath rule.** Every sentence over ~20 words carries an internal pause point (comma or em-dash) where a speaker would naturally pause; a 25+ word sentence with no internal punctuation is a defect. Generalizes the v1.9.0 semicolon rule. Gate 1, rhythm profile, punctuation profile, and Do/Don't updated.
- **Depth cap.** Long evidence sentences (20–40 words) carry one level of embedding only, with the subject and main verb inside the first ~10 words — word count alone misses the overload that stacked subordination creates. Gate 1, rhythm profile, and Do/Don't updated.
- **Word-length plainness.** Prefer the shorter word when the meaning survives; no sentence built mostly of 3+ syllable abstractions (general-audience prose averages 4–5 letters per word). Gate 3, word-choice profile, and Do/Don't updated.
- **Sound-trip scan.** Read-aloud pass flags unintended rhyme and sibilant/alliterative runs in adjacent stressed words — distinct from the root-echo rule (echo = repeated word root, trip = sound collision). Gate 6 and Do/Don't updated.
- **Passive voice budget.** Key claims in active voice, actor before verb; passive under ~10% of sentences, kept for variety or a genuinely unknown actor. Gate 3, word-choice profile, and Do/Don't updated.

## 1.10.0 — 2026-09-19

Source: Ahmed's correction on the v1.9.0 redo of the AI-ROI-after-the-pilot daily test in #ai-writing-voice ("Be careful not to over use however and clauses. They are helpful but can become burdensome if overused."). The v1.9.0 redo carried however twice plus meanwhile, Instead, In practice, although, on its own, and in most cases — nearly every sentence hedged. (Synced to this repo late — the rule shipped in the local skill before the repo update that became v1.11.0.)

- **Connective budget.** The v1.5.0 connective floor gets a ceiling: however at most twice per piece; a hedging sub-clause ("meanwhile," "in practice," "on its own," "in most cases," "so far") at most once per paragraph; one qualification per sentence — a sentence that turns on a connective doesn't also carry a hedge. When most sentences hedge, the draft reads as if it doesn't trust its own claims: cut the hedges, keep the claims. Gate 1 and Do/Don't updated.

## 1.9.0 — 2026-09-19

Source: Ahmed's approvals and corrections on the v1.8.0 daily test (AI-ROI-after-the-pilot piece) in #ai-writing-voice.

- **Root-echo rule extended across sentence boundaries (Ahmed: "Extend the root echo rule").** The v1.6.0 rule banned doubled roots inside one sentence; the v1.8.0 test echoed "workflow" through three consecutive sentences and passed legally. Now: the same content root in 3+ consecutive sentences reads generated even when each sentence is clean — vary the noun or restructure the middle sentence. Gate 3 and Do/Don't updated.
- **Format-scoping addendum (Ahmed: "Fine on format scoping").** For standalone-sentence runs carrying an attribution sentence, a median of 15–16 is acceptable — chasing 14 fragments the evidence sentences. Gate 1 updated.
- **Bridge-the-jump-cut rule (Ahmed, mid-revision correction).** Sentences should not cut harshly from one to the next when a bridge is natural: "The stall, however, is rarely a model problem. The budgets that funded the experiment did not fund…" leaves the reader to make the turn alone; "Instead, the real problem often sits in the budgets: …" hands off explicitly. Scan every boundary where a sentence explains or extends the previous one; a cold new subject gets a transitional marker or a restated subject. Scoped to sentence-level hand-offs — the formal-opener ban (Furthermore/Moreover/Therefore as paragraph scaffolding) stands. Gate 3 and Do/Don't updated.
- **Semicolon pacing rule (Ahmed, mid-revision correction).** A semicolon never joins two long clauses — "Funding that shift first guarantees nothing; it does, however, make the pilot's promise testable within a year" should be two sentences. The voice is optimized for subvocalization: punctuation is pacing, and the reader needs the full stop to breathe. The semicolon survives only when one side is short. Gate 3, punctuation profile, and Do/Don't updated.

## 1.8.0 — 2026-09-19

Source: Ahmed's consolidated list of what AI writing does badly, translated into the style guide (v0.7) and folded in here.

- **Register check: never too knowing.** The umbrella over the v1.4.0/v1.5.2 persona bans — the tell is the stance (cheeky, cool, ahead of the reader), not any single device. New Gate 3 rule and Do/Don't entry: write alongside the reader, not above them; when a sentence's charm comes from being clever rather than right, rewrite it.
- **Recipe-advice ban.** AI advice makes outcomes sound deterministic and easy — "Do this, then that happens. Do this and this, then that and that." New Gate 3 rule: any [action] → [promised outcome] sentence gets the friction test (name the cost, timeline, or contingency inside the advice). Applies to dedicated advice sections too. Do/Don't updated.
- **Connectives-as-breath confirmed.** Ahmed's diagnosis ("words that add tokens so might seem useless but give readers a second to breathe when they subvocalize") restates and hardens the v1.5.0 connective check — no rule change, the Gate 1 scan stands.

## 1.7.0 — 2026-09-19

Source: Ahmed on the v1.6.0 revised daily test closer ("I don't know what it is about that last sentence that doesn't make any sense") in #ai-writing-voice.

- **Literal-read rule for payload sentences, especially closers.** "For now, the value leaks out between code written and code trusted, and most budgets have not noticed" failed three ways: a container metaphor ("leaks out") stretched over a gap ("between"), a personified inanimate (budgets cannot notice), and two clauses stapled with "and" carrying no stated relationship. New Gate 3 rule: one metaphor per sentence, actors that can perform their verbs, and the second clause must be the consequence of the first — the fix is plainness, not a better metaphor ("almost no budget has a line for the difference"). Gate 3 and Do/Don't updated.

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
