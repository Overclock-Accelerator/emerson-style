---
name: emerson-style
description: "Use when Ahmed asks for copy in 'Emerson Style'."
version: 1.4.0
author: Emerson (extracted 2026-09-19 from PwC/Strategy& insight articles)
license: internal-use
metadata:
  hermes:
    tags: [writing, voice, copywriting, executive, consulting]
    category: creative
    related_skills: [voice-extraction, humanizer]
---

# Emerson Style

Ahmed's named premium voice: polished executive-consulting register built on the extracted PwC / Strategy& thought-leadership voice, with anti-AI gates enforced before delivery. Formerly called "elevated voice" — renamed Emerson Style 2026-09-19.

## When to use this skill

Load this skill when Ahmed asks for copy "in Emerson Style" (or "the Emerson Style"). This is a named, always-available voice — distinct from asking to "use the wiki voice" or another extracted profile, which routes to `voice-extraction`.

## Source note

Foundation: PwC / Strategy& thought-leadership, extracted 2026-09-19 from 4 insight pages (strategyand.pwc.com AI-and-technology POV, pwc.com "New Equation" strategy, PwC Leadership Agenda agentic-AI article, PwC US AI Agent Survey). No documented house style guide exists; house exceptions below are observed from samples, not official. The full extraction lives at `workspace/voice-profiles/pwc.md` (raw samples: `workspace/voice-samples/pwc-2026-09-19.md`), but this skill is self-contained and works without those files.

## Versioning

This skill is versioned and tracked in the public `emerson-style` repo (Overclock-Accelerator org on GitHub). Every material change bumps the version and gets a CHANGELOG entry. **Always state the version in the delivery note** (e.g. "Emerson Style v1.1.0") so Ahmed can compare output across versions.

## Workflow

1. **Draft against the profile below.** Read the calibration passages first — they are the few-shot payload. Patterns beat adjectives.
2. **Gate 1 — Rhythm.** Split the draft into sentences with a script. Target: mean 14–16 words, with the signature long-evidence/short-verdict pairing (a 20–40-word analytical sentence followed by a qualified verdict of 6–14 words — never a bare pronouncement; see Gate 3). If the draft is metronomic, rewrite at least two sentences into that pairing. **Overcorrection check (added v1.2.0):** if more than ~30% of sentences are under 8 words, the draft has drifted into punchy-social staccato — that is NOT this voice. Rebuild with long analytical sentences carrying the evidence; the short verdicts only work as punctuation against them. Every paragraph or two needs at least one 20–40-word sentence. **Format scoping (added v1.3.0):** the 14–16 mean applies to paragraph prose. For standalone numbered sentences with mid-sentence attribution ("in our survey of 15,000…"), attribution adds 4–6 words per sentence; a mean up to ~18 is acceptable provided the median stays near 14 and the long/short pairing survives.
3. **Gate 2 — AI-tell scan.** Search the draft for: delve, leverage, unlock, harness, seamless, innovative, transformative, landscape, utilize, game-changer, "in today's", "It's not X, it's Y" pivots, formal openers (Furthermore/Moreover/Therefore), meta-commentary ("In this article"), vague upbeat endings ("the future looks bright"). Fix every hit. (PwC marketers use "unlock"/"harness" in headlines; that license does not extend to insight prose.)
4. **Gate 3 — Structural AI-tell scan (density and argument shape).** Word-level bans are not enough — the AI-ness of a draft usually lives in structure. **These budgets are caps, not targets (v1.2.0): the devices below are signature moves of this voice. Budget them, do not eliminate them — a draft with zero rhetorical texture and all-short sentences has been stripped, not fixed. Run Gate 3 first, then re-run Gate 1 to confirm the rhythm survived.** Check and fix:
   - **Colon budget: ≤1 per paragraph, ≤2 per piece.** Colons are this voice's weakest tic — every "The pitch is X:" and "The result is Y:" is a claim announcing itself. Rewrite as two sentences or a comma splice that earns its place.
   - **Rhetorical-question device: ≤1 per piece, never two in one piece.** "A potential pitfall?" is a house move, but one per piece is a signature and two is a formula.
   - **Verdict-sentence pairing: ≤1 per paragraph, ≤2 per piece (v1.3.0).** The long-evidence/short-verdict move is a signature, not a skeleton. If three sentences in a row are set up as punchlines, flatten two of them — and count across the whole piece: three short verdicts in ten sentences reads as a formula even when each obeys the per-paragraph cap. **Qualified, never bare (v1.4.0, Ahmed):** every standalone verdict carries a qualifier or subordinate clause — "Adoption, however, is often the easy part.," not "Adoption is the easy part." Useful qualifiers: however, often, in practice, at least, for now, on its own. A bare two-to-five-word verdict poses as a casual aside; that pose is the AI tell. Exception: the fragment answer inside the rhetorical-question device stays ("A potential pitfall? Settling for too little."), because the question carries the setup.
   - **Evidence mix: at most one attributed survey per piece (v1.3.0).** Anchor on a single survey; every further evidence point should be a named company, a dated decision, or an observable fact. Two surveys stacked reads as report aggregation, not a point of view.
   - **Ban the negative-reveal opener** ("A new class of X is entering…, and it does not Y"). State the subject's claim directly instead.
   - **Ban in-line justification**: "which is exactly why," "the result is a… that," "which is precisely." State the fact; let the implication sit. Trust the reader.
   - **Not-X-but-Y pivots are banned by structure, not string**: "not X, it's Y," "X rather than Y," "less like X and more like Y" all count. ≤1 per piece, any phrasing.
   - **Three-item escalating lists**: cut the third item if it's there for rhythm. Two specifics beat three.
   - **Loose-thread rule**: real analysis leaves something unresolved. Vendor numbers get doubt carried in the sentence ("vendor-reported, unverified"); one question or implication may stay open at the end.
   - **The closer must not announce its own insight** ("For leaders, the shift is strategic rather than technical:"). End on a sharp observation, not a summary of what the piece meant — and never on an imperative addressed to the reader (see the advice-register rule).
   - **Ban the advice-register shift (v1.4.0, Ahmed).** The voice is impersonal exposition: it observes, weighs, and points — it does not advise the reader. A reader-directed imperative ("Fund the review layer as deliberately as you funded the models") shifts into helpful-assistant register, and that shift is an AI giveaway. State the imbalance and let the implication sit: "The review layer, not the model, is where the productivity leaks out." Imperatives survive only inside a dedicated, labeled advice section with bolded leads ("Focus on people."), never in analytical prose.
   - **Ban the in-group tell (v1.4.0, Ahmed).** Constructions that invite the reader into a hip club of winners — "The teams getting the most from agents…," "the companies winning at AI" — read as casual insider language ("it's cool to be in the know"), not executive consulting. Name the practice and its evidence directly instead: "Teams that write more specifications, and that treat context as a discipline with its own budget, report the strongest results." The general principle across all three v1.4.0 rules: the voice never performs a persona — not the casual aside, not the helpful assistant, not the hip insider.
5. **Gate 4 — Do/Don't checklist.** Walk the Do/Don't list below line by line against the draft.
6. **Gate 5 — Vale (if installed).** Run `vale` with the Emerson style pack on the file; fix errors, weigh warnings.
7. **Deliver with a note** naming the style and version ("Emerson Style vX.Y.Z") and flagging any spots that need real client data (percentages, survey counts) — never invent figures.

## The profile

### Rhythm
- Sentence length (measured, n=80): mean 15.3 words, median 14. 28% under 10 words, 45% at 10–19, 21% at 20–29, 6% at 30+. Range 2–46.
- Signature move: a long analytical sentence (20–40 words, often carrying survey data or a causal chain) followed by a short verdict sentence. **The verdict is qualified, never bare (v1.4.0, Ahmed):** a two-to-five-word pronouncement ("Adoption is the easy part.") poses as a casual aside and is a reliable AI tell; carry a qualifier or subordinate clause ("Adoption, however, is often the easy part."). Verdicts run 6–14 words. The bare fragment survives only as the answer inside the rhetorical-question device ("A potential pitfall? Settling for too little.") — the question carries the setup.
- Paragraph length: 2–4 sentences. Headers are declarative full sentences ("AI becomes an enterprise capability."), not topic labels.
- Cadence: claim → evidence (percentages, survey counts) → implication for leaders. The short sentence lands the implication.

### Openers
- Direct claims with the subject up front: "AI is changing the role of technology in enterprise performance."
- Time-framed resets: "Today, they're delivering real results."
- Numbered-shift structure ("Four shifts are changing how technology creates and scales value."), each shift named as a sentence.
- Rhetorical-question volleys to dismiss objections: "Cybersecurity concerns? AI agents can be made secure. Cost? A well-designed implementation can pay for itself."

### Word choice
- Register: executive-consultative — plain sentences, boardroom vocabulary.
- Signature words: trust, sustained outcomes, measurable value/results/impact, "how work gets done," enterprise capability, reinvention/reimagine, "sharper choices," governance, responsible AI, scale (as verb), "in concert," virtuous circle.
- Signature constructions: "not X, but Y" inversions ("strategic choices, not disconnected investments"); "X becomes part of Y" ("Trust becomes part of performance"); paired imperatives in advice bullets ("Focus on people." "Orchestrate and integrate.").
- Era framing: name the current moment as an era ("The New Equation," "an AI-powered, platform-led era") and position the reader's decision inside it.
- Avoid: hype adjectives (revolutionary, game-changing, cutting-edge), slang, winner-club casualisms ("teams getting the most from X," "companies winning at Y"), first-person singular, jokes.

### Punctuation and mechanics
- Heavy em-dash use for the pivot clause ("people—including senior leaders—are holding AI agents back").
- Rhetorical question + immediate answer is a repeated device ("A potential pitfall? Settling for too little.").
- Semicolons rare; commas carry the long sentences. Percentages and survey figures embedded mid-sentence, always attributed ("Of the 300 senior executives in our May 2025 survey, 88% say…").
- Contractions used freely (doesn't, they're, it's) — confident, not stiff.
- Sentence-case headers; numbered shifts and bulleted advice with bolded two-or-three-word leads.

### Attitude
- Stance toward reader: impersonal exposition addressed to CEOs and boards — the voice observes and weighs; it does not advise (v1.4.0, Ahmed). Second person appears only inside dedicated advice sections, never in analytical prose. Never chummy.
- Humor: none.
- Claims: assert, then cite the firm's own research. Skeptical of hype in a controlled way — name the pitfall, dismiss the excuse, redirect to the opportunity. Governance and trust are performance issues, not compliance chores.

### Structural habits
- Opens with a one-line declarative headline and a point-of-view framing; long-form pieces close with a dedicated advice section (three bolded imperatives is a house pattern), while standalone pieces close on a sharp observation — never a reader-directed imperative (v1.4.0).
- Body arc: era shift → evidence → pitfall → implication (a dedicated advice section may follow in long-form; the analytical arc itself ends on the implication). Transitions are short bridge sentences ("That disconnect points to a deeper truth.").

### Do / Don't
- DO pair every long evidence sentence with a short qualified verdict sentence.
- DO frame technology as a strategic choice tied to measurable outcomes and trust, never capability for its own sake.
- DO name the current era and position the reader's decision inside it.
- DO use the rhetorical question / short answer device to clear objections.
- DO end long-form pieces with a dedicated advice section: two or three bolded imperatives a leader can act on. Standalone pieces end on an observation instead.
- DON'T use hype adjectives or AI-slop verbs (delve, leverage, unlock, harness, utilize).
- DON'T stack devices: ≤1 colon per paragraph, ≤1 rhetorical question per piece, ≤1 verdict pairing per paragraph and ≤2 per piece. Density is the tell (Ahmed, 2026-09-19).
- DON'T write bare pithy verdicts ("Adoption is the easy part.") that pose as casual asides — qualify the verdict ("Adoption, however, is often the easy part."). The unqualified punchline is an AI giveaway (Ahmed, 2026-09-19).
- DON'T close with an imperative addressed to the reader ("Fund the review layer…") — the shift from impersonal exposition to helpful-assistant advice is an AI giveaway. Close on the observation; let the reader draw the prescription (Ahmed, 2026-09-19).
- DON'T frame evidence through a hip in-group ("The teams getting the most from agents…") — casual insider language is an AI giveaway. Name the practice and its evidence directly (Ahmed, 2026-09-19).
- DON'T stack surveys: one attributed survey per piece, then switch to named cases and observable facts. Two surveys in one piece reads as aggregation (self-assessment, 2026-09-19).
- DON'T overcorrect the other way: the budgets cap signature devices, they don't ban them. All-short sentences and zero texture is staccato slop, not Emerson Style (Ahmed, 2026-09-19).
- DON'T open with a negative reveal or close by announcing the insight; the ending observes, it doesn't summarize or prescribe.
- DON'T celebrate adoption without warning about settling for too little — the voice always pairs momentum with the gap.
- DON'T write topic-label headers ("Introduction," "Background"); headers are declarative sentences.
- DON'T joke, hedge with "might perhaps," or speak in first person singular; the voice is the firm ("we," "our survey").

## Calibration passages (few-shot payload — verbatim from source)

> "As AI, cloud, and software continue to converge, value will not come from adding more technology to the business. It will come from making sharper choices about where intelligence belongs, where platforms can scale, and how investment can create measurable performance."

> "We believe that the successful organisations of the future will be the ones that create a virtuous circle between building trust and delivering sustained outcomes."

> "A potential pitfall? Settling for too little. Broad adoption doesn't necessarily mean deep impact."

> "When it comes to AI agents, technology isn't the barrier, mindsets are. And that's exactly where the opportunity lies."

> "As AI and data become central to performance, cybersecurity, resilience, and responsible AI become central to trust. Without trust, intelligent systems cannot scale."
