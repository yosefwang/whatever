---
description: 'Use this skill when writing, rewriting, or polishing policy reports,
  country profiles, economic surveys, or analytical text in OECD official publication
  style. Triggers include: "OECD style", "像OECD那样写", "改写为OECD风格", "policy brief",
  "rewrite in OECD style", "polish", "润色", "改写段落", "篇章改写", or any request to produce
  institutional policy prose.'
name: oecd-writing-style
---


# OECD Writing Style Guide

Transform any text into OECD institutional prose — or generate it from scratch. This guide covers diction, syntax, structure, logic, and a rewrite protocol drawn from 740 OECD publications (development cooperation, economic surveys, carbon pricing, health profiles, circular economy, tax governance, regional policy).

## How to read this guide (principles first, catalog second)

The guide is built in two layers, and reading order matters:

1. **The operating layer** — *Step 0 / Step 0b (genre dials)*, *the core skeleton*, and **the Generative Core (ten moves)**. This is what you internalise and write from. It is small on purpose, and it is what makes the style generalise to genres, topics, and sentences not in the catalog.
2. **The evidence-and-lookup layer** — the 60-plus sentence templates (T-numbers), the fingerprints (A–X), the logic patterns (A–P), and the 40-plus genre profiles in §9. These are *surface realisations* of the ten moves, recorded as proof and as a reference palette. **Consult them; do not try to satisfy them all.** Applying the whole catalog uniformly is the single most common way to make OECD-style output read as AI (see move M8).

If you only have attention for one section, read **the Generative Core**. The rest exists to deepen and verify it.

*Maintenance note for editors of this skill:* the file has grown by accumulation across sampling rounds and is now very large. The highest-leverage next step is to **split it** — keep the operating layer (Step 0 → Generative Core → §10 self-check → §7/§8 worked examples) as the loaded `SKILL.md`, and move the evidence catalog (T-templates, fingerprints, §9 profiles) into a referenced file loaded only when a specific genre or surface form must be confirmed. Generalisation improves when the operating layer is not buried under the catalog.

## Modes of Operation

- **Generate mode**: User provides topic/outline → produce OECD-style text.
- **Rewrite mode**: User provides existing text → rewrite in OECD style while preserving factual content. Work the ten moves (Generative Core) over the draft first — subjects, rhythm, concession, logic-bridges — then use the catalog to confirm surface forms. Do not fabricate data.

## Step 0: Identify the genre before applying any rule

OECD output is **not a single style**. It is a family of registers that share a small **core skeleton** and diverge on the rest. Before applying any specific rule from this guide, identify the target genre. Mismatched application is the single largest source of "AI-feel" in OECD-style writing — for example, injecting "albeit" / "inter alia" / heavy citations into a Policy Primer, or stripping the warm "considerations" tone out of an Education Country Review and replacing it with dry Survey prose.

**Decision tree**:
1. Is the user asking for a **short, accessible explainer with bullets and "What is X?" headings**? → Policy Primer / Brief (§9.6)
2. Is the user asking for **a research paper with we-voice, methodology, JEL codes**? → Working Paper (§9.8)
3. Is the user asking for **dense fiscal / structural analysis of a country with chapter-length depth**? → Economic Survey chapter (§9.1)
4. Is the user asking for a **peer-review evaluation, often numbered paragraphs, "the lead examiners commend / note"**? → Peer Review (§9.5)
5. Is the user asking for **a country snapshot built around indicators with conceptual openings**? → Country Profile / GaaG (§9.3)
6. Is the user asking for **a longer review with chapters and stakeholder framing on education / health / skills**? → Country Review (§9.7)
7. Is the user asking for **a 1-2 page conclusion-block document with gerund subtitles**? → Executive Summary (§9.2)
8. Is the user asking for an **ODA / DAC profile**? → Development Cooperation Profile (§9.4)

**If the genre is unclear, ask.** Do not default to Economic Survey style — that is the densest register and over-applies fingerprints that other genres do not use.

## Step 0b: The genre-dial model (use this for any genre, listed or not)

The decision tree above and the 40-plus profiles in §9 are **presets**. Underneath them, every OECD genre is a setting of six dials plus two toggles. The presets cover the genres sampled so far; the dials cover the ones that are not. **When a request does not map cleanly onto a listed genre, do not force-fit it and do not fall back to Economic Survey — read the six dials off the request itself and write from those.** This is what lets the skill generalise to genres and topics it has never seen.

| Dial | Low end ←—————→ High end | How to read it from the request |
|---|---|---|
| **D1 Register** | warm / accessible ←→ dry / impersonal | audience of citizens and ministers → warmer; audience of technical peers → drier |
| **D2 Citation density** | none ←→ one per 2–3 sentences | evidentiary genre (Survey, Peer Review, Working Paper) → high; brief or primer → none |
| **D3 Recommendation force** | "there is scope to" ←→ "calls on / must" | addressing a sovereign government → soft; a treaty signatory in breach → firm (see M4) |
| **D4 Texture** | continuous analytical prose ←→ bullets / itemised lists | reference / scoreboard / roadmap → itemised; argument / analysis → prose |
| **D5 Data treatment** | data-light (data illustrates) ←→ data-dense (data *is* the deliverable) | "explain / assess" → light; "report / track / compare" → dense, with `Note:` blocks |
| **D6 Opening convention** | pick one: state-of-play fact · "set to" projection · abstract-concept-then-data · data-first · definitional · threat / geography | see §2.5 and the target genre in §9 |

Two toggles sit on top of the dials: **Voice** (third-person institutional by default; first-person "we" only in Working Papers and study Prefaces) and **Warmth vocabulary** (only Education / Health Country Reviews and Primers license "thrive", "those who need them most").

**Worked dial-reads (note how each lands on a genre without being told the genre):**
- *A carbon-border-tax explainer for the general public* → D1 warm, D2 none, D3 soft, D4 bullets, D5 light, D6 definitional / question-headings → this is a **Policy Primer**, even though "carbon border tax" was never a sampled topic.
- *A fisheries-subsidy assessment for trade negotiators* → D1 dry, D2 medium, D3 firm-but-hedged, D4 prose plus bullets, D5 medium, D6 "What's the issue?" → **Trade Brief**.
- *An unsampled subject inside a sampled genre* (e.g. a quantum-computing Economic Survey chapter) → keep every Economic Survey dial setting; change only the topic vocabulary.

The dials are the part that generalises. The §9 profiles are convenience presets for the most common dial combinations — consult them to confirm surface conventions, not to decide whether a genre "qualifies".

## What is universal across OECD genres (the core skeleton)

These features hold across **all** OECD output, regardless of genre — verified empirically across 18 documents spanning 8+ OECD publication types (Economic Survey, Country Review, Policy Primer, Working Paper, Peer Review, Environmental Performance, Water Governance, Steel Outlook, Supply Chain, Tokenisation, Digital Policy, Fisheries, Pension Notes). They are the irreducible OECD voice. **Apply all 10 of these before considering any genre-specific fingerprint below.**

1. **Concrete named subjects** — countries, agencies, regulators, sectors as actors (not "stakeholders" in the abstract). See §1.5.
2. **Quantification anchors comparison** — every comparative claim has a benchmark (an OECD average, a peer country, a prior year, a target). See §6.
3. **"such as" / "including" example unfolding** — every general claim is followed by 2-4 concrete examples. The single most cross-genre-stable fingerprint.
4. **Repeated technical terms** rather than synonym substitution — "CLL" stays "CLL", country names repeat, key concepts do not get decorative replacement. See §1.9-G.
5. **Hedged projections, firm history** — futures use "is set to / is expected to / is projected to"; past facts are reported flat. See §1.6.
6. **Graded recommendation modals** — "should / would help / could / there is scope to / could consider" — calibrated to firmness, not interchangeable. See §2.12.
7. **No meta-discourse** — never "this section examines", "two strands of debate", "as discussed above". See §1.8-A.
8. **No subjective evaluation** — never "the data are striking / alarming / remarkable". OECD lets numbers speak.
9. **No journalistic colour** — no metaphors, no rhetorical questions (except as Primer headings), no aspirational closes.
10. **Imperfect parallelism allowed** — clean parallel structure is an AI signal; mild grammatical drift in lists is human.

## The Generative Core: ten moves behind every surface pattern

**This is the operating layer of the skill. Everything that follows — the 60-plus sentence templates (T-numbers), the fingerprints (A–X), the logic patterns (A–P), the 40-plus genre profiles in §9 — is *evidence and lookup*: surface realisations of the ten moves below.** A writer who internalises the ten moves can produce OECD prose in a genre never sampled and in fresh wording. A writer who only pattern-matches the templates reproduces them mechanically — and mechanical reproduction is itself the loudest AI tell. So: **apply the moves; consult the catalog only to confirm a specific surface form.**

Each move is a *judgement*, not a phrase. The surface marker is interchangeable; the move is not. For each move below: the deep rule, the variable surface markers, the catalog items it subsumes, and the AI-default-versus-OECD contrast.

**M1 — Anchor every number to a comparator.**
A bare figure has no meaning; its meaning lives in what it is measured against. Every number carries at least one of: an OECD or peer average, a peer country, a prior year, a target, or a denominator.
*Surface:* "above the OECD average of 39%", "compared with 2022", "in real terms", "26th of 39", "8 in 10 (78%)".
*Subsumes:* T7, T29, T39; logic P; §6; fingerprint U.
*AI default* reports the number alone; *OECD* never lets a number stand without its frame.

**M2 — Unfold every generalisation into 2–4 named examples.**
The most cross-genre-stable habit in all of OECD prose: a general claim is immediately followed by concrete instances.
*Surface:* "such as" (in-line), "including", "e.g." (parenthetical), "for example".
*Subsumes:* skeleton #3; fingerprint B.
*AI default* states the generalisation and moves on; *OECD* compulsively exemplifies.

**M3 — Concede, then qualify (visible two-sidedness).**
Institutional credibility comes from never being wholly positive or wholly negative: state the progress, and in the same breath name the residual gap. This is the single most universal OECD *sentence*.
*Surface (one move, many markers):* "X has improved, **but** Y remains"; "**While** X, Y"; "**Despite** X, Y"; "**On the other hand**…"; "…**albeit** at a slower rate"; "**Nevertheless**, the lead examiners note…".
*Subsumes:* T1, T1b–d, T3, T18, T34, T35; logic L/M/N; the peer-review concession structure.
*AI default* picks a side; *OECD* holds both. **Deploy at least once per analytical paragraph, and pick a different marker each time** — uniform "but… but… but…" is itself an AI tell (see M8).

**M4 — Grade the recommendation force deliberately.**
Recommendation strength sits on a ladder and is chosen to match the evidence and the addressee — softer to a sovereign government, firmer to a treaty signatory in breach. The modals are not interchangeable.
*Ladder (soft → firm):* there is scope / room to → could consider → is encouraged to → would help / benefit from → should → calls on → it is incumbent upon → must.
*Subsumes:* T2, T8, T16, T19–21, T38; §2.12; the recommendation-verb sets.
*AI default* repeats one modal ("should… should…"); *OECD* varies the modal to signal varying confidence (T38) and reserves "must" for treaty obligations.

**M5 — Carry the logic in the sentences; never narrate the structure.**
The argument moves diagnosis → inference → recommendation, but the joints are made of *content*, not signposts. No "this section examines", "two strands of debate", "as discussed above".
*Surface:* "This **suggests / reflects / underscores**…" (demonstrative + analytical verb); "**On this basis**…"; "**Against this background**…"; "**Going forward**…"; a demonstrative pronoun pointing back at the whole prior claim ("This differentiation limits…").
*Subsumes:* T11, T13, T15, T30–33; logic K/O; skeleton #7.
*AI default* uses "Therefore / Consequently" plus meta-discourse; *OECD* makes the evidence sentence itself the bridge.

**M6 — Hedge the future; report the past flat.**
Epistemic honesty is asymmetric in time: projections are always hedged, established facts never are.
*Surface:* future → "is set to / is expected to / is projected to / could / which, if realised, will"; past → plain past tense, no "approximately" unless the datum is genuinely uncertain; "not yet" marks in-progress-but-incomplete.
*Subsumes:* skeleton #5; T5, T12, T27, T28; §1.6; §2.7.
*AI default* hedges everything or nothing; *OECD* hedges precisely where the uncertainty actually lives.

**M7 — Concrete actors as subjects; repeat key terms; define institutions by purpose.**
Countries, agencies, regulators, and named instruments are the grammatical subjects — not "stakeholders" or abstract nouns. Technical terms and country names are *repeated verbatim*, never synonym-swapped. Institutions are introduced by what they are *for*.
*Surface:* "Portugal… Portugal… Portugal" (never "the southern European economy"); "CLL… CLL… CLL"; "The Committee **was established to**…"; numbered "**four pillars**"; chapter heading "Tertiary education: **Creating a more attractive system**" (the argument, not a topic label).
*Subsumes:* skeleton #1/#4; §1.4, §1.5, §2.3; T6, the T7 heading pattern, T14, T24; fingerprint G.
*AI default* uses abstract-noun subjects and aggressive synonym variation; *OECD* uses concrete subjects and lexical repetition. (Synonym-swapping is one of the loudest AI tells, so M7 is also an anti-AI move.)

**M8 — Vary the rhythm and leave controlled roughness.**
Uniformity reads as machine; deliberate unevenness reads as human. This is the move that produces 人味 (the human texture).
*Surface:* mix sentence lengths (at least one ≤12-word sentence and one 35+-word sentence per paragraph; never three similar-length sentences in a row); leave one preposition-stacked long sentence un-split; break parallelism slightly (let a clause sit among noun phrases); end some paragraphs on a flat fact rather than a synthesis; leave some implications unstated.
*Subsumes:* §2.2; skeleton #10; fingerprints D/F/I/J/L; the "unresolved argument" closer.
*AI default* is smooth, uniform, every argument closed; *OECD* is textured, occasionally rough, with some arguments left for the reader to finish.

**M9 — Strip colour, meta, and undata'd evaluation (the restraint move).**
Remove the narrator. No metaphors, no rhetorical questions (except Primer headings), no aspirational closes, no "striking / alarming / remarkable", no "it is important to note", no universal-truth openings.
*Subsumes:* skeleton #8/#9; §1.8; the §10 dryness test.
*AI default* is persuasive, warm, and self-narrating; *OECD* is drier than journalism — trust the data, delete the adjective.

**M10 — Ground claims in evidence and precedent, and admit the limits.**
Attach a source to empirical claims at the genre-appropriate density (D2); ground arguments in past experience rather than abstract reasoning; and state plainly what the analysis does *not* cover.
*Surface:* "(OECD, 2024)" repeated within a paragraph; "**Past experience has shown that**…"; "This **could simply be**…" (the boring alternative); "X **does not automatically equate to** Y"; "It **must be stressed that** the indicator measures de jure policy, not enforcement"; "**beyond the scope of this paper**".
*Subsumes:* fingerprints A, M, N, S, W; logic F.
*AI default* offers unsourced confidence and no self-limitation; *OECD* is sourced, precedent-anchored, and honest about its own blind spots.

**How the ten moves cover the six aims of this skill:** 布局谋篇 (composition) → M5, M7, and the D4 texture dial; 遣词造句 (diction and sentence-craft) → M2, M6, M7, M9; 逻辑思考 (logic) → M3, M5; 清晰表达 (clarity) → M1, M7, M9; 数字、数据的叙述 (narrating data) → M1; 人味 and anti-AI → M7, M8, M9, M10.

**The two failure modes the moves are built to prevent:**
1. *Thesaurus rewriting* — upgrading vocabulary while leaving abstract subjects, uniform rhythm, and concept-scaffolding openings intact (see the Failure Case Study, §8). M7 + M8 + M5 fix this; word-swaps alone never do.
2. *Checklist mechanicalness* — applying all the templates and fingerprint boxes uniformly, which manufactures the very smoothness that flags as AI. M8 is the deliberate antidote: treat the catalog as a palette to draw from unevenly, not a checklist to satisfy completely.

### Cross-genre sentence patterns — the evidence layer (lookup, not checklist)

The patterns below (T-numbers) are the **surface evidence** for the moves above: each T-pattern is one realisation of one move (the subsumption is mapped in each move). Use them to confirm a specific surface form or to widen your repertoire of markers — **not** as a list to satisfy in full. Reproducing many of them mechanically in one passage recreates the AI smoothness that M8 exists to break.

These syntactic patterns have been verified across Economic Surveys, Environmental Performance Reviews, Education Reviews, Water Governance reports, Health System reports, Policy Primers, and Working Papers. They are the sentence-level "accent" shared across the OECD family.

**T1. The "affirmative + but" balanced-concession sentence** — the most universal OECD sentence structure. It states a positive development, then immediately introduces a remaining challenge or qualifier. AI tends to be fully positive or fully negative; OECD is always partially both.

> "Japan has intensified efforts to ease pressures on biodiversity, **but** better policy alignment is needed."
> "Romania is taking measures to develop its education data infrastructure, **but** capacity and resources to analyse and report data need strengthening."
> "Spending on prevention amounts to less than 2% of health spending **but** drives up costs without promoting better health outcomes."
> "Portugal's income has continued to converge, **but** at a slower rate."

**The key grammar**: [Country / Subject] + [positive verb phrase] + `,` **but** + [remaining gap / qualifier].

This is **not** the same as "although X, Y". The OECD "but" is **clause-level**, not subordinating. It creates a stop-and-go rhythm that reads as balanced institutional assessment.

**Deploy 2-3 times per paragraph in Country Reviews and Environmental Performance Reviews; at least once per paragraph in Economic Survey analytical prose.**

**T1b. The "not X, but rather Y" negative-contrast structure** — OECD uses "but rather" far more than "but instead" or "but instead of". It defines what something **is not** by immediately stating what it **is**.

> "The principles **are not** an attempt to harmonise global law, **but rather** to provide a common framework."
> "The system **is not** designed to eliminate risk, **but rather** to manage it within acceptable limits."
> "The approach **is not limited to** onboarding, **but** importantly **involves** the safeguarding of the asset."

**T1c. The "not only X, but also Y" dual-function sentence** — OECD uses "not only ... but also" to make a dual-function claim: X is useful, and X also serves a second purpose.

> "These objectives **not only** drive change across most sectors, **but also** raise potential risks."
> "The model **not only** incorporates trade concentrations, **but also** allows modelling of behavioural responses."

**T1d. The "X is not [only] Y, but [also] Z"** — the most common way OECD presents a thing's dual nature, especially in risk-opportunity framing.

> "Quantum technologies hold great promise **but** also present significant risks."
> "The reforms aim to improve expenditure quality **but** require complementary measures to deliver results."

**T2. The "There is scope / room / considerable opportunity to…" recommendation frame** — the OECD way to say "this is needed" without sounding prescriptive. More hedged than "should", less conditional than "would help". Used in country assessments where OECD offers guidance rather than instruction.

> "**There is scope to** enhance coherence and cost effectiveness of environmental policies."
> "**There is room to** strengthen institutional capacity at subnational level."
> "**There is considerable opportunity to** provide more consistent price signals."
> "**There is scope to** develop whole-of-government approaches to water governance."

**The key grammar**: "There is [scope | room | considerable opportunity | potential] to [verb] [area]."

This construction appears in **all** peer-review and assessment genres (EPR, Education Review, Water Governance, Health). It is the OECD way of identifying gaps without naming who is at fault.

**T3. The "Where X, Y" conditional clause** — OECD uses "where" in the institutional sense ("in settings where"), not in the geographic sense. This is a sentence opener that narrows from the general to the specific.

> "**Where** subnational bond markets are small, yields can respond more to common risk appetite."
> "**Where** labour market rigidities are pronounced, firms may delay adoption."
> "**Where** local governments retain most of the new tax base, we might expect a stronger immediate improvement."

**T4. The "in order to" purpose clause** — OECD uses "in order to" at higher frequency than other prose. It makes the institutional purpose explicit.

> "**In order to** improve dialogue and communication, Hungary established an Inter-Ministerial Committee."
> "**In order to** address these challenges, the government introduced a new monitoring framework."

**T5. "comparable" / "appropriate" / "adequate" as institutional adjectives** — OECD prose uses these adjectives to embed a standard of sufficiency without explicit judgment.

> "at **comparable** subnational geographies"
> "at the **appropriate** scale"
> "with **adequate** capacity"
> "ensuring **adequate** price signals"

**T6. "is designed to / was established to" — functional-institutional grammar** — OECD frequently explains the *purpose* of an institution by naming it and appending its design function.

> "This series **is designed to** make available to a wider readership selected studies."
> "The HSPA framework **is structured around** outcomes, processes, inputs, and cross-cutting domain blocks."
> "The Inter-Ministerial Committee **was established to** enhance co-ordination."

**T7. Chapter heading pattern: "[Topic]: [Gerund-phrase-as-statement]"** — OECD report chapters consistently follow a colon-separated structure where the topic is followed by a gerund-phrase subtitle that functions as a complete statement about the topic, not a topic label.

> "**School education:** Giving every student a fair chance to succeed"
> "**Tertiary education:** Creating a more attractive, relevant and accessible system"
> "**Skills:** Building the workforce for a modernising economy"
> "**Water in Hungary:** Overview and trends"
> "**Towards** climate-resilient water governance in Hungary"

The gerund subtitle is the **executive-sentence headline** convention — it tells the reader what the chapter argues, not just what it covers. The pre-colon label names the domain; the post-colon phrase names the analytic claim.

When generating chapter headings, avoid generic topic-only headings ("Chapter 3: Education"). Always add the gerund subtitle that tells the reader the chapter's argument.

**T8. "should be [past participle]" — the OECD passive recommendation** — this is the standard way to express a recommendation without a named actor, which is appropriate for institutionally neutral language where OECD is not directing a specific government department.

> "Regulations **should be** strengthened."
> "Price signals **should be** provided in a more consistent manner."
> "Policy coherence **should be** enhanced."
> "Workforce capacity **should be** adapted to the complexity of challenges."

Verified across Economic Surveys (56 per report), Education Reviews (34), Environmental Performance Reviews (35), Water Governance (23). This passive-recommendation voice is far more universal than the active "Argentina should" (which is specific to Peer Review).

**T9. "X remains [adjective]" — the OECD state-of-persistence verb** — "remains" is the most universal verb in OECD analytical prose. It signals "the situation has not changed", implicitly arguing that change is needed. More frequent than "continues to be" or "is still".

> "Romania **remains** low on many learning outcomes."
> "Growth **remains** subdued."
> "Implementation **remains** uneven."
> "The situation **remains** fragile."
> "Access to healthcare **remains** a challenge."

Verified: appears 27–230 times per report across ALL genres sampled (Environmental Performance 88, Education Review 127, Economic Survey 230, Water Governance 29, Health System 27). This is the single most frequent analytical verb in the OECD family.

**T10. "has been [present participle] / have continued to [verb]" — present-perfect continuous as OECD's ongoing-action tense** — OECD uses present-perfect continuous ("has been promoting", "have continued to reform", "have stepped up") to describe actions still in progress. This tense is far more common in OECD prose than in other institutional writing.

> "Japan **has been** promoting a place-based approach."
> "Bulgaria's income **has continued to** converge."
> "Japan **has been** piloting local climate adaptation."
> "Romania **has been** expanding its education system."
> "Food inflation **has** accelerated, **continuing** its upward trend."

Verified: "has been" appears 21–122 times per report across ALL genres. This is the OECD author's default tense for describing a country's ongoing reform trajectory.

**T11. "On this basis / Taking this into consideration / Based on this" — the OECD recommendation-bridging phrase** — OECD transitions from diagnosis to recommendation using explicit logical-bridge phrases. These connectors make the argumentative structure visible: "I've shown you X → therefore I recommend Y."

> "**On this basis**, policymakers could consider developing a clear state ownership policy."
> "**Taking this into consideration**, strengthening board effectiveness will be key."
> "**Based on this**, embedding RBC systematically into SOE policy could be considered."
> "**Against this background**, the 2025 reform package was adopted."
> "**In light of** these findings, the government should strengthen disclosure requirements."

These are the OECD equivalents of "therefore" — but less abrupt and more institutional. AI defaults to "therefore" or "consequently"; OECD reaches for "On this basis" and "Taking this into consideration."

**T12. "X is not yet [adjective] / X has not yet [past participle]" — the OECD partial-progress hedge** — OECD uses "not yet" to indicate something is in progress but incomplete, which is softer than "has failed to" or "has not". This is the OECD way of acknowledging effort while still flagging a gap.

> "The government's sustainability priorities are **not yet translated** into a concise ownership policy."
> "Human rights due diligence is **not yet systematically built** into project cycles."
> "Requirements and supervision **remain** uneven across the portfolio."
> "Early-stage consultation is **not consistently disclosed**."

The grammar: [subject] + "is not yet" / "has not yet" / "is not consistently" + [past participle / adjective]. This is more common in assessment and review genres (EPR, Education Review, SOE Review, Health System) than in Economic Surveys.

**T13. "Going forward / Looking ahead" — the OECD forward-looking transition** — OECD uses "Going forward" to signal a shift from diagnosis to forward-looking recommendation. It is the companion to "On this basis" (which signals backward-looking logical bridge).

> "**Going forward**, policymakers could consider establishing a harmonised disclosure framework."
> "**Looking ahead**, inflation expectations have moved upwards."
> "**Going forward**, the key will be to translate these into concrete targets."

Use sparingly (once or twice per chapter); overuse reads as AI padding. OECD uses "Going forward" at section-break points, not mid-paragraph.

**T14. The "[number] pillars" framing device** — OECD policy reports frequently structure their analysis around a numbered set of pillars, dimensions, or benchmarks, introduced early and used as a reference framework throughout.

> "This paper assesses progress across **four pillars**: (i) the role of the state owner, (ii) the role of boards, (iii) disclosure and transparency, and (iv) responsible business conduct."
> "Luxembourg's HSPA framework consists of **12 domains** and **30 subdomains**."
> "The reforms are built on **three strands**: fiscal consolidation, structural reform, and institutional strengthening."

The numbered-pillar framework is a structural convention that signals OECD institutional analysis. AI tends to write about topics without establishing a numbered analytical framework; OECD always does.

**T15. Demonstrative-pronoun sentence openers ("This policy / This differentiation / This commitment")** — OECD prose frequently opens a new sentence with a demonstrative pronoun that refers back to the entire preceding argument. This creates a "chain-of-evidence" cohesion that AI rarely produces.

> "**This differentiation** limits the state's ability to exercise informed ownership oversight."
> "**This policy** should set minimum expectations for sustainability governance."
> "**This** would require SOEs to implement structured stakeholder engagement."

The pattern: [demonstrative noun] + [new claim about the referent]. This links diagnosis → consequence → recommendation in a chain without repeating the subject. AI defaults to "Therefore" or "As a result"; OECD uses the demonstrative pronoun as a bridge.

**T16. "policymakers could consider" — the OECD's most hedged recommendation frame** — in assessment genres, OECD rarely uses "should" directly. Instead, it uses "could consider + gerund/noun" as the softest possible recommendation.

> "Policymakers **could consider** developing a clear state ownership policy."
> "Governments **could consider** strengthening whistleblowing frameworks."
> "The government **could consider** establishing a mandatory disclosure framework."

This is softer than "should" (firm recommendation) and softer than "would help" (conditional benefit). It is the default in Peer Review, EPR, and Country Review genres. Economic Surveys use it less — they prefer "should" + named subject.

**T17. Country Review recommendation bullets: the OECD imperative-verb set** — in Country Review recommendations (Education, Health, Rural, etc.), bullet-point recommendations consistently begin with a closed set of imperative verbs. These are the verbs OECD authors reach for; AI defaults to a different set ("Consider", "Ensure", "Implement", "Improve").

**OECD Country Review imperative verbs (by frequency across Rural + Education Reviews):**
- **Strengthen** (40-58): "Strengthen regional assemblies as co-ordination hubs"
- **Develop** (27-37): "Develop State of Rural Ireland reports and dashboards"
- **Support** (10-27): "Support ability to engage in rural-sensitive planning"
- **Embed** (23): "Embed spatial skills intelligence within Ireland's skills architecture"
- **Build** (21): "Build differentiated rural labour market analysis"
- **Establish** (6-7): "Establish DRCDG as keeper of rural intelligence"
- **Introduce** (11): "Introduce dual-track monitoring"
- **Pilot** (34): "Pilot Rural Economic Development Zones"
- **Leverage** (15): "Leverage rural assets e.g. renewable energy"
- **Promote** (26): "Promote and encourage use of the six-way split"
- **Facilitate** (15): "Facilitate stronger linkages among programmes"
- **Empower** (5): "Empower local authorities with resources"
- **Clarify** (9): "Clarify overlapping mandates"
- **Address** (9): "Address interconnected barriers"
- **Shift** (6): "Shift to a differentiated monitoring model"
- **Rebalance** (6): "Rebalance volunteer dependence"
- **Adapt** (6): "Adapt compact growth to dispersed settlement networks"
- **Enhance** (5): "Enhance data systems through foresight intelligence"
- **Make** (10): "Make rural regions attractive places to live"

**AI-default verbs to avoid in Country Review recommendations** (these appear in AI output but are not the OECD recommendation register):
- "Consider" (too passive for bullet recommendations — use "could consider" in prose instead)
- "Ensure" (too bureaucratic; OECD uses "Strengthen" or "Embed")
- "Implement" (too operational; OECD uses "Establish" or "Introduce")
- "Improve" (too vague; OECD uses "Strengthen" or "Enhance")

**T18. "While [positive fact], [negative reality]" — the OECD concessive-clause opener** — a more formal alternative to "affirmative + but" (T1). Where T1 uses two independent clauses joined by "but", T18 uses a "While" subordinating clause to front-load the positive before the negative.

> "**While** rural education is improving overall, lifelong learning gaps persist between accessible and remote regions."
> "**While** a minority of Romanian students reach levels of excellence, many more leave school without mastering basic competencies."
> "**While** these plans are positive, there is scope to strengthen implementation."
> "**While** top performers achieve outcomes comparable to peers, nearly half perform below basic competency."

Verified: "While" sentence-openers appear 2–33 times per report across ALL genres. This is the OECD author's preferred concessive-clause structure when the concession is longer than a single clause.

**Grammar**: "While [longer positive clause], [longer negative/residual clause]." This creates a balanced institutional tone — acknowledging progress while sustaining critique. AI defaults to "Although" or "Despite"; OECD reaches for "While".

**T19. "is encouraged to / are encouraged to" — the OECD's polite-institutional recommendation frame** — this is the softest recommendation voice, used when OECD is not directing but advising. It appears frequently in Gender Equality reports, Education Reviews, and thematic reports where OECD recommends to institutions (EU Commission, Member States) rather than countries.

> "EU Member States **are encouraged to** act on these findings."
> "The European Commission **is encouraged to** monitor and enforce the Directive."
> "Countries **are encouraged to** continue to work together to develop harmonised taxonomies."

This is softer than "should" (firm) and softer than "could consider" (hedged). It is the OECD's polite-institutional voice — acknowledging sovereignty while recommending action.

**T20. "calls on [actor] to [verb]" — the OECD's most assertive recommendation verb** — used sparingly, when OECD wants to signal urgency without being directive.

> "This report **calls on** governments, social partners, civil society and the private sector **to** renew their commitments."
> "The OECD **calls on** Member States **to** strengthen implementation."

**T21. "It is incumbent upon [actor] to" — the OECD's formal-obligation frame** — used in concluding paragraphs to signal moral or institutional duty.

> "**It is incumbent upon** policy makers and societies at large **to** seize this moment."
> "**It is incumbent upon** governments **to** ensure that no one is left behind."

**T22. "Indeed," — the OECD sentence-opener for emphasis** — OECD uses "Indeed," at the start of a sentence to introduce supporting evidence or to strengthen a preceding claim. This is more common in thematic reports (Gender Equality, Education) than in Economic Surveys.

> "**Indeed,** on average across the EU, full-time working women earned 9% less than men."
> "**Indeed,** one of the biggest obstacles to further progress is women's and men's different roles in providing unpaid care."

**T23. "In a context of [X]" — the OECD situating-phrase** — used to frame the policy environment before making recommendations.

> "**In a context of** emerging political priorities – such as security and competition – gender equality should continue to be mainstreamed."
> "**In a context of** rapid technological change, governments must adapt their regulatory frameworks."

**T24. "To support [actor] in [gerund]" — the OECD purpose-infinitive for recommendations** — a specific purpose-clause pattern where the recommendation is framed as supporting an actor's capacity.

> "**To support** policy makers **in** transforming gender equality goals into outcomes, this report provides a conceptual framework."
> "**To support** countries **in** implementing these reforms, the OECD has developed guidance."

**T25. "hereafter" — the OECD abbreviation-introduction convention** — OECD uses "hereafter" in parenthetical form to introduce a shortened name for a long entity or country. This is a distinctive institutional convention that AI rarely produces.

> "the People's Republic of China (**hereafter** 'China')"
> "the Organisation for Economic Co-operation and Development (**hereafter** 'the OECD')"
> "the European Union (**hereafter** 'EU')"

**T26. "through [year]" — the OECD time-horizon frame** — OECD uses "through" to specify the end-date of a projection or trend, without needing "until" or "up to".

> "**Through 2030**, world demand is expected to grow by 0.7% per year."
> "**Through 2027**, excess capacity is expected to grow further."

**T27. "which, if realised, will [verb]" — the OECD conditional-hedging parenthetical** — OECD embeds conditional hedges inside relative clauses to qualify projections without breaking the main sentence.

> "Substantial increases in capacity... are planned worldwide, **which, if realised, will** exacerbate excess capacity."
> "New investments are expected to come online by 2026, **which, if completed, will** alter the market structure."

**T28. "at best" — the OECD pessimistic qualifier** — OECD uses "at best" to signal that a projection is optimistic, often used in commodity or industry outlooks.

> "With demand growth expected to be sluggish **at best**, capacity utilisation could once again decline."
> "Growth is set to remain modest **at best** over the medium term."

**T29. "around [X]%" / "close to [X]%" / "the majority of" — the OECD quantifier set** — OECD uses "around" and "close to" as its primary approximate quantifiers, not "approximately". "The majority of" is used instead of "most" when a specific number is implied. These are the OECD author's habitual approximators.

> "**Around** 80% of tax administrations reported getting data directly from business systems."
> "**Close to** 40% of tax administrations also reported being able to prefill VAT returns."
> "**The majority of** administrations is already in a position to offer complete prefilling."
> "**Around** 34 out of 39 countries have higher SME rates."

Verified: "around" appears 28–211 times per report across ALL genres. "close to" appears 6–17 times. "the majority of" appears 1–27 times. These replace "approximately" in OECD prose — which is almost never used.

**T30. "Taken together / Taken as a whole" — the OECD synthesising connector** — used to introduce a paragraph that draws together evidence from the preceding discussion. Unlike "In summary" (which is only for Policy Primers), "Taken together" works in all analytical genres.

> "**Taken together**, these developments suggest that economic uncertainty continues to contribute to sluggish SME credit growth."
> "**Taken as a whole**, the evidence points to a mixed picture."

**T31. "In light of / In the context of / Against this backdrop" — the OECD situating-phrase family** — these three phrases serve the same function: anchoring the current discussion in the broader policy context. They are interchangeable in OECD prose.

> "**In light of** these findings, the government should strengthen disclosure requirements."
> "**In the context of** the evolving conflict in the Middle East, higher energy prices would add to business costs."
> "**Against this backdrop**, while there are tentative signs of recovery, lending remains fragile."

These three phrases appear across ALL genres and are the OECD author's primary way of saying "given that X is happening, Y matters." AI defaults to "Due to" or "Because of"; OECD reaches for "In light of" / "In the context of" / "Against this backdrop".

**T32. "As a result / Consequently / Therefore" — the OECD causal connectors** — OECD uses all three, but "As a result" is the most frequent in analytical prose. "Consequently" is more formal. "Therefore" is used sparingly — OECD prefers "As a result" or "Consequently".

> "**As a result**, profitability has experienced a similar trajectory."
> "**Consequently**, the credit impact may be more muted."
> "**Therefore**, the estimates should be interpreted as descriptive."

**T33. "In fact / Indeed" — the OECD emphasis connectors** — OECD uses "In fact" and "Indeed" at sentence starts to strengthen a preceding claim with additional evidence. "Indeed" is slightly more formal than "In fact".

> "**Indeed**, lending in 2024 was still 4% down on 2022."
> "**In fact**, long-term loans, often used to finance investments, edged down."

Verified across Gender Equality, SME Financing, Steel Outlook, and Economic Surveys. Both appear in ALL genres.

**T34. "Despite [X], [Y]" — the OECD concessive-prepositional phrase** — OECD uses "Despite" as a prepositional phrase to introduce a concession without a full clause. This is more compact than "While" (T18) and works when the concession is a noun phrase rather than a clause.

> "**Despite** a gradual decline in inflation, financial conditions remain relatively restrictive."
> "**Despite** the increase in SME interest rates, the interest rate spreads with large firms generally declined."
> "**Despite** women's tremendous progress in tertiary education, notable gaps persist."
> "**Despite** efforts since 2018, there is no sign of decline in excess capacity."

Verified across SME Financing, Steel Outlook, Gender Equality, and Economic Surveys. This is the compact concessive form — use when the concession is a noun phrase; use "While" (T18) when the concession is a full clause.

**T35. "On the other hand" — the OECD two-sided-argument connector** — OECD uses "On the other hand" to present a contrasting perspective or evidence. It is more common in analytical and assessment genres than in recommendations.

> "**On the other hand**, the rebound is uneven and concentrated in few large investments."
> "**On the other hand**, fragmented issuance and small free floats can limit price discovery."
> "**On the other hand**, despite the increase in SME interest rates, spreads with large firms generally declined."

Verified across SME Financing, Supply Chain Review, Gender Equality, and Environmental Performance Reviews. This is the OECD author's preferred way to present a balanced two-sided argument. AI defaults to "However" for all contrasts; OECD uses "On the other hand" when presenting a genuinely different perspective rather than a direct contradiction.

**T36. Ultra-short emphasis sentence — "[X] differ(s)."** — OECD occasionally uses a dramatically short sentence (3–6 words) for emphasis, typically after a long explanatory paragraph. This is rare and deliberate.

> "National investment ecosystems **differ**."
> "The changes **will be uneven**."
> "Such impacts **won't be evenly distributed**."

Pattern: a single subject + verb, sometimes with a complement. The shortness creates contrast with surrounding prose. Verified in Investment Brief (VC), Environmental Brief (Fisheries). **Use sparingly** — one per document at most. AI never produces sentences this short; it always adds qualifiers.

**T37. Colloquial math — "that still leaves [proportion] that aren't"** — OECD occasionally uses informal arithmetic to make data relatable, especially in Policy Briefs aimed at non-specialist audiences.

> "And, of course, if 81% of assessed fish stocks are healthy, **that still leaves one in five that aren't**."

Pattern: "if X% are [Y], that still leaves [fraction/number] that [aren't/don't]." — the OECD way of humanizing a statistic. Verified in Environmental Brief (Fisheries). This is one of the most human patterns in all of OECD prose — it sounds like a person talking, not a machine reporting. **Genre-restricted**: use only in Policy Briefs, never in Surveys or Working Papers.

**T38. Parallel modal verbs for recommendation lists — "This could mean… It may require… would help to…"** — OECD uses different modal verbs across parallel recommendation sentences to avoid monotony and signal varying degrees of confidence.

> "This **could mean** conducting or supporting more regular and comprehensive fish stock assessments. It **may require** adjusting TACs and national quota allocations. Greater co-operation between scientists, stakeholders and policymakers **would help to** anticipate climate impacts."

Pattern: each recommendation sentence uses a different modal verb (could / may / would / should / there is scope to), creating variety within a parallel structure. Verified in Environmental Brief (Fisheries), Trade Brief (Subsidies). AI defaults to repeating the same modal ("should… should… should…"); OECD varies the modals to signal that some recommendations are more certain than others.

**T39. Country-tier comparison ladder — "X% in [A], Y% in [B], and Z% in [C]"** — OECD presents cross-country data in descending or ascending order, creating a ranked ladder that lets the reader immediately see who leads and who lags.

> "Algorithmic management tools are already widespread in the United States (adoption rate of 90%) and in the European countries surveyed (average of 79%), but less prevalent in Japan (40%)."
> "In the United States, 55% of firms monitor the content and tone of conversations, voice calls or emails. This compares to only 6% in Europe and 8% in Japan."

Pattern: "[Country A] ([X%]) ... [Country B] ([Y%]) ... [Country C] ([Z%])" — always three tiers. The ladder creates instant visual ranking. Verified in Algorithmic Management (Employment), Competition Trends. AI defaults to presenting countries in the order they appear in the data; OECD **reorders** to create a descending or ascending ladder.

**T40. "This is also the first [noun] to [verb]..." — the OECD novelty claim** — when a study or report offers genuinely new evidence, OECD flags it explicitly.

> "This is also the first study to offer direct evidence on how managers – the firsthand users – view such tools."
> "For the US and Japan, this study is the first to estimate the prevalence of algorithmic management tools using representative data from firms."

Pattern: "This is [also] the first [study/report/survey] to [verb] [what is new]." — use this to claim novelty without AI-default superlatives like "groundbreaking" or "unprecedented". Verified in Algorithmic Management, Budgeting Singapore.

**T41. "In contrast to [X], [Y] most often use..." — the OECD country-behaviour contrast** — OECD contrasts not just data points but **behavioural patterns** across countries.

> "In contrast to U.S. firms, European firms most often use instruction (adoption rate of 69%) and basic monitoring tools (33%), both of which are potentially less likely to draw on personal data."
> "In contrast to their European and Japanese counterparts, U.S. managers at non-adopting firms report that it is likely that their firms will adopt algorithmic management tools in the future."

Pattern: "In contrast to [Group A], [Group B] [verb] [different behaviour]." — this is more specific than "However" or "By contrast" — it names the comparator explicitly. Verified in Algorithmic Management, Competition Trends.

**T42. "The stronger impact observed in [X] could be due to the fact that..." — OECD hedged causal attribution** — when OECD explains why one country shows different results, it hedges the causal claim.

> "The stronger impact observed in the United States could be due to the fact that, as highlighted in Section 1, U.S. firms adopt algorithmic management tools with greater intensity."
> "This could be due to the possibility that white collar sectors are more digitalised and have made use of legacy technology systems for decades."

Pattern: "[Finding] could be due to [the fact that / the possibility that] [explanation]." — OECD never states cross-country causal claims as fact. AI defaults to "This is because"; OECD hedges with "could be due to the fact that". Verified in Algorithmic Management, ESG Ratings.

**T43. "While [X] offer some hope, the results show [Y]" — the OECD balanced hope/reality sentence** — OECD acknowledges that some evidence is promising while noting that the overall picture is mixed.

> "While managers' responses offer some hope in this regard, the results across countries show two opposing results."
> "While these efforts are positive, Spain has 19 ongoing foreign bribery cases."

Pattern: "While [positive evidence] offer(s) some hope / are positive, [overall results] show [mixed/reality]." — this is the OECD way of saying "it's not all bad, but it's not all good either". More nuanced than AI's "While X has benefits, it also has drawbacks". Verified in Algorithmic Management, Anti-Bribery Peer Review.

**T44. "though it should be noted that [X] does not automatically equate to [Y]" — the OECD analytical caveat** — OECD uses this to prevent over-interpretation of findings.

> "nearly two-thirds of managers have at least one concern regarding the trustworthiness of the algorithmic management tools they use (though it should be noted that concern does not automatically equate to harm)."

Pattern: "though it should be noted that [X] does not automatically equate to [Y]" — this is a **genuine analytical caveat**, not AI padding. Use when a finding could be misread. Verified in Algorithmic Management, ESG Ratings.

**T45. "This compares to only [X]%" — the OECD cross-region benchmark** — OECD introduces a comparison data point with "This compares to" to immediately benchmark a previously stated figure.

> "In the United States, 55% of firms monitor the content and tone of conversations, voice calls or emails. This compares to only 6% in Europe and 8% in Japan."

Pattern: "[Country A] [data point]. This compares to only [X]% in [Country B] and [Y]% in [Country C]." — the "This compares to only" creates dramatic contrast. Verified in Algorithmic Management, Competition Trends.

---

## What is genre-specific (do NOT cross-port)

Apply only to the indicated genre:

| Element | Belongs to |
|---------|------------|
| Inline citations every 2-3 sentences | Economic Survey, Education Review, Peer Review |
| "albeit" / "inter alia" / "thereby" / "notwithstanding" | Economic Survey, Peer Review (sparingly), Financial Market Paper |
| "in practice" reflex | Economic Survey, Peer Review |
| Dense "notably" / "particularly" / "in particular" | Economic Survey |
| Heavy nominalisations ("the implementation of") | Economic Survey, Working Paper, Peer Review, Financial Market Paper |
| Mid-clause "however" parentheticals | Economic Survey, Peer Review |
| Question-form section headings | Policy Primer / Brief, Trade Brief, Environmental Brief, Security Brief |
| Bullet-led recommendations | Policy Primer / Brief, Country Profile, Investment Brief |
| First-person "we" voice | Working Paper |
| JEL codes / academic references | Working Paper |
| Gerund subtitles ("Strengthening X…") | Executive Summary, Survey chapter headings |
| "Considerations" softer than "recommendations" | Country Review (Education / Health) |
| Warm vocabulary ("thrive", "those who need them most") | Country Review (Education) |
| "The lead examiners commend / note / observe" | Peer Review |
| Abstract conceptual opening | Country Profile (GaaG, Cancer Profile) — see §9.3 |
| "In summary" / "To conclude" closes | Policy Primer / Brief only |
| "What's the issue?" / "Why is this important?" structure | Trade Brief, Environmental Brief, Security Brief |
| Box format for case studies | Financial Market Paper |
| Neutrality disclaimer ("without taking a position") | Financial Market Paper |
| Creative subtitles ("Too close to the sun") | Trade Brief (rare) |
| "win-win-win" triple-benefit framing | Environmental Brief |
| Colloquial math ("that still leaves one in five") | Environmental Brief |
| Ultra-short emphasis sentences ("X differ.") | Investment Brief |
| Multi-group data presentation ("women (8% vs. 10%)…") | Country Policy Assessment Notes |
| Program outcome statements ("more than 1,000 have completed") | Country Policy Assessment Notes |
| Threat-focused opening ("In the last three decades…") | Security Brief |
| Actor adaptation description ("X exploit advancements in Y") | Security Brief |
| Acknowledgments listing contributors by name/institution | Financial Market Paper |
| Committee discussion dates in metadata | Financial Market Paper |

**The most common overfitting mistake**: applying the full Economic Survey fingerprint set (citations, "albeit", "thereby", heavy nominalisations, dense "notably") to a Policy Primer, Trade Brief, or Country Review. Do not do this. Each genre has its own equilibrium.

---

## 1. Diction (用词)

OECD diction is a **closed lexical system** — the same 200–300 words and phrases recur across publications. Mastery means internalising this restricted register, not generating synonyms.

### 1.1 Formality register: replace common words

| Colloquial / generic | OECD-preferred |
|---------------------|----------------|
| help | facilitate, foster, bolster, underpin, support, enable |
| get worse | deteriorate, worsen, weaken, erode |
| get better | improve, strengthen, advance |
| big | substantial, considerable, significant, sizeable, marked |
| small | modest, limited, marginal, minor |
| show | demonstrate, indicate, reveal, point to, highlight, underscore |
| use | employ, deploy (sparingly), apply, leverage, draw on |
| a lot of | a substantial share of, a considerable proportion of, the bulk of |
| many | a number of, several, numerous |
| problem | challenge, issue, gap, deficiency, weakness, constraint, impediment |
| good | sound, robust, well-designed, effective |
| bad | weak, inadequate, deficient, ineffective |
| about (approx.) | approximately, roughly, around, on the order of |
| start | initiate, launch, embark on, commence |
| end | conclude, terminate, phase out, discontinue |
| change | adjust, recalibrate, modify, revise, reform |
| think | consider, view, regard, assess |
| keep | maintain, retain, preserve, sustain |
| stop | curb, contain, halt, prevent |

### 1.2 The verb system (动词系统)

OECD verbs cluster into **five functional families**. Pick from the right family for the rhetorical move you are making.

**(a) Trend verbs — describe movement of indicators**
- Upward: "increase", "rise", "grow", "expand", "accelerate", "pick up", "rebound", "edge up", "tick up", "surge"
- Downward: "decrease", "decline", "fall", "drop", "ease", "moderate", "soften", "subside", "abate", "slow", "contract", "edge down", "tick down", "plunge", "tumble", "dip", "slip"
- Stable: "remain stable", "stand at", "hover around", "hold steady", "broadly stabilise", "plateau", "level off", "bottom out"
- Volatile: "fluctuate", "oscillate", "vary", "swing"
- Magnitude pairing: trend verbs almost always carry a magnitude modifier — "increased **slightly**", "rose **sharply**", "fell **considerably**", "**broadly** stabilised"
- **Graduated movement verbs** — OECD distinguishes tiny, moderate, and large movements with different verbs:
  - Tiny: "edge up/down", "tick up/down", "inch up/down", "nudge up/down" — "SME rejection rates **edged up**."
  - Moderate: "increase", "rise", "decline", "fall" — "GDP **rose** by 2.1%."
  - Large: "surge", "soar", "plunge", "tumble", "jump" — "Capacity **surged** by 130%."
  - **OECD never uses the same movement verb twice in the same paragraph.** Vary: if you used "increase" once, use "rise" or "edge up" next.
- **State-change verbs** — describe transitions, not just movements:
  - "ease" / "easing" — gradual, controlled decline: "Borrowing costs were beginning to **ease**."
  - "subside" — decline from a peak: "Inflationary pressures **subsided**."
  - "plateau" / "plateaued" — reaching a stable level after change: "Growth **plateaued** at around 2%."
  - "bottom out" — reaching the lowest point: "Capacity utilisation appears to be **bottoming out**."
  - "level off" — stabilising after a trend: "Outstanding stocks of SME loans **levelled off**."
  - "cool" / "cooling" — gradual decline from overheated state: "The housing market is **cooling**."
  - "soften" / "softening" — gentle decline: "Labour markets are **softening**."

**(b) State verbs — describe what is the case**
- "stand at [number]" (signature OECD verb): "Gross debt **stood at** 117% of GDP at the end of 2024."
- "remain + adjective": "remain limited", "remain in place", "remain valid", "remain robust", "remain significant"
- "represent": "USD 1.3 billion **represented** 25.4% of bilateral ODA"
- "amount to": "Public expenditure **amounted to** 28.2% of GDP"
- "account for": "Microenterprises **accounted for** 92.6% of all enterprises"
- "make up": "ODA for social infrastructure **makes up** 31% of bilateral commitments"
- "rank [N]th": "Argentina **ranked 26th** in FDI stock"

**(c) Policy verbs — describe what governments/institutions do**
- Strengthening: "strengthen", "enhance", "bolster", "reinforce", "consolidate", "step up", "scale up", "deepen"
- Easing: "ease", "phase out", "discontinue", "scale back", "wind down"
- Implementing: "implement", "operationalise", "roll out", "introduce", "enact", "pursue", "advance"
- Aligning: "align with", "mainstream into", "embed in", "integrate with", "reconcile with"
- Reviewing: "monitor", "oversee", "assess", "evaluate", "scrutinise", "review"

**(d) Analytical verbs — connect evidence to inference**
- "reflect" (most common): "This **reflects** the fact that…"
- "underscore": "These trends **underscore** the need for reform"
- "highlight": "The data **highlight** persistent vulnerabilities"
- "point to": "These figures **point to** structural weaknesses"
- "warrant": "Risks **warrant** careful oversight"
- "compound" / "exacerbate": "High debt **compounds** the risk of fiscal stress"
- "drive": "House prices are **driven by** insufficient supply"
- "weigh on": "Tariffs **weigh on** the economic outlook"

**(e) Recommendation verbs — modal + bare infinitive constructions**
- "should + verb": "Canada **should reapply** the fuel charge"
- "warrant + noun": "The situation **warrants** decisive action"
- "could be + past participle": "This **could be offset** by…"
- "ought to" — avoid; less institutional
- "must" — use sparingly, only for treaty/convention obligations

### 1.3 The adjective and adverb system (形容词与副词系统)

OECD prose runs on **gradient modifiers** that hedge or sharpen claims with surgical precision.

**Magnitude ladder (light → heavy)**
> slight → modest → moderate → considerable → substantial → significant → marked → pronounced → severe

**Adverbial intensifiers / dampeners** — these are **the most distinctive OECD lexical signature**:
- **broadly**: softens precision — "broadly stable", "broadly in line with", "broadly speaking"
- **relatively**: comparative softener — "relatively low", "relatively stable"
- **notably / particularly / especially / in particular**: very high-frequency in OECD prose. A single Economic Survey may use "notably" 30-100 times. Use freely as a softer alternative to "especially" or to flag the most relevant element of a list. Pattern: "…public investment, **notably** in transport infrastructure", "expenditures, **particularly** for ageing-related costs"
- **largely**: attributes most but not all — "largely driven by", "largely uneven"
- **comparatively**: implicit benchmark — "comparatively low", "comparatively favourable"
- **somewhat**: weakest hedge — "somewhat higher", "somewhat distinctive"
- **slightly**: minimal magnitude — "slightly above", "slightly distinctive"
- **considerably / significantly / substantially**: strong but neutral
- **markedly / pronouncedly**: emphasis without drama
- **persistently / consistently**: temporal weight — "persistently weak", "consistently above"

**Evaluative adjectives** — institutional judgement vocabulary:
- Positive: "robust", "sound", "resilient", "well-designed", "comprehensive", "well-targeted", "credible", "stringent"
- Negative: "weak", "uneven", "limited", "fragmented", "inadequate", "insufficient", "deficient", "ineffective", "vulnerable"
- Neutral observational: "noteworthy", "salient", "distinctive", "marked"

**Avoid these adjectives entirely** (too informal/emotional): "amazing", "great", "huge", "tiny", "terrible", "horrible", "wonderful", "fantastic", "tremendous", "alarming", "devastating", "shocking".

### 1.4 The noun system (名词系统)

**Nominalisation preference** — OECD turns verbs into nouns to compress and depersonalise:
- "the government implements" → "the implementation of [X]"
- "they review" → "the review process"
- "they comply" → "compliance with"
- "they provide" → "the provision of"
- "they oversee" → "oversight of"
- "they monitor" → "monitoring of"

**Institutional abstract nouns** (high-frequency):
> framework, mechanism, instrument, arrangement, scheme, regime, system, structure, capacity, framework, governance, oversight, alignment, coherence, sustainability, resilience, integrity, transparency, accountability, compliance, adoption, uptake, coverage, scope

**Use sparingly** — these are needed but **never as paragraph-opening subjects** (see §2 subject rules).

### 1.5 Signature collocations (高频固定搭配)

Internalise these as **single units of meaning**. They are the lexical fingerprints of OECD prose.

**Comparison / benchmark phrases**
- "in line with the OECD average"
- "broadly in line with"
- "above / below the OECD average"
- "compared to / compared with [benchmark]"
- "in real terms" (always after change figures)
- "in international comparison"
- "compared with [year]"
- "as a share of GDP / GNI"
- "relative to peers" / "relative to its peers"

**Quantification phrases**
- "stood at [number]" / "stands at [number]"
- "amounted to [number]"
- "accounted for [percentage]"
- "represented [percentage]"
- "reached [number]"
- "the share of [X] in [Y] is [percentage]"
- "approximately three-quarters" / "almost two-thirds"

**Trend phrases**
- "an increase / decrease of X% from [year]"
- "from X% in [year] to Y% in [year]"
- "X percentage points higher / lower than"
- "a decline of X% in real terms"
- "X% per annum"
- "broadly stabilised" / "broadly stable"
- "on a declining path" / "on an upward trajectory"

**Recommendation phrases**
- "there is scope to [verb]"
- "there is room to [verb]"
- "would benefit from [noun]"
- "this is welcome and should be continued"
- "warrants further action"
- "[X] should be stepped up"
- "more can be done to [verb]"

**Hedging phrases** (see §1.6 below)
- "appears to be", "tends to", "is likely to"
- "available evidence suggests"
- "preliminary data indicate"

**Causation phrases**
- "this reflects"
- "this is due to"
- "driven by"
- "as a result of"
- "compounded by"

**Tricolon (rule of three) — a near-mandatory rhetorical device**
OECD authors love three-element parallel lists, especially for recommendations or evaluations:
- "timely, targeted, and temporary" (fiscal support)
- "more systematic, recurrent, and comprehensive"
- "fiscal sustainability, patient access, and incentives for innovation"
- "investigation, prosecutions, and corporate accountability"
- "transparency, responsiveness, and data-driven decision-making"
- "designing, implementing, and evaluating"

**Use the tricolon at least once per executive summary or section opener.**

### 1.6 Hedging (缓冲措辞) — the OECD epistemic register

OECD prose **almost never makes flat claims**. Almost every assertion is wrapped in a hedge that signals institutional caution. This is the single most underestimated stylistic feature.

**Epistemic hedges** (signal degree of certainty)
- "appears to be" — softer than "is"
- "tends to" — generalisation without absolutes
- "is likely to" / "is expected to" — projections
- "may" / "could" — possibility
- "available evidence suggests"
- "preliminary data indicate"
- "broadly speaking"

**Quantification hedges** (soften numerical claims)
- "approximately", "roughly", "around", "about"
- "on the order of"
- "in the region of"
- "an estimated"
- "in the range of X to Y"

**Attribution hedges** (distance the OECD from the claim)
- "according to [source]"
- "the OECD estimates that"
- "as reported by"
- "based on [source]"
- "data show that" (rather than "we found")

**Conditional hedges** (caveat the recommendation)
- "provided that"
- "subject to"
- "depending on"
- "should [X] materialise"
- "if conditions allow"

**Apply hedging to projections and judgements**, NOT to historical facts. "GDP grew by 1.5% in 2024" needs no hedge. "GDP **is expected to grow** by 1.1% in 2026" needs the hedge.

### 1.7 Spelling and conventions

- **British English**: "recognise" not "recognize", "colour" not "color", "programme" not "program" (except "program" for software/computing), "labour" not "labor", "centre" not "center", "behaviour" not "behavior"
- Latinate hyphenation: "co-operation", "co-ordination", "decision-making", "policy-making"
- Oxford comma: optional but consistent within a document
- Currency: "USD" / "EUR" / "GBP" before the number (USD 7.5 billion)
- Per cent: write "per cent" (two words) in running text; "%" only in tables and parentheses
- Dates: "10 December 2025" (day-month-year), not "December 10, 2025"
- Use **non-breaking spaces** between numbers and units in formal output: "USD 7.5 billion", "0.62% of GNI"

### 1.8 Anti-AI lexical signals (防止默认 AI 风格渗透)

This section is **the most important defence** against generic AI prose creeping into output. Modern language models default to a recognisable register — vague, padded, evaluative, hedge-rich in the wrong places. OECD prose is none of those things. Drill this list into every output.

**A. Banned AI-default phrases** (eliminate on sight):

| AI default phrase | Why it fails | OECD replacement |
|------------------|--------------|------------------|
| "It is important to note that…" | Padding; OECD doesn't tell you what's important | Just state the fact |
| "It is worth noting that…" | Same problem | Just state the fact |
| "It should be noted that…" | Throat-clearing | Drop and start with the fact |
| "Notably," (every paragraph) | Salience inflation | Use ≤ once per page |
| "In today's world / In the modern era" | Empty framing | Drop entirely |
| "Plays a crucial role" | Bureaucratic vague | Name what the entity does: "regulates X", "funds Y", "monitors Z" |
| "A multifaceted approach" | Vague | Specify the components |
| "Navigate the complexities of" | Cliché | "address", "respond to", "manage" |
| "Leverage" (as verb) | Overused | "use", "draw on", "apply" |
| "Robust framework" (no specifics) | Empty praise | Name the framework's actual provisions |
| "Holistic" / "synergistic" | Buzzwords | Be concrete |
| "In an increasingly [adjective] world" | Cliché framing | Drop |
| "Stakeholders" (when vague) | When unclear who | Name them: "workers, firms, regulators" |
| "It goes without saying" | Then don't say it | Drop |
| "At the end of the day" | Conversational | "In conclusion" / drop |
| "Cutting-edge" / "state-of-the-art" | Marketing register | "advanced", "modern", or omit |
| "Ever-evolving" / "rapidly changing" | Vague | Specify the change |
| "Boasts" (a country boasts X) | Promotional tone | "has", "maintains" |
| "Deep dive" | Casual | "detailed analysis" |
| "Game-changer" / "paradigm shift" | Hyperbole | Describe the actual change |
| "Unprecedented" (overused) | Cliché since 2020 | Quantify or qualify |
| "Critical importance" / "of paramount importance" | Empty intensification | Drop the modifier |
| "Showcases" (a study showcases X) | Marketing register | "shows", "demonstrates", "indicates" |
| "Underscore the importance of" (every other sentence) | Overuse | Use sparingly, ≤ once per page |
| "Sheds light on" | Cliché | "examines", "documents" |
| "Bring to the fore" / "come to the fore" | Cliché | "highlight", "draw attention to" |
| "Cornerstone" / "linchpin" / "bedrock" | Metaphor padding | Drop the metaphor |
| "Tapestry of" / "ecosystem of" / "landscape of" | Filler metaphor | Drop or be specific |
| "Vibrant" / "dynamic" / "thriving" | Promotional | Drop or use "active", "expanding" |
| "Look no further than" | Conversational | Drop |
| "When it comes to" | Verbal placeholder | "On", "Regarding", or restructure |
| "It's not just X, it's Y" | Rhetorical pattern | Restructure declaratively |
| "From X to Y to Z" (rhetorical sweep) | Padding | List or specify |
| "In a nutshell" | Casual | "In sum", or drop |

**B. Banned AI-default sentence structures**:

- ✗ "While X, it is also true that Y." → ✓ "X. Y, however, …"
- ✗ "On the one hand, X. On the other hand, Y." → ✓ "X. By contrast, Y." (or merge into one sentence)
- ✗ "Not only X, but also Y." → ✓ "X. Furthermore, Y." (or merge)
- ✗ "Furthermore, it is essential to recognise that…" → ✓ Drop the framing; state the fact
- ✗ "This raises the question of whether…" → ✓ State the question directly or skip the meta-framing
- ✗ "In essence" / "Essentially" → ✓ Drop; state the substance
- ✗ "This serves to highlight…" → ✓ "This highlights…" (active, no auxiliary)
- ✗ Three-clause rhetorical sweeps with semicolons covering every angle → ✓ Pick the two most relevant points; let them land
- ✗ Concluding sentences that summarise the paragraph ("Together, these factors demonstrate that…") → ✓ Drop; let the evidence speak. OECD almost never summarises within a paragraph

**C. Banned tonal moves** (the AI "essay-mode" tells):

- **Universal-truth openings**: "Throughout history, humanity has…", "In an interconnected world…", "As nations grapple with…" — never use these
- **Self-reflective sentences about the analysis itself**: "This analysis reveals that…", "It becomes clear that…", "What emerges is a picture of…" — OECD does not narrate its own findings
- **Emotive intensifiers without data**: "extremely significant", "absolutely critical", "deeply concerning" — use plain "significant", "important", "concerning" only when warranted
- **Aspirational closers**: "Going forward, [country] must…", "The path ahead requires…", "Only by working together can we…" — OECD recommendations are concrete, not motivational
- **Rhetorical questions in body text**: "How can [country] address these challenges?" — OECD almost never asks rhetorical questions in running prose

**D. Banned structural moves**:

- Triple synonym lists for emphasis: "comprehensive, holistic, and integrated approach" — pick one or be specific
- Triple-adjective stacking: "robust, resilient, and adaptive system" — limit to two unless they carry distinct meaning
- "Both X and Y" when only Y matters — just say Y
- Bullet lists when prose would carry the same content more cohesively
- Paragraph-final summaries beginning "In conclusion," / "Overall," / "Taken together," — drop them; the evidence already stands
- Section openings that summarise what the section will cover: "This section examines…", "The following discusses…" — open with content, not signposts

**E. Tonal calibration check** — read your draft and ask:
1. Does any sentence read like a TED talk? Cut it.
2. Does any sentence sound like a corporate press release ("[Country] is committed to delivering best-in-class outcomes")? Rewrite plainly.
3. Does any sentence sound like a textbook trying to teach a concept ("Inflation, defined as the general rise in prices, …")? OECD assumes the reader knows the concept.
4. Does any paragraph end with a value judgement uninvited by the data? Cut the final sentence.
5. Does any sentence use a metaphor (cornerstone, lifeline, bedrock, springboard, tapestry, landscape)? Almost always drop the metaphor — OECD prose is post-metaphorical.

**F. The 30-second smell test**: imagine this paragraph appearing in *The Economist*'s leader column versus an OECD Economic Survey. If it would fit better in *The Economist* — too journalistic, too punchy, too rhetorical — pull it back. OECD is **drier** than serious journalism. The dryness is the signature.

**G. AI → OECD word-level replacement table** (cross-verified across 25+ documents, 12+ genres)

This is the **most practical anti-AI tool**. When you see an AI-default word in your draft, replace it with the OECD equivalent. Each row is verified against real OECD documents.

| AI default | OECD replacement | Why | Example |
|-----------|-----------------|-----|---------|
| "significantly" | "markedly", "sharply", "notably", "considerably" | AI overuses "significantly"; OECD uses it but also varies | "add **markedly** to business costs" |
| "important" | "significant", "salient", "critical", "key" | AI uses "important" as a universal intensifier | "**salient** gaps persist" |
| "impact" (verb) | "weigh on", "affect", "have implications for", "bear on" | AI uses "impact" as a verb; OECD rarely does | "tariffs **weigh on** the outlook" |
| "increase/decrease" (noun) | "rise/fall", "pickup", "decline", "easing" | AI nominalises verbs awkwardly | "the **pickup** in investment" |
| "because" / "due to" | "given", "as", "since", "owing to", "in light of", "reflecting" | AI defaults to "because"; OECD varies | "**Given** the scale of the challenge" |
| "however" (every sentence) | "Nonetheless", "In contrast", "On the other hand", "By contrast", "At the same time" | AI uses "however" as the only contrast connector | "**By contrast**, in [country]…" |
| "furthermore" / "moreover" | "In addition", "More broadly", "Similarly", "Additionally" | AI uses these as default additions | "**More broadly**, the regulatory environment…" |
| "it is important to note" | *(delete entirely)* | OECD never tells the reader what's important | Just state the fact |
| "in order to" | "to" (simple infinitive) | AI pads purpose clauses; OECD uses bare "to" | "strengthen surveillance **to** prevent…" |
| "plays a crucial role" | "regulates X", "funds Y", "monitors Z", "accounts for X%" | AI uses vague role-claims; OECD names the function | "the central bank **supervises** 85% of assets" |
| "has/have been able to" | "has/have [past participle]" | AI pads with "been able to"; OECD is direct | "countries **have adopted**" not "have been able to adopt" |
| "a wide range of" | "various", "a variety of", or name them | AI uses "a wide range of" as filler | "**various** policy instruments" or list them |
| "comprehensive" | "robust", "credible", "well-designed", "well-targeted" | AI uses "comprehensive" as universal praise | "a **well-designed** regulatory framework" |
| "multifaceted" | name the facets | AI hides behind "multifaceted"; OECD specifies | "fiscal, regulatory, and labour market reforms" |
| "navigate" | "address", "respond to", "manage", "tackle" | "navigate" is AI/corporate jargon | "**address** the challenges" |
| "landscape" | *(drop or be specific)* | AI uses "landscape" as filler metaphor | "the regulatory **framework**" or "the **market structure**" |
| "ecosystem" | *(drop or be specific)* | AI uses "ecosystem" as filler metaphor | "the **sector**", "the **industry**", "the **market**" |
| "leverage" (verb) | "use", "draw on", "apply", "exploit" | "leverage" is corporate jargon | "**draw on** existing infrastructure" |
| "robust" (standalone) | "robust" + noun (always pair with a specific noun) | AI uses "robust" as empty praise; OECD always specifies what is robust | "a **robust** regulatory framework" not just "robust" |
| "stakeholders" (vague) | name them: "workers, firms, regulators, unions" | AI hides behind "stakeholders"; OECD names the actors | "**employers and trade unions**" |
| "drive" (as in "drive change") | "foster", "promote", "support", "facilitate", "encourage" | AI overuses "drive" as a causation verb | "**foster** innovation" |
| "enhance" (standalone) | "strengthen", "improve", "deepen", "expand" | AI uses "enhance" as a universal improvement verb | "**strengthen** oversight" |
| "foster" (every paragraph) | "promote", "support", "facilitate", "encourage", "enable" | AI uses "foster" as its only policy verb | "**support** SME access to finance" |
| "crucial" | "important", "critical", "essential", "key" | "crucial" is AI's favourite intensifier | "**essential** for financial stability" |
| "paramount" | *(delete or use "critical")* | "paramount" is hyperbolic | "of **critical** importance" → just "important" |
| "unprecedented" | "unusual", "exceptional", quantify the scale | AI overuses "unprecedented" since 2020 | "**the largest decline since 2008**" |
| "ever-evolving" | specify the change | AI filler | "the **rapid expansion of** digital services" |
| "rapidly changing" | specify the change | AI filler | "the **growing** role of AI" |
| "cutting-edge" | "advanced", "modern", or omit | Marketing register | "**advanced** analytical tools" |
| "in today's world" | *(delete entirely)* | Empty framing | Just start with the substance |
| "this is worth noting" | "this is noteworthy because [reason]" or just state the fact | AI uses "it is worth noting" as empty padding; OECD uses "noteworthy" with a **specific reason** or uses "It is worth noting that" only when introducing a genuinely surprising data point | "It is worth noting that 72% of U.S. firms already use at least one tool" (surprising data) vs. AI's "It is worth noting that this is important" (empty) |
| "it should be noted" | "though it should be noted that [X] does not automatically equate to [Y]" | AI uses "it should be noted" as filler; OECD uses "though it should be noted" as a **genuine analytical caveat** that prevents over-interpretation | "though it should be noted that concern does not automatically equate to harm" |
| "this is because" | "This could be due to the fact that", "This reflects", "This is to be expected, as" | AI states causation as fact; OECD hedges with "could be due to the fact that" or explains why the result is expected | "The stronger impact observed in the US could be due to the fact that US firms adopt tools with greater intensity" |
| "more research is needed" | "Further research would be needed to ascertain whether [X] and if so, whether [Y]" | AI uses "more research is needed" as a throwaway line; OECD specifies **what** research and **what conditional outcome** it would confirm | "Further research would be needed to ascertain whether these are the most relevant drivers and if so, whether the increase will lead to greater enforcement" |
| "the analysis shows" | "The analysis remains at the [X] level" / "This does not consider [Y]" | AI states findings without scope limitations; OECD explicitly states what the analysis does NOT cover | "The analysis remains at the metric level. This analysis does not consider scoring methodologies." |
| "leveraging" | "draw on", "use", "apply", "exploit" | "leveraging" is corporate jargon; OECD uses "exploit" (for illicit actors) or "draw on" (for legitimate use) | "exploit advancements in technology" (illicit) / "draw on a unique survey" (legitimate) |
| "spearheading" | "leading", "driving", "initiating" | AI uses "spearheading" as heroic framing; OECD uses plain verbs | "leading the development of" |
| "empowering" | "enabling", "supporting", "providing [X] with [Y]" | "empowering" is development jargon; OECD uses it only in operational guidance manuals (Tax Manual genre) | "providing jurisdictions with the tools and knowledge needed" |
| "grapple with" | "address", "respond to", "manage" | "grapple with" is acceptable in OECD when describing policymakers facing genuine uncertainty (verified in Algorithmic Management) — but NOT as a universal replacement for "address" | "As policymakers grapple with how to respond" (genuine uncertainty) |
| "at odds with" | "inconsistent with", "contrary to", "diverge from" | "at odds with" is a genuine OECD connective (verified in ESG Ratings) — more precise than "conflicts with" | "This structure is also at odds with recent standards" |
| "de facto" | "in practice", "effectively", or specify | "de facto" is acceptable OECD Latin (verified in ESG Ratings: "de facto standard setters") — but don't overuse | "de facto standard setters to standard takers" |
| "simply be" | keep as-is when offering alternative explanation | "This could simply be [mundane explanation]" is a **genuine OECD fingerprint** — AI never defaults to the boring explanation | "This could simply be a time delay in cases feeding into the data" |
| "pose a threat / challenge" | "challenge", "complicate", "affect", "burden" | AI uses "pose" as a generic risk verb; OECD uses it only for **structural/constitutional threats** — "these reforms can pose challenges for smaller organisations" (Regulatory Brief) | "which can pose challenges for smaller organisations with limited resources" |
| "lag behind" | "fall short of", "fail to meet", "are weaker than" | **OECD signature phrase** for regulatory-gap analysis (verified in PMR Evidence, Anti-Corruption) — "lag behind best practice" is a specific OECD institutional-assessment frame | "the regulatory frameworks... lag behind best practices in many countries" |
| "room for" (improvement) | "scope for improvement", "needs to improve" | OECD's preferred reform-indication phrase — "suggesting room for stronger obligations" (PMR Evidence) — softer than "needs" | "suggesting room for stronger obligations to foster the quality of policies" |
| "associated with" (causal link) | "caused by", "leads to", "results in" | OECD always uses "associated with" rather than asserting direct causality from correlation — standard empirical caution | "studies have found a negative association between corruption and income and human development" |
| "highlight" / "underscore the importance" | "prove", "demonstrate conclusively" | AI overclaims with "prove/demonstrate"; OECD uses "highlight" and "underscore" as **medium-strength analytical bridges** — stronger than "suggest" but weaker than "prove" | "these findings underscore the importance of better regulatory policies" |
| "a growing number of" | "many", "numerous", "most" | AI uses vague quantifiers; OECD uses **"a growing number of"** to signal an empirically observed trend without specifying an exact count — a genuine OECD hedge | "the growing number of countries adopting these policies" |
| "do not automatically equate to" | "do not mean", "do not indicate" | OECD uses this long-form qualification to prevent over-interpretation — a **genuine human fingerprint** (fingerprint N) | "though it should be noted that concern does not automatically equate to harm" |

**H. Context-dependent AI signals** — some phrases are AI padding in one context but genuine OECD usage in another. Know the difference:

| Phrase | AI padding when… | Genuine OECD when… |
|--------|-----------------|---------------------|
| "It is worth noting that" | Followed by a vague importance claim ("this is important") | Followed by a **surprising data point** ("72% of U.S. firms already use…") |
| "It should be noted that" | Opening a paragraph as filler | Embedded as "though it should be noted that X does not equate to Y" — a genuine caveat |
| "On the one hand / On the other" | Used in analytical body paragraphs | Used **only in abstracts** of empirical reports to frame the policy tension (§9.16) |
| "This is important because" | Followed by a generic reason | Followed by a **specific analytical consequence** ("This is noteworthy because [Country] has the highest rate") |
| "In order to" | Padding a simple purpose clause | Acceptable in operational guidance manuals (Tax Manual genre) where legal precision requires it |
| "Furthermore / Moreover" | Connecting paragraphs with generic addition | Acceptable when adding a **genuinely new dimension** (not just "also") |
| "It will be worth monitoring" | Generic forward-looking filler | Genuine when tied to a **specific data trend** and a **specific future edition** ("in future editions of this report") |

### 1.9 Human-author fingerprints (真人作者指纹)

This section addresses a problem the lexical and syntactic rules above cannot solve on their own. Even after every AI-default phrase is purged, polished AI prose still feels too **smooth, too uniform, too clean**. AI detectors flag this smoothness as "robotic formality" or "mechanical precision". Real OECD authors, despite writing formal institutional prose, leave specific **roughness markers** that AI does not produce by default.

**You must deliberately introduce these fingerprints.** They are not stylistic flaws — they are the texture of human institutional writing.

#### Genre-applicability matrix (read this before applying any fingerprint)

**WARNING: not every fingerprint applies to every OECD genre.** Mechanical application across all OECD output is itself a sign of overfitting. Cross-genre measurement on real OECD documents shows the following distribution. Apply each fingerprint **only at the indicated density for the target genre**.

| Fingerprint | Economic Survey | Country Review (Education / Health) | Country Profile (GaaG / Cancer) | Working Paper | Policy Primer / Brief | Peer Review (Anti-Bribery / NCPE) |
|-------------|:---------------:|:-----------------------------------:|:-------------------------------:|:-------------:|:---------------------:|:---------------------------------:|
| Inline citations every 2-3 sentences | **YES, very dense** | YES (Education) / **LOW** (Health) | LOW | LOW-MED | **NONE** | YES, dense |
| "such as" / "including" example unfolding | YES | **YES (most dense)** | YES | YES (less) | YES (less) | YES |
| "in practice" reflex | **YES, signature** | rare | rare | rare | rare | **YES, signature** (also Supply Chain / Compliance / Procedural reviews) |
| "notably" / "particularly" / "in particular" | **YES, very dense** | rare | YES (sparingly) | rare | rare | YES |
| "albeit" | YES (sparingly) | **NEVER** | rare | rare | **NEVER** | rare |
| "inter alia" | rare-YES | **NEVER** | **NEVER** | rare | **NEVER** | rare |
| "thereby" / "to that end" / "notwithstanding" | YES (sparingly) | YES (Environmental Performance, Supply Chain) | rare | rare | rare | YES (sparingly) |
| Heavy preposition stacking | **YES** | medium | medium | YES | **NO (deliberately accessible)** | YES |
| Imperfect parallelism | YES | YES | YES | YES | medium | YES |
| Repeated technical terms (no synonym swap) | **YES** | YES | YES | YES | YES (less) | **YES** |
| Mid-clause "however" parentheticals | YES | medium | medium | YES | rare | YES |
| Heavy nominalisations | **YES, default** | medium | medium | YES | **NO (more verbal)** | YES |
| Flat-fact paragraph endings | YES | medium | YES | YES | rare (often summary) | YES |
| Unresolved arguments | YES | medium | medium | YES | NO (primers conclude) | YES |
| Slightly warmer / human tone | **NO (drier)** | **YES (Education especially)** | NO | NO | YES (more accessible) | NO |
| Bullet-point recommendations | rare | rare | YES | NO | **YES** | rare |
| Question-form section headings | **NEVER** | rare | rare | NEVER | **YES ("What can policymakers do?")** | NEVER |
| Synthesising / "in summary" closes | **NEVER** | rare | rare | NEVER | **YES** | NEVER |
| First-person "we" voice | **NEVER** | NEVER | NEVER | **YES (working papers)** | rare | NEVER |

**Extended matrix — new genres verified from v8 deep sampling:**

| Fingerprint | Empirical Survey Report | Country Governance Study | Annual Data / Trends Report | Metric Assessment Report | Operational Guidance Manual |
|-------------|:-----------------------:|:------------------------:|:---------------------------:|:------------------------:|:---------------------------:|
| Inline citations every 2-3 sentences | LOW-MED (academic refs) | LOW (institutional) | LOW (data source annexes) | MED (methodology notes) | LOW (country examples) |
| "such as" / "including" example unfolding | YES | YES | YES | YES | YES |
| "in practice" reflex | rare | rare | rare | rare | YES (procedural) |
| "notably" / "particularly" | rare | rare | rare | YES (data observations) | rare |
| "albeit" | rare | rare | rare | rare | **NEVER** |
| Heavy preposition stacking | medium | YES | medium | medium | YES (legal precision) |
| Imperfect parallelism | YES | YES | YES | medium | YES |
| Repeated technical terms | YES | YES | YES | YES | **YES (legal terms)** |
| Mid-clause "however" | YES | medium | YES | medium | rare |
| Heavy nominalisations | medium | YES | medium | YES | YES (procedural) |
| Flat-fact paragraph endings | YES | YES | YES | YES | YES |
| Unresolved arguments | YES | medium | YES | YES | NO (guidance concludes) |
| Question-form section headings | **YES (research questions)** | NEVER | NEVER | NEVER | NEVER |
| First-person institutional voice | **YES ("this study")** | rare | NEVER | NEVER | **YES (Preface "we")** |
| Balanced "one hand / other" framing | **YES (abstract only)** | NEVER | NEVER | NEVER | NEVER |
| Hypothesis enumeration | rare | rare | **YES** | rare | NEVER |
| Data-then-qualification | rare | rare | **YES** | rare | NEVER |
| Scope limitation with negative clarification | rare | rare | **YES** | **YES** | rare |
| Country-tier comparison ladder | YES | rare | **YES** | rare | NEVER |
| Lifecycle / procedural structure | NEVER | NEVER | NEVER | NEVER | **YES** |
| Caveat section before analysis | rare | rare | rare | **YES** | **YES** |
| Country official Preface | NEVER | NEVER | NEVER | NEVER | **YES** |

**Extended matrix — v10 genres (Employment, Trust, Commodity, Regional):**

| Fingerprint | Employment / Labour Market Evidence | Country Trust / Governance Perception | Commodity Market / Structural Price Analysis | Regional / Subnational Thematic Review |
|-------------|:-----------------------------------:|:-------------------------------------:|:--------------------------------------------:|:--------------------------------------:|
| Inline citations every 2-3 sentences | **YES, very dense** (survey + labour force data) | YES (Trust Survey + Gallup + WVS + national studies) | YES (academic + OECD WP + market data) | YES (OECD surveys + city gov docs) |
| "such as" / "including" example unfolding | YES | YES | YES | YES |
| "in practice" reflex | rare | rare | rare | rare |
| "notably" / "particularly" | rare | rare | rare | rare |
| "albeit" | rare | rare | rare | rare |
| Heavy preposition stacking | medium | medium | YES (econometric) | medium |
| Imperfect parallelism | YES | YES | YES | YES |
| Repeated technical terms | YES | YES | **YES (metal/energy terms)** | YES |
| Mid-clause "however" | medium | medium | YES | medium |
| Heavy nominalisations | medium | YES | YES | medium |
| Flat-fact paragraph endings | YES | YES | YES | YES |
| Unresolved arguments | YES | medium | YES (limitations noted) | medium |
| Dual-dimension framing ("not only X but also Y") | **YES (pay + non-pay)** | rare | rare | rare |
| Demographic disaggregation | **YES (by age/gender/sector)** | YES (by trust dimension) | rare | YES (by city/region) |
| "Areas of opportunity" + findings balance | rare | **YES (paired structure)** | rare | rare |
| Three-part analysis structure | rare | rare | **YES (stated explicitly)** | rare |
| Forward-trajectory qualifier (fingerprint T) | YES | medium | **YES (energy transition)** | YES |
| Understated causal link (fingerprint S) | **YES (long evidence chains)** | YES | YES | medium |
| Progress taxonomy ("not yet, but under development") | rare | rare | rare | **YES** |
| Multi-level governance cascade (logic AI) | YES | YES | rare | **YES (city/region/national)** |
| Specific-case deep-dive "In the case of" (logic AJ) | YES | YES | rare | **YES (Flanders, Leuven, etc.)** |

**Extended matrix — v11 genres (Gender Equality, Education Diagnostic, Revenue Statistics, SME Financing):**

| Fingerprint | Gender Equality Policy Roadmap | Education Diagnostic / PISA Study | Revenue Statistics / Tax Data Report | SME Financing Scoreboard |
|-------------|:-----------------------------:|:---------------------------------:|:-----------------------------------:|:------------------------:|
| Inline citations every 2-3 sentences | LOW-MED (OECD instruments + country evidence) | **YES, dense** (PISA tables + methodology notes) | LOW (data source annexes + StatLink 2) | LOW-MED (OECD Scoreboard + national survey data) |
| "such as" / "including" example unfolding | YES (in recommendation items) | YES | YES (tax category breakdowns) | YES (financing instruments) |
| "in practice" reflex | rare | rare | rare | rare |
| "notably" / "particularly" | rare | rare | rare | rare |
| "albeit" | **NEVER** | rare | rare | rare |
| Heavy preposition stacking | medium | medium | YES (tax terminology) | YES (financial terminology) |
| Imperfect parallelism | YES (bullet items) | YES | YES (country-by-country bullets) | YES |
| Repeated technical terms | YES (policy terms) | YES (PISA terminology) | **YES (tax categories)** | **YES (financing instruments)** |
| Mid-clause "however" | rare | medium | rare | medium |
| Heavy nominalisations | medium | medium | YES | medium |
| Flat-fact paragraph endings | YES | YES | YES | YES |
| Unresolved arguments | medium | YES (limitations section) | YES (ratio caveats) | YES |
| Bullet-dominant recommendation structure | **YES (primary structure)** | rare | rare | rare |
| "EU / OECD Member States are encouraged to act on" | **YES (canonical header)** | NEVER | NEVER | NEVER |
| Feedback-loop cross-domain causal chains | **YES ("gaps in one area have repercussions")** | rare | rare | rare |
| Mixed-pattern rise-fall-recovery data narrative | rare | **YES (PISA score arcs)** | rare | rare |
| Relative-position + absolute-loss framing | rare | **YES ("above OECD average but reversal")** | rare | rare |
| Country-comparison ladder with Nordic/Benchmark reference | rare | **YES ("In the Nordic region...")** | rare | rare |
| Methodology "Note:" blocks after every table | rare | **YES (PISA table conventions)** | **YES (average scope, excluded countries)** | YES |
| Ratio-decomposition caveat ("the numerator / denominator") | NEVER | NEVER | **YES (T60)** | rare |
| "Several factors contribute to / may explain" (T61) | rare | rare | **YES (multi-cause enumeration)** | rare |
| Country-by-country bullet analysis (each ≥1.0 p.p.) | NEVER | NEVER | **YES (primary structure)** | rare |
| Fiscal-year reporting caveat (T62) | NEVER | NEVER | **YES (Caribbean, Bahamas)** | NEVER |
| Box-format methodology explanations | NEVER | rare | **YES ("Box 1.1: The tax-to-GDP ratio")** | YES |
| Median-based cross-country summary | NEVER | NEVER | rare | **YES ("Scoreboard median")** |
| Quarter-level temporal granularity | NEVER | NEVER | rare | **YES ("In Q4 2023...")** |
| Mixed-signal macro framing ("While X has begun to moderate, Y lingers") (T58) | rare | rare | rare | **YES (macro context)** |
| Government policy response inventory | rare | NEVER | NEVER | **YES (guaranteed loans, VC, programmes)** |

**Extended matrix — v12 genres (Lobbying Regulation, Scenario Planning, Disaster Risk, AI Skills, Cash Management, Behavioural Science):**

| Fingerprint | Regulatory Compliance / Indicator-Based Assessment | Scenario Planning / Futures Study | Disaster Risk / Climate Vulnerability | AI Skills Demand / Labour Market Tech | Government Cash / Liquidity Management | Behavioural Science / Nudge Evidence |
|-------------|:--------------------------------------------------:|:---------------------------------:|:-------------------------------------:|:-------------------------------------:|:--------------------------------------:|:------------------------------------:|
| Inline citations every 2-3 sentences | LOW-MED (PMR database refs) | LOW-MED (OECD CERI + working papers) | **YES, very dense** (academic + IPCC + OECD) | **YES, dense** (OJP data + academic) | LOW-MED (country survey data) | **YES, dense** (RCT/experiment refs) |
| "such as" / "including" example unfolding | YES (requirement lists) | YES | YES (hazard types) | YES (skill categories) | YES (institutional options) | YES (bias types) |
| "in practice" reflex | rare | rare | rare | rare | rare | rare |
| "notably" / "particularly" | rare | rare | rare | rare | rare | rare |
| "albeit" | **NEVER** | **NEVER** | rare | rare | rare | rare |
| Heavy preposition stacking | medium | medium | YES (geographic terms) | YES (technical terms) | YES (financial/institutional) | medium |
| Imperfect parallelism | YES | YES | YES | YES | YES | YES |
| Repeated technical terms | **YES (PMR indicators)** | medium | **YES (hazard terminology)** | **YES (skills taxonomy)** | **YES (cash management terms)** | YES (behavioural terms) |
| Mid-clause "however" | rare | rare | rare | medium | rare | rare |
| Heavy nominalisations | medium | LOW (narrative style) | medium | medium | YES | medium |
| Flat-fact paragraph endings | YES | YES | YES | YES | YES | YES |
| Unresolved arguments | YES (de jure vs enforcement) | YES (scenario uncertainty) | YES (data limitations) | YES (data caveats) | YES (context-dependency) | YES (context-dependency) |
| Roman numeral enumeration in running text | **YES (i, ii, iii, iv)** | rare | rare | rare | rare | rare |
| "What if…" transformative-vision sentences | NEVER | **YES (T66, chapter headings)** | NEVER | NEVER | NEVER | NEVER |
| "Meet [Name] and [Name]" persona introductions | NEVER | **YES (T67)** | NEVER | NEVER | NEVER | NEVER |
| Multi-hazard cascade chains (logic AQ) | NEVER | NEVER | **YES (primary structure)** | NEVER | NEVER | NEVER |
| Physical geography paragraphs in introduction | NEVER | NEVER | **YES (2-3 paragraphs)** | NEVER | NEVER | NEVER |
| Specific disaster event citations with casualties | NEVER | NEVER | **YES (casualty counts, dates)** | NEVER | NEVER | NEVER |
| Methodology comparison section (3-4 alternatives) | rare | rare | rare | **YES (mandatory)** | rare | rare |
| "Some caveats apply when using [data source]" | rare | rare | rare | **YES (before results)** | rare | rare |
| Cross-country validation of national trends | rare | rare | rare | **YES ("shared with other countries")** | rare | rare |
| Anti-prescriptive positioning ("no single optimal model") | rare | rare | rare | rare | **YES (AP, primary stance)** | rare |
| Visibility-asymmetry logic ("X is widely discussed, Y is less visible") | rare | rare | rare | rare | **YES (AO)** | rare |
| Definitional-divergence framing ("countries diverge on basic definitions") | rare | rare | rare | rare | **YES** | rare |
| Dual Foreword (national + OECD) | rare | **YES (national official + OECD)** | rare | rare | **YES (dual directors)** | rare |
| Glossary chapter | rare | rare | rare | rare | **YES** | rare |
| Preface by national official (personal voice) | rare | **YES (mandatory)** | rare | rare | rare | rare |
| Stakeholder survey with percentage findings | rare | **YES (100% rated...)** | rare | rare | rare | rare |
| Three-tier action structure (transformation → first steps → specific) | rare | **YES** | rare | rare | rare | rare |
| Experimental evidence citation (RCTs, field experiments) | NEVER | NEVER | NEVER | NEVER | NEVER | **YES (primary evidence)** |
| "Behavioural insights" as term of art | NEVER | NEVER | NEVER | NEVER | NEVER | **YES (mandatory)** |

**How to use this matrix.** Before writing or rewriting, identify the target genre:
- **Economic Survey / Survey chapter**: full §1.9 fingerprint set, drier register, no warmth
- **Education / Health Country Review**: warmer tone allowed, citations heavy in Education / lighter in Health, no "albeit" or "inter alia"
- **Country Profile / Cancer Profile / GaaG note**: dashboard prose, abstract opening allowed (see §9.3), bullet-friendly recommendations, no Latinate connectives
- **Working Paper**: "we" voice, JEL codes, methodological hedging, citations to academic literature, less Survey-style softening
- **Policy Primer / Brief**: question-form headings, bullet recommendations, accessible register, **no inline citations**, "in summary" allowed
- **Peer Review (Anti-Bribery Phase reports, NCPE etc.)**: full Survey-style fingerprint set, heavy "in practice", peer-review evaluative verbs
- **Empirical Survey Report** (§9.16): balanced abstract ("one hand / other"), question-form section titles, country-tier comparison ladders, "this is also the first study to…"
- **Country Governance Study** (§9.17): temporal evolution narrative, "from an OECD perspective" marker, three-level sub-section numbering, constitutional/legal provisions quoted
- **Annual Data / Trends Report** (§9.18): hypothesis enumeration, data-then-qualification, "it will be a trend worth monitoring", scope limitations with negative clarification
- **Metric Assessment Report** (§9.19): three-type classification, three-factor divergence explanation, "Prior considerations" section, explicit scope exclusions
- **Operational Guidance Manual** (§9.20): country official Preface, lifecycle structure, minimum-requirements enumeration, caveat section, country examples as evidence
- **Employment / Labour Market Evidence** (§9.29): dual-dimension framing (pay + non-pay conditions), demographic disaggregation by age/gender/sector, understated causal links (fingerprint S), very dense survey citations, policy disclaimer at section end (T52)
- **Country Trust / Governance Perception Study** (§9.30): governance position vs OECD peers as opening anchor, "areas of opportunity" paired with main findings, balanced evaluative tone, multi-source survey data (Trust Survey + Gallup + WVS)
- **Commodity Market / Structural Price Analysis** (§9.31): three-part analysis structure stated explicitly in abstract, forward-trajectory qualifiers on energy transition (fingerprint T), "a key distinction to note is that" framing, numbered future research directions, limitations caveats
- **Regional / Subnational Thematic Review** (§9.32): definitional paragraph with survey methodology, progress taxonomy ("not yet, but under development"), multi-level governance cascade (logic AI), specific-case deep-dives "In the case of" (logic AJ), city/region data
- **Gender Equality Policy Roadmap** (§9.33): bullet-dominant recommendation structure, "are encouraged to act on" canonical header, feedback-loop cross-domain causal chains, em-dash expansions within bullet items, life-course approach framing
- **Education Diagnostic / PISA Study** (§9.34): mixed-pattern rise-fall-recovery data narrative, relative-position + absolute-loss framing, country-comparison ladder with regional benchmarks, PISA table-note conventions with statistical significance, explicit "Limitations" section distinguishing association from causation
- **Revenue Statistics / Tax Data Report** (§9.35): ratio-decomposition caveat (T60), "Several factors contribute to" multi-cause enumeration (T61), country-by-country bullet analysis for outliers ≥1.0 p.p., fiscal-year reporting caveats (T62), StatLink 2 URLs, Box-format methodology explanations
- **SME Financing Scoreboard** (§9.36): median-based cross-country summary (not mean), quarter-level temporal granularity, mixed-signal macro framing (T58), government policy response inventory, institutional investor classification taxonomy
- **Regulatory Monitoring / Indicator-Based Assessment** (§9.37): roman numeral enumeration in running text, "Only X% of N countries surveyed" prevalence formula, dual-extreme outlier framing (leaders + laggards), de jure/enforcement caveat (fingerprint W), "A staggering X%" for exceptional findings
- **Scenario Planning / Futures Methodology Study** (§9.38): "What if…" transformative-vision sentences (T66), "Meet [Name]" persona introductions (T67), dual Preface (national official + OECD), stakeholder survey percentages, three-tier action structure, anti-prescriptive participatory co-creation
- **Disaster Risk / Climate Vulnerability Assessment** (§9.39): 2-3 paragraphs of pure physical geography in introduction, multi-hazard cascade chains (logic AQ), specific disaster event citations with casualty counts and dates, compound hazard framing, country-by-country parallel policy structure
- **AI Skills Demand / Labour Market Technology Analysis** (§9.40): methodology comparison section (3-4 alternatives), "some caveats apply" data-limitation disclaimer, cross-country validation of national trends, counterintuitive findings with data literacy (T68), skills co-occurrence network analysis
- **Government Cash / Liquidity Management Practice Review** (§9.41): "no single optimal model" anti-prescriptive positioning (AP), visibility-asymmetry logic (AO), definitional-divergence framing, dual Foreword (national + OECD), glossary chapter, institutional taxonomy tables with staff headcounts
- **Behavioural Science in Policy / Nudge Evidence Review** (§9.42): "behavioural insights" as term of art, experimental evidence citations (RCTs, field experiments, A/B tests), step-by-step implementation guidance, context-dependency caveats for experimental findings

**The most important rule**: if the input source genre is Policy Primer, do **not** rewrite it into Economic Survey style by injecting "albeit", "thereby", and dense citations. That is genre confusion, not OECD style. Match the host genre.

---

The fingerprints below are documented in their **maximum-application form (Economic Survey / Peer Review)**. For other genres, refer to the matrix above and dial back accordingly.

#### A. Citation density (the single strongest fingerprint)

A typical OECD Economic Survey contains **600–800 inline citations** in 60-90 pages — roughly **one citation every 2–3 sentences** in analytical paragraphs. AI default output is citation-sparse.

**Rule**: in any analytical paragraph, every empirical claim should carry an inline citation: `(OECD, 2024)`, `(IMF, 2024)`, `(Banco de Portugal, 2025)`, `(Smith et al., 2023)`. Repeated authors in the same paragraph are normal — "(OECD, 2024)" can appear 3-4 times in a single dense paragraph. Do not paraphrase to avoid repeating the citation; OECD repeats.

**Repeated-author signature pattern**:
> "These reforms reflect long-standing OECD recommendations (OECD, 2019). The implementation of spending reviews has progressed (OECD, 2024). However, monitoring of results remains uneven (OECD, 2024; Tribunal de Contas, 2024)."

If the source data has no citations, **add plausible institutional sources** drawn from the topic area (OECD, IMF, World Bank, EC, ILO, UNDP, central bank, national statistics office) where the user's underlying facts would have come from. **Do not invent specific paper titles**, but `(OECD, 2024)` style attribution is conventional and expected.

#### B. The "such as" reflex (high-frequency example unfolding)

OECD authors compulsively unfold examples. In each Economic Survey, "**such as**" appears **180-350 times**, "**including**" appears **300-500 times**, and "**for example**" appears **40-80 times**. AI default prose is far less example-dense.

**Rule**: every general claim is followed by 2-4 concrete examples introduced by "such as", "including", "e.g." (in parentheses), or "for example". "For instance" is used but less frequently than these three.

> "Several sectors, **such as** manufacturing, construction, and tourism, have faced labour shortages."
> "Other OECD countries, **including** Germany, France, and the Netherlands, have adopted similar measures."
> "Vulnerable groups, **for example** older workers, lone parents, and persons with disabilities, face higher poverty risk."
> "…critical gaps persist in accessing rural housing **e.g.** water, housing, land use."

**Frequency note**: "e.g." is the most frequent example-introduction marker in OECD parenthetical usage (43–147 per report), often appearing inside parentheses after a general term. "Such as" is the most frequent in-line marker (91–468 per report). Use "e.g." for parenthetical examples and "such as" for in-line examples.

#### C. The "in practice" qualifier (reality check)

"**In practice**" appears **20-80 times** per OECD report. It signals the gap between formal rules and observed behaviour — a distinction central to OECD analytical mode. AI default prose rarely reaches for this phrase.

> "Formal independence by law is not enough; **in practice**, regulators may experience 'pinch points' over time."
> "**In practice**, expertise and experience in foreign bribery cases remain concentrated in a small number of teams."
> "The system covers all citizens; **in practice, however**, take-up rates remain below 25%."

Use it once or twice per page in policy analysis.

#### D. Heavy preposition stacking (the OECD prose texture)

Real OECD prose contains **prepositional phrase chains** that AI tends to smooth out into cleaner constructions. Example from a real Economic Survey:

> "The 2025 measures include compensation **of** past purchasing power losses **for** public servants and pension increases **beyond** the regular indexation rule (0.5% **of** GDP), **along with** cuts **to** personal and corporate income taxes (0.5% **of** GDP), **through** the adjustment **of** the personal income tax brackets **by** 4.6%, **above** the projected headline inflation rate, **the** strengthened youth PIT scheme **and** the lowering **of** the corporate income tax rate."

This sentence has **15 prepositional phrases** in one breath. Most AI rewrites of this content would split it into 3-4 cleaner sentences. **Do not split.** Allow long, preposition-stacked constructions to stand. This is the texture of institutional documentation.

#### E. Reluctant Latinate connectives (used sparingly but distinctively)

OECD writers reach for slightly archaic legalistic connectives that AI default prose rarely uses:
- **"albeit"** — concessive, more formal than "though": "Bulgarian incomes have continued to converge, **albeit** at a slower rate than regional peers."
- **"thereby"** — causal-purpose: "transparency supports confidence in regulation, **thereby** reducing administrative costs."
- **"inter alia"** — Latin "among other things": "Argentina has used investigative techniques, including **inter alia** search and seizure, forensic audits, and interception of communications."
- **"to that end"** / **"to this end"** — purpose marker: "**To that end**, Portugal has established a Spending Review Unit."
- **"notwithstanding"** — concessive preposition: "**Notwithstanding** these reforms, fragmentation persists."
- **"in this regard"** / **"in this respect"** — reference back: "**In this regard**, the OECD recommends…"
- **"against this background"** — context-setting: "**Against this background**, the 2025 reform package was adopted."

Use 1-2 of these per page in formal policy analysis. They are **extremely characteristic** of human-written OECD prose and absent from AI default output.

#### F. Imperfect parallelism (key fingerprint AI rarely produces)

AI defaults to **clean parallel structure** ("X, Y, and Z" all in matching grammatical form). Real OECD prose often runs slightly broken parallels — the third element shifts grammatical category, or a list mixes nouns and gerunds, or modifiers attach to only some elements.

Example from a real OECD Survey:
> "The reforms aim to improve expenditure quality, reducing inefficient tax expenditures and strengthening the use of spending reviews."

Three reform aims, in **three different grammatical forms** (infinitive "to improve", gerund "reducing", gerund "strengthening" — but with the inserted "use of" before the third element). This unevenness is human.

Another example:
> "Regional disparities persist, with limited access to specialist care, long waiting times for diagnostic procedures, and primary care that remains fragmented across municipalities."

The third element is a full clause ("primary care that remains fragmented") while the first two are noun phrases. AI defaults would smooth this to all noun phrases. **Don't smooth.**

#### G. Re-use of the same key term (vs synonym substitution)

AI is trained to vary vocabulary — to replace "framework" with "system" with "structure" with "arrangement" across consecutive sentences. **OECD does the opposite.** Key technical terms are **repeated verbatim** to avoid ambiguity.

Real example:
> "The CLL applies to legal persons. The CLL covers both domestic and foreign bribery. Under the CLL, sanctions include fines, restitution, and corporate community service."

"CLL" appears three times in three sentences. No "framework", no "law", no "regime". AI would aggressively synonym-swap. **Do not swap technical terms.**

Same with country and institution names: "Portugal" / "Portugal" / "Portugal" appears 5 times in a 200-word paragraph. Don't substitute "the country" or "the southern European economy".

#### H. Embedded qualifications (mid-sentence parentheticals)

Real OECD sentences carry **mid-clause qualifications** that AI tends to relegate to separate sentences. The "subject + auxiliary, however, predicate" pattern is one example; here are others:

> "Bank profitability **has, however, declined** since 2023."
> "Implementation, **however,** has experienced systematic delays."
> "These reforms, **important as they are,** require complementary measures to deliver results."
> "Spending, **at 28.2% of GDP,** remains below the OECD average."
> "Inflation, **after peaking at 10.6% in October 2022,** has returned to target."
> "Portugal, **like other small open economies,** is exposed to external shocks."

These mid-sentence inserts create the **stop-and-go rhythm** of human-edited prose. AI tends toward straight subject-verb-object-period.

#### I. Slightly heavy nominalisations (OECD's preferred verbosity)

Where AI defaults to verbal forms ("regulators monitor X"), OECD often nominalises ("the monitoring of X by regulators"). This is **counterintuitive** — most "good writing" advice says use verbs over nominalisations — but OECD prose is not optimised for readability; it is optimised for institutional precision.

Examples from real Surveys:
- "the **implementation** of spending reviews" (not "implementing spending reviews")
- "the **strengthening** of regulatory capacity" (not "strengthening regulatory capacity")
- "the **provision** of social benefits" (not "providing social benefits")
- "the **establishment** of inter-ministerial bodies" (not "establishing inter-ministerial bodies")
- "the **reduction** of marginal effective tax rates" (not "reducing marginal effective tax rates")

Use the heavier nominalisation **about half the time**. It signals the institutional register that AI undershoots.

#### J. Unresolved sentences (claims that don't fully argue themselves)

AI default prose tends to **complete every argument**: claim → evidence → resolution. Real OECD prose often **states a fact and moves on**, leaving the implication for the reader.

Example:
> "Spending on prevention amounts to less than 2% of health spending. Around 12.8% of the population is not registered with a dedicated general practitioner. The excessive use of emergency rooms drives up costs without promoting better health outcomes."

Three facts, no resolution. The implications are obvious to the policy-literate reader. AI would add: "Together, these factors suggest the need for primary care reform." **Don't add.**

#### K. Strategic small typos / inconsistencies (advanced — use cautiously)

Real OECD reports contain occasional small inconsistencies: a missing Oxford comma in one list and present in the next; "U.S." vs "USA" within the same chapter; a missing space before parenthesis; "co-operation" in one paragraph and "cooperation" elsewhere; a typo like "rises" → "raises". These are not random — they are **edit-pass artefacts** from many human contributors.

**Caution**: do not deliberately introduce typos in user-facing output. But **do not over-normalise either**. If the input has minor inconsistencies, you can preserve some of them. Excessive consistency reads as machine-generated.

#### L. The "humble factual closer" (paragraph endings)

AI tends to end paragraphs with a **synthesising flourish** ("Together, these reforms underscore…"). OECD paragraphs often end with a **flat additional fact** that doesn't summarise — it just adds.

Example endings (real OECD):
- "…The minimum age for early retirement, set at 60, is not [indexed to life expectancy]."
- "…Bulgaria joined the euro area in 2026."
- "…New loans are dominated by mixed-rate agreements (at 82% of the mortgages issued in 2024)."
- "…StatLink: https://stat.link/cl5wv6"

Resist the synthesising flourish. End paragraphs with a fact, a date, a number, a name — not a moral.

#### M. The "boring alternative explanation" (OECD's analytical humility)

AI never defaults to the mundane explanation. When data shows an unexpected trend, AI reaches for a substantive causal story. OECD authors **also offer the boring possibility**.

> "This could simply be a time delay in cases feeding into the data, and it will be a trend worth monitoring in future editions of this report."
> "This is to be expected, as larger firms may be more capable of making large investments."
> "It is also possible that different perceptions about bias result from variation across firms."

Pattern: "This could simply be [mundane explanation]" / "This is to be expected, as [obvious reason]" — OECD uses "simply" and "to be expected" to signal that the boring explanation might be correct. This is a **genuine human fingerprint** — AI always prefers the more interesting interpretation. Verified in Competition Trends, Algorithmic Management. **Genre**: Universal — appears in all analytical genres.

#### N. The "does not automatically equate to" caveat (preventing over-interpretation)

AI tends to either state findings as fact or hedge with "may". OECD authors use a specific construction to prevent readers from drawing too-strong conclusions: "though it should be noted that [X] does not automatically equate to [Y]".

> "nearly two-thirds of managers have at least one concern regarding the trustworthiness of the algorithmic management tools they use (though it should be noted that concern does not automatically equate to harm)."

Pattern: "though it should be noted that [finding] does not automatically equate to [stronger claim]" — this is the OECD way of saying "don't over-read this". It is more precise than AI's "However, this does not mean..." because it names the specific logical gap. Verified in Algorithmic Management, ESG Ratings. **Genre**: Universal — appears in all analytical genres.

#### O. The "forward-looking monitoring commitment" (closing with future data)

AI tends to close sections with synthesis or implications. OECD authors close with a commitment to **watch the data in future editions**.

> "it will be a trend worth monitoring in future editions of this report"
> "it will be a trend worth monitoring in future editions of this report"
> "While for now it seems that their use is requiring additional staff, in the future, it would be worth monitoring whether this may be offset by the efficiency gains from using such tools"

Pattern: "it will be a trend worth monitoring in future editions of this report" / "in the future, it would be worth monitoring whether [X]" — OECD closes analysis with a **data-monitoring commitment**, not a policy recommendation or synthesis. This signals institutional continuity — the OECD will keep watching. Verified in Competition Trends, Algorithmic Management. **Genre**: Annual Data / Trends Reports, Empirical Survey Reports. Do NOT use in Economic Surveys or Policy Briefs (they close differently).

**P. The "complex interaction" admission (naming analytical messiness)**

Genre applicability: **Universal** — especially prominent in Survey-Based Studies, Country Philanthropy Studies, Working Papers, and Capacity Assessments.

The human author explicitly acknowledges that the data does not tell a clean story, rather than forcing a simple narrative. This is OECD's institutional version of intellectual honesty.

> "The data shows a complex interaction between poverty levels and allocation of philanthropic resources."
> "The share of variation explained by the model is low, which suggests a complex relationship between funding allocation and poverty levels."

AI forces clean narratives from messy data. OECD **names the messiness** and lets the reader draw their own partial conclusions. Verified in Philanthropy Study, Working Paper (Regulatory Compliance). **Deploy once per data-analysis section when the data genuinely does not support a simple causal claim.**

**Q. The "scope limitation" transparency signal (naming what the data cannot do)**

Genre applicability: **Universal** — prominent in Working Papers, PMR Evidence Papers, Survey-Based Studies, Capacity Assessments.

The human author explicitly states the boundaries of the data or analysis, preventing over-interpretation. This is distinct from hedging (§1.6) which qualifies the strength of a claim; the scope limitation names what the analysis **does not cover at all**.

> "While this paper does not provide a monetary quantification of all the benefits derived from regulatory policy, it then aims to relate the costs estimated above to general measures of economic performance."
> "It must be stressed that the PMR indicators measure the 'de jure' policies, but not actual enforcement."
> "Although the organisational survey had a relatively low response rate – requiring caution when drawing definitive conclusions – the overall sample size is comparable to OECD studies in other emerging economies."

Pattern: "While / Although [scope limitation], [what the analysis DOES cover / why the findings are still useful]." — Always a concessive structure. The limitation comes first; the value proposition follows. AI tends to hide limitations in footnotes; OECD **puts them in the main text, prominently**. Verified in PMR Evidence, Philanthropy Study, Working Paper. **Deploy once per major data section.**

**R. The "numbered recommendation" as structural anchor**

Genre applicability: **Genre-specific** — Capacity Assessment, Governance Review, Operational Guidance, RBC Country Reports. **Never** in Economic Surveys, Policy Briefs, or Working Papers.

The human author uses bolded, numbered recommendations as the primary structural unit of the text. Each recommendation is a standalone imperative, followed by an explanatory paragraph with context and evidence.

> "**Recommendation 4.** If, reflecting cost or related considerations, a combined R&D and innovation survey remains the preferred method, an appropriate hybrid sampling and estimation design should be promptly developed."
> "**Recommendation 8.** An easily understood Business R&D and Innovation Survey Methodology Report should be readily available to researchers and survey practitioners."

Key features:
- Recommendations use "should" (never "must" or "could")
- They include qualifying conditions ("If…", "In view of…") or purpose clauses ("to produce statistically robust…")
- They are numbered sequentially and referenced by number in the text
- The explanatory paragraphs provide **evidence** for the recommendation, not just restatement

AI defaults to unnumbered bullet-point recommendations or "best practice" statements. OECD uses **numbered, conditional, evidence-backed imperatives**. Verified in Capacity Assessment (Egypt STI), Digital Governance Guidance (Ireland). **Deploy only in the genres listed above.**

**S. The "it may then come at little surprise" understated-causal-link (presenting findings as self-evident)**

Genre applicability: **Universal** — especially prominent in Employment Policy Papers, Trust Studies, Commodity Market Papers, and any analytical genre with a long evidence chain.

The human author builds a long chain of evidence across multiple paragraphs, then delivers the conclusion as if it were self-evident — not by asserting causation, but by letting the reader draw the inference. This is OECD's institutional version of "show, don't tell."

> "It may then come at little surprise to observe increased labour shortages in this sector, especially as the pandemic acted as an eye opener about the pressures endured by the profession."
> "Given the similar importance of Russia in the production of both metals, one might have expected a comparable response in terms of price volatility."

AI never produces this pattern. AI either (a) asserts causation directly ("This caused X"), (b) hedges weakly ("This suggests X"), or (c) over-explains the link. OECD **trusts the reader** to see the connection from the evidence laid out. Verified in Labour Shortages, Commodity Market WP. **Deploy once per long analytical section where the evidence chain is strong.**

**T. The "at present... however, as [X] progresses" forward-trajectory qualifier**

Genre applicability: **Universal** — prominent in Commodity Market Papers, Circular Economy Reviews, Trust Studies, and any document analysing evolving dynamics.

The human author describes the current state as bounded or limited, then immediately flags that this state could change as a dynamic process unfolds. This is NOT the same as the "forward-looking monitoring commitment" (fingerprint O), which promises future observation. The forward-trajectory qualifier **warns the reader that the current finding may not hold**.

> "At present, the use of derivatives in metal markets remains largely limited to financial markets and the mining sector. However, as the energy transition progresses, the need to hedge against metal price volatility is likely to expand."
> "While these metals do not currently exhibit impacts beyond prices, this may change as critical minerals become crucial for energy generation."
> "While Australia has so far managed to avoid extreme polarisation, there are indications that efforts to prevent further social fragmentation should remain a priority."

Pattern: "At present / Currently / So far, [X] remains [limited]. However, as [dynamic process] progresses, [X] is likely to [expand/change]." — AI describes the current state and stops. OECD describes the current state **and** immediately flags the trajectory. Verified in Commodity Market WP, Circular Economy, Trust Study. **Deploy when the current state is not representative of future conditions.**

**U. The "N in M" population-prevalence converter**

Genre applicability: **Universal** — prominent in Gender Equality Reports, Education Reviews, Financing Scoreboards, and any document presenting survey findings with policy salience.

The human author converts a percentage into a human-scale "N in M" or "N out of M" fraction to make the prevalence immediately tangible to non-technical readers. This is distinct from simple percentage reporting — it adds a layer of institutional pedagogy.

> "A record 8 in 10 SMEs (78%) reported an increase in interest rates in 2023."
> "About a third of students stated that they were distracted by classmates in most or nearly all lessons."
> "With 32% of women reporting feeling unsafe while walking alone at night."

AI tends to report only the percentage. OECD **also provides the "N in M" equivalent** when the finding is policy-relevant and the audience needs to grasp scale. The parenthetical percentage follows for precision. Verified in Gender Equality, Financing SMEs, Education Sweden. **Deploy when presenting survey findings with high policy salience.**

**V. The "Note:" methodology footnote as in-text transparency block**

Genre applicability: **Genre-specific** — Revenue Statistics, National Accounts, PISA Reviews, Financing Scoreboards, and other data-heavy reports.

The human author places a "Note:" block immediately after a data table or figure, explaining: (a) how the average is calculated (weighted vs unweighted), (b) which countries are excluded and why, (c) what the denominator represents, and (d) any data revisions. This is not a footnote — it is a structured in-text block with its own conventions.

> "Note: The LAC average represents the unweighted average of 26 LAC countries included in this publication and excludes Venezuela due to data availability issues. The OECD average represents the unweighted average of 38 OECD member countries."
> "Note: Statistically significant values are indicated in bold. The OECD average is based on data from 35 member countries. The average decennial trend is the average change, per 10-year period..."

AI rarely includes this level of methodology transparency in the main text. OECD **always includes it** because the audience includes policymakers who need to know exactly what the numbers represent. Verified in Revenue Statistics, Education Sweden. **Deploy only in data-heavy genres — never in analytical prose.**

**W. The "it must be stressed that [indicator] measures [X], but not [Y]" de jure / enforcement caveat**

Genre applicability: **Genre-specific** — PMR Evidence Papers, Regulatory Compliance Briefs, Indicator-Based Assessment Reports, and any document that uses quantitative indicators of regulatory quality.

The human author explicitly warns that the indicator measures what is written on paper, not what is enforced in practice. This caveat is placed in conclusions or methodology sections, not in footnotes. It is a signature of institutional intellectual honesty — the OECD acknowledging the limits of its own measurement tools.

> "It must be stressed that the PMR indicators measure the 'de jure' policies, but not actual enforcement. Therefore, countries with competition-friendly regulatory frameworks 'on paper' may score well, even if implementation is lacking."
> "Countries with competition-friendly regulatory frameworks 'on paper' may score well, even if implementation is lacking."

AI tends to either ignore the gap between regulation and enforcement, or overstate it. OECD **names it precisely and briefly** — one or two sentences, then moves on. Verified in Lobbying Regulation, PMR Evidence. **Deploy once per indicator-based assessment paper, in the conclusion or limitations section.**

**X. The "[institutional unit] chaired by [name and title], [institution], and supported by [secretariat]" governance-attribution block**

Genre applicability: **Genre-specific** — Practice Reviews, Institutional Surveys, Working Party Reports, Ad Hoc Group Reports, and any document produced by a multi-country expert group.

The human author credits the governance structure of the producing entity with extreme precision: the chair's name, title, and institutional affiliation; the sub-group leaders; the number of countries; the duration of work. This is not acknowledgements boilerplate — it is a genre-defining structural element that establishes the report's institutional authority.

> "Chaired by Thomas Anthony Linehan, WPDM vice-chair and Deputy Director of Ireland's Funding and Debt Management in the National Treasury Management Agency (NTMA), the group operated with the support of the OECD Secretariat for approximately 12 months between November 2023 and November 2024."
> "The group consists of delegates from 22 OECD and OECD accession countries with specific experience in or responsibility for cash management."

AI tends to write generic acknowledgements. OECD **embeds institutional authority in the governance description** — the specific number of countries, the exact duration, the named chair with full title. Verified in Managing Government Cash. **Deploy in Foreword or Acknowledgements of practice-review and institutional-survey genres.**

#### Summary: the human-fingerprint checklist

After purging AI defaults from §1.8, deliberately add:
- [ ] Inline citations every 2-3 sentences in analytical prose: `(OECD, 2024)`, `(Source, year)`
- [ ] At least one "such as" or "including" example unfolding per paragraph
- [ ] At least one "in practice" or "to date" or "in particular" per page
- [ ] At least one heavy preposition-stacked sentence per section (resist the urge to split)
- [ ] At least one Latinate connective per page ("albeit", "thereby", "notwithstanding", "to that end")
- [ ] Imperfect parallelism in at least one list per section
- [ ] Repeated technical terms — no synonym swapping for "CLL", "RRP", country names
- [ ] Mid-sentence parenthetical qualifications ("Implementation, however, has…")
- [ ] Heavy nominalisations roughly half the time ("the implementation of" not "implementing")
- [ ] At least one "complex interaction" admission per data section (fingerprint P) — name the messiness when data doesn't tell a simple story
- [ ] At least one "scope limitation" transparency signal per major data section (fingerprint Q) — state what the analysis does NOT cover, in the main text
- [ ] In capacity/governance genres: numbered, bolded "Recommendation N" with qualifying conditions (fingerprint R)
- [ ] At least one "it may then come at little surprise" understated causal link per long analytical section (fingerprint S) — trust the reader to see the connection
- [ ] At least one "at present... however, as [X] progresses" forward-trajectory qualifier per section on evolving dynamics (fingerprint T) — warn that current state may not hold
- [ ] At least one "N in M" population-prevalence converter per survey-finding presentation (fingerprint U) — make the percentage tangible to non-technical readers
- [ ] In data-heavy genres: "Note:" methodology blocks after every table/figure (fingerprint V) — explain weighted/unweighted averages, excluded countries, data revisions
- [ ] In indicator-based assessment papers: "It must be stressed that [indicator] measures [X], but not [Y]" caveat (fingerprint W) — acknowledge the gap between de jure and enforcement
- [ ] In practice-review / institutional-survey genres: governance-attribution block with chair name, title, institution, number of countries, duration (fingerprint X) — establish institutional authority
- [ ] At least one paragraph ending with a flat fact, not a synthesising sentence
- [ ] No paragraph "completes every argument" — leave some implications unstated
- [ ] At least one "boring alternative explanation" per analytical section ("This could simply be…") — AI never defaults to the mundane
- [ ] At least one "does not automatically equate to" caveat per data-heavy section — prevent over-interpretation
- [ ] Annual/Trends reports: close analytical sections with "it will be a trend worth monitoring in future editions" — institutional continuity signal

These are **the fingerprints AI detectors don't catch but AI-text feels missing**. They are also what makes formal institutional prose feel **human-produced** rather than smooth-generated.

---

## 2. Sentence Patterns (句式)

OECD syntax is built from **a finite set of sentence templates**, recombined endlessly. Learning to write OECD prose is largely learning to recognise and deploy these templates.

### 2.1 The eight core sentence templates

**T1. Quantified state**
> [Subject] + [state verb: stand at / amount to / account for / represent] + [number] + [unit + benchmark + year]

> Canada's gross debt **stood at** 117% of GDP at the end of 2024.
> ODA for social infrastructure **totalled** USD 1.7 billion.
> Microenterprises **accounted for** 92.6% of all enterprises in Ireland.

**T2. Quantified change**
> [Subject] + [trend verb] + [magnitude adverb] + [comparator phrase]

> Bank profitability **has declined since 2023** due to increased funding costs.
> Total ODA **decreased in 2024** to USD 7.5 billion, representing 0.62% of GNI.
> The labour market **has softened** with job vacancies **coming down**.

**T3. Concession + main claim**
> [Acknowledgement of positive/negative fact], **However / Nevertheless / At the same time**, [contrasting claim].

> Canada's economy has been resilient, with growth picking up over 2024. **However**, its per capita GDP performance has lagged behind other OECD countries in recent years.
> Argentina has made legislative progress. **Nevertheless**, foreign bribery enforcement remains limited and uneven.
> While Argentina has opened 18 formal investigations, **many cases have not progressed beyond investigation**.

**T4. Evidence-to-cause**
> [Observable fact / data point]. **This reflects / This is driven by / This is due to** [causal explanation].

> House prices and rents have increased more strongly than in most other OECD countries. **This is due to** an insufficient supply of housing and a mismatch between available housing and demand.
> Reporting of public debt within Canada focuses mostly on net public debt. **This reflects the fact that** Canada has important financial asset holdings.

**T5. Recommendation with rationale**
> [Subject = institution / instrument] + **should** + [verb] + [object]. [Optional rationale clause].

> The preferential corporate tax rate for SMEs **should be discontinued** and R&D incentives **harmonised** across firms.
> Canada **should reapply** the fuel charge and **improve** communication on the benefits of the system.
> OSFI **should stay vigilant** and **maintain** stringent regulation given the significant mortgage market risks.

**T6. Parallel-mechanism enumeration (semicolon tricolon)**
> [Topic sentence]. [Stage 1 with action]; [Stage 2 with action]; [Stage 3 with action].

> These instruments apply at different stages of a drug's commercial lifecycle. At market entry, regulators negotiate prices and conduct pharmacoeconomic assessments; during the period of patent exclusivity, rebate arrangements contain cost growth; once patents expire, generic and biosimilar substitution brings prices down further.

**T7. Comparative anchoring**
> [Country/region/entity] + [verb] + [number] + **above / below / compared to** + [benchmark: OECD average / other countries / previous year].

> Chile **scored 1.7 on the index, improving from 0.34 in 2013 but below the OECD average of 2.3**.
> Norway's explicit carbon prices **reach an average of EUR 79.18 per tonne of CO₂**.
> The region's GDP per capita **is 42% below the national average**.

**T8. Risk / vulnerability framing**
> [Risks / challenges / vulnerabilities] + [remain / persist] + [adverb], + **and warrant** + [action].

> Risks, particularly those related to the domestic mortgage market, **remain significant and warrant** careful oversight.
> Persistent delays **are compounded by** structural capacity constraints, including a significant number of judicial vacancies.

### 2.2 Sentence length and rhythm (节奏)

OECD prose breathes. Average sentence length sits at 25–40 words, but **uniformity is forbidden**. Each paragraph alternates lengths.

**The five-beat rhythm pattern** (typical OECD paragraph)
```
■■■■■■■■■■■        (中长 25-35w，定调 — topic sentence with quantification)
■■■                (短 ≤12w，承接 — pivot, fact, or country anchor)
■■■■■■■■■■■■■■■    (长 40-60w，分号并列 — parallel mechanisms via semicolons)
■■■■               (短-中 12-20w，国别落地 + 引用)
■■■■■■■■■■         (中长 25-35w，导向 — implication or recommendation)
```

**Concrete signature short sentences (≤ 12 words)** — these appear repeatedly:
- "Risks of sovereign stress are limited."
- "These measures are welcome."
- "The financial system has proven resilient."
- "Inflation has returned to the target rate."
- "Labour market pressures have eased."
- "No action taken."
- "These initiatives are welcome and should be continued."

These short sentences **anchor the paragraph** and create rhythmic contrast with the long sentences around them.

**Long sentence structure**: when sentences run long (40+ words), they are held together by **parallel structure** (semicolons, "as well as", "while", "and"), not nested subordination. Avoid more than two levels of clause nesting.

**Comma rhythm within sentences**: OECD long sentences typically have 3–5 commas creating internal pauses, often around inserted clauses ("which is", "particularly", "including", "such as", "for example", "notably").

### 2.3 Subject choice (主语策略)

OECD prefers **concrete, named subjects** because they make claims feel grounded and verifiable. Abstract-noun subjects (the framework, the interplay, the system, the toolkit) feel evasive and are flagged as a failure mode.

**Preferred subject types**, in rough order of frequency:
1. **Country / region**: "Canada", "the Netherlands", "the Western Region", "OECD members"
2. **Institutions**: "the Bank of Canada", "OSFI", "the Working Group on Bribery", "the European Commission"
3. **Specific instruments / mechanisms**: "the federal carbon pricing system", "rebate arrangements", "the Corporate Liability Law", "spending reviews"
4. **Measurable quantities / indicators**: "house prices", "the gross debt-to-GDP ratio", "ODA", "GHG emissions"
5. **People / actors** (when relevant): "households", "lenders", "firms", "auditors", "whistleblowers"
6. **Acts / events**: "this measure", "the 2025 reform", "Argentina's first foreign bribery conviction"

**Acceptable abstract subjects** (use ≤ once per paragraph):
- "The data show / suggest / indicate"
- "Available evidence points to"
- "The OECD recommends"
- "Recent estimates indicate"

**Discouraged abstract subjects** (likely to make prose feel hollow):
- "the framework reflects"
- "the interplay shapes"
- "the toolkit operates"
- "the dynamics drive"
- "the ecosystem enables"
- "the architecture supports"

### 2.4 Voice (语态) — active is the default, not passive

**Common misconception**: OECD prose is institutional and therefore mostly passive. **Wrong.** Real OECD prose is **predominantly active**, with passive used sparingly for specific functions. Inspect any policy brief and you will find roughly **70–80% active voice**.

**Why active dominates**: OECD writers care about **agency** — who acts, who decides, who reforms. Passive voice obscures the agent and makes prose feel evasive. Country names, institutions, and indicators are deliberate subjects of action verbs.

**Active voice is the default for**:
- Country / institution behaviour: "Criminals use sophisticated concealment methods.", "Canada has made considerable progress.", "The OECD convenes policymakers."
- Trend descriptions: "House prices have increased.", "Inflation is moderating.", "Bank profitability has declined."
- Mechanism descriptions: "FTZs offer clear advantages.", "Maritime transport is a high-volume channel.", "Synthetic drug manufacturing is highly adaptable."
- Recommendations: "Canada should reapply the fuel charge.", "Governments must understand and address vulnerabilities."

**Use passive only for** these narrow purposes:
- Established procedures with no relevant agent: "Evaluations are shared with the parliament", "Mortgage lending is regulated by OSFI"
- Citations / data attribution: "USD 7.5 billion was allocated to least developed countries"
- When the patient (the thing acted upon) is genuinely the topic: "These reforms have been adopted by 18 countries"

**Diagnostic**: count the passive constructions in any draft paragraph. If more than **2 in 5 sentences** are passive, the prose has slipped into Brussels-bureaucratese, not OECD style. Convert most back to active by naming the agent.

**Passive-to-active examples**:
- ✗ "These instruments are deployed at successive stages."
- ✓ "These instruments apply at successive stages." (or: "Regulators apply these instruments at successive stages.")

- ✗ "Considerable progress has been made by Canada."
- ✓ "Canada has made considerable progress."

- ✗ "It is widely recognised that..."
- ✓ "Available evidence indicates..." (or simply drop the framing and state the fact)

- ✗ "These findings are broadly consistent with the wider literature."
- ✓ "The wider literature reaches similar conclusions." (or: "Comparative studies of European reimbursement systems reach similar conclusions.")

### 2.5 Opening moves (篇首句策略)

The first sentence of any paragraph or section sets **the tone of fact**, not the tone of argument. OECD never opens with conceptual framing.

**Good opening types**:

**O1. Stated fact**
> "Cost-containment measures for pharmaceuticals are widely used in publicly financed health systems."

**O2. Quantified observation**
> "In 2024, the Netherlands ranked seventh in terms of ODA volume among DAC members."

**O3. Country status**
> "Canada's economy has been resilient, with growth picking up over 2024."

**O4. Trend**
> "House prices and rents have increased more strongly than in most other OECD countries."

**O5. Institution + action**
> "OSFI has raised the Domestic Stability Buffer to 3.5% of total risk-weighted assets in November 2023."

**O6. Specific event / milestone**
> "Argentina concluded its first foreign bribery case against a natural person in 2025."

**O7. Gerund-phrase subject (the OECD signature opener for executive summaries and recommendation sections)**
A nominalised action — gerund + object — serving as subject of "requires", "will require", "would benefit from", "is essential for". Universal in section headings and topic sentences.
> "**Strengthening Canada's productivity performance** requires a combination of policies."
> "**Tackling Portugal's housing affordability challenge** will require a comprehensive reform package."
> "**Maintaining fiscal sustainability over the longer term** is a central priority."
> "**Addressing climate change** requires significant investment in adaptation and mitigation."
> "**Increasing the effective retirement age** would help offset rising pension costs."

This pattern is especially common as the **subtitle** of an executive summary section (see §3 for full structure).

**O8. "While / Although + concession" opener**
A concessive subordinate clause first, with the main claim landing in the second half of the sentence. Carries the contrast without scaffolding.
> "**While** GDP growth has picked up, productivity performance has continued to lag."
> "**Although** progress has been made on enforcement, many cases remain pending."

**O9. Sectoral or geographic framing**
> "In the financial sector, …"
> "Across OECD countries, …"
> "At the regional level, …"
> "In the housing market, …"

**Bad opening types** (concept scaffolding — **avoid in analytical prose**, except in the country-profile genre noted in §9.3):
- "Modern economies face complex challenges..."
- "Publicly financed systems deploy a toolkit of..."
- "It is widely understood that..."
- "In today's interconnected world..."
- "The importance of [X] cannot be overstated..."

**Genre exception**: in *Government at a Glance* country notes and similar **dashboard-style country profiles**, an abstract conceptual sentence opening a section is conventional, **provided** it transitions immediately to a quantified country-vs-OECD comparison in the next sentence. Do not import this pattern into Economic Survey chapters or analytical prose — there it is the AI scaffolding flagged in §1.8. See §9.3 for genre rules.

### 2.6 Punctuation as signal (标点节奏)

**Em-dashes** for parenthetical clarification or emphasis:
> "the OECD employs gross debt due to the challenges of international comparability in asset valuation – for example, the varied approaches to estimating the assets of state-owned enterprises"

**Semicolons** for parallel mechanisms (the OECD signature move — see T6 above):
> "regulators negotiate prices; rebate arrangements contain cost growth; substitution brings prices down"

**Colons** to introduce a list or elaboration:
> "Three main challenges remain: first, ...; second, ...; third, ..."

**Parentheses** for citations, abbreviations, supplementary numbers:
> "(Bank of Canada, 2024)"
> "(USD 1.3 billion)"
> "the Corporate Liability Law (CLL)"

**Avoid**: exclamation marks, ellipses, double dashes, ampersands in running text.

### 2.7 Tense system (时态系统) — what to use when

OECD authors use a **disciplined and predictable** tense system. Each tense carries a specific epistemic function.

**Present simple** — for stable structural facts, system properties, ongoing arrangements
> "Canada **has** a federal carbon pricing system."
> "The Corporate Liability Law **applies to** legal persons."
> "Microenterprises **account for** 92.6% of all enterprises."

**Present continuous** — for active, ongoing processes
> "Inflation **is moderating**."
> "House prices **are increasing**."
> "Risks **are weighing on** the outlook."

**Present perfect** — for trends extending from the past into the present (the **most distinctive OECD tense**)
> "Canada's economy **has been resilient**."
> "Bank profitability **has declined since 2023**."
> "Argentina **has opened** 18 formal investigations since 2017."
> "House prices **have increased** more strongly than in most other OECD countries."

This tense is the workhorse of OECD analytical prose. It frames data as **established but continuing**.

**Past simple** — for completed events tied to specific dates
> "OSFI **raised** the Domestic Stability Buffer to 3.5% in November 2023."
> "ODA **decreased** in 2024."
> "Argentina **concluded** its first foreign bribery case in 2025."

**Future / projection forms**:
- "**is expected to** [verb]" — neutral projection: "GDP is expected to grow by 1.1% in 2026"
- "**is set to** [verb]" — slightly more confident: "Inflation is set to return to target"
- "**is projected to** [verb]" — for model-based forecasts
- "**will** [verb]" — for stated policy commitments: "The government will phase out the subsidy"
- "**should** [verb]" — for recommendations (not future tense): "Canada should reapply the fuel charge"

**Conditional / hypothetical**:
- "**would benefit from** [noun]" — soft recommendation
- "**could be offset by** [X]" — possibility framing
- "**should [X] materialise** ..." — conditional risk

**Tense rule of thumb**:
- Talking about the present state of a country/sector → present perfect for trends, present simple for structures
- Reporting a 2024 outcome → past simple
- Projecting to 2026 → "is expected/projected/set to"
- Recommending → "should" + bare infinitive

### 2.8 Information structure (信息结构) — end-focus

OECD sentences place the **most informative element at the end**. The reader's eye lands on the new fact, the magnitude, or the conclusion. This is called *end-focus* or *end-weight*.

**End-focus examples**:
- Weak: "Considerable progress has been made by Canada in carbon pricing."
- Strong: "Canada has made considerable progress in carbon pricing."

- Weak: "An insufficient supply of housing is the cause of rising prices."
- Strong: "Rising house prices are driven by **an insufficient supply of housing**."

**End-weight via inversion**: long, heavy phrases go to the end of the sentence:
- "Canada's economy has been resilient, **with growth picking up over 2024 and the labour market remaining tight despite some softening**."

**Information sequencing within a sentence**:
> [Given / known information] → [topic] → [comment / new information]

> "Bank profitability [given] has, however, declined since 2023 [topic shift] **due to increased funding costs and rising loan-loss provisions** [new information at end]."

### 2.9 Cohesion and flow (篇章衔接) — fixing crunchy prose

This is the single most overlooked layer. Many drafts that pass the lexical and syntactic checks still feel **crunchy** — choppy, scaffold-heavy, mechanical. The fix lies in inter-paragraph and inter-sentence cohesion.

#### Diagnostic: what makes prose crunchy?

1. **Meta-discourse scaffolding** — sentences that announce structure instead of carrying content:
   - ✗ "Two strands of debate surround this arrangement."
   - ✗ "The first concerns... The second concerns..."
   - ✗ "We now turn to..."
   - ✗ "Having discussed X, we move to Y."
   - **OECD never narrates its own organisation.** It just shifts topic and trusts the reader.

2. **Subjective evaluation injected as fact** — words that voice an opinion the OECD won't take:
   - ✗ "The data are striking / alarming / remarkable."
   - ✗ "Notably, the situation is dire."
   - **OECD lets the numbers speak.** "Only 36%" carries the weight; no need for "striking".

3. **Atomised paragraphs** — each sub-point given its own paragraph. OECD paragraphs are **dense and continuous**, often 6–10 sentences. Splitting after every shift in idea breaks rhythm.

4. **Repeated paragraph-opening rhythm** — every paragraph starting with a noun-phrase subject of similar length. Vary the openings.

5. **Dropped lexical chains** — using a different noun every time the same concept reappears. OECD repeats and lightly varies key terms ("FTZs" → "non-transparent FTZs" → "FTZs in Spain and Costa Rica") to keep the reader anchored.

#### Cohesion techniques OECD actually uses

**(a) Topic continuity through subject chaining**
The subject of a new sentence picks up a noun (or pronoun) introduced in the previous sentence's predicate. The chain creates flow without explicit connectors.

> "Maritime transport is a high-volume, low-risk channel for criminals, favoured for the transport of cocaine and other bulk drugs. **Criminals** conceal narcotics in containers, refrigerated units, and even ship structures. **At-sea transfers** are increasing, and authorities are identifying new concealment methods…"

Notice: "criminals" is the predicate of sentence 1 → subject of sentence 2. "Concealment" idea closes sentence 2 → "at-sea transfers" picks it up.

**(b) Embedded transition rather than meta-transition**
OECD tucks "however" / "by contrast" / "while" inside the sentence carrying new content, not into a standalone signpost sentence.

- ✗ Standalone signpost: "There is, however, a different perspective."
- ✓ Embedded: "The access literature, **by contrast**, draws attention to delayed availability rather than to cost-effectiveness."
- ✓ Embedded: "**While** Canada has opened 18 investigations, many cases have yet to progress beyond investigation."

**(c) "Also" / "Furthermore" / "In addition" carry heavy lifting**
A simple "also" can introduce a parallel point without paragraph rupture:
> "The rise of e-commerce and small parcel delivery services **has also** created an alternative trafficking route…"

This single word does the work of "Two strands of debate surround this arrangement."

**(d) Lexical repetition and partial substitution**
Repeat the key term, or vary it minimally. Don't reach for elegant synonyms.

> "**FTZs** have grown rapidly… **FTZs** offer clear advantages… Criminal networks use non-transparent **FTZs**… **FTZs in Spain and Costa Rica** are amongst the first to obtain certification."

The repetition is **a feature, not a bug**. It anchors the reader.

**(e) Demonstrative + summary noun**
"This pattern", "these findings", "this gap", "this trend" — all bridge sentences by re-pointing to the previous content with a single noun phrase.

> "Reimbursement rates vary considerably across Europe… **This variation** is largely accounted for by fiscal capacity and HTA practice…"

**(f) Numbers that lock together**
When citing comparators, sequence them so adjacent numbers belong to adjacent ideas. Do not jump back and forth.

- ✓ "36% in Ireland, against an EU27 average of 51% and a German benchmark of 91%."
- The progression Ireland → EU27 → Germany lets each comparator land cleanly.

#### Paragraph length and density

OECD paragraphs are **denser and longer** than typical academic prose. Aim for:
- 5–10 sentences per paragraph in main analytical text
- 100–250 words per paragraph
- One **dominant theme** per paragraph; secondary points subordinated within sentences, not split off as their own paragraphs
- A short pivot sentence (≤ 12 words) somewhere mid-paragraph for breathing room

**Resist the urge to split**. If you have two opposing views on the same topic, often the right move is to keep them in **one paragraph** with an embedded "by contrast" / "however", not break into two paragraphs labelled "First… Second…".

#### A worked cohesion comparison

**✗ Crunchy version (over-segmented, scaffold-heavy):**
> The threshold itself is contested.
>
> Two strands of debate surround this arrangement.
>
> The first concerns the threshold itself. An opportunity-cost argument holds that €45,000 is too permissive…
>
> The second concerns access. The access literature draws attention to Ireland's delayed availability of new oncology medicines…
>
> The most recent EFPIA W.A.I.T. data are striking. Only 36% of oncology products approved by the EMA between 2021 and 2024 have been reimbursed in Ireland…

**✓ OECD-style cohesive version:**
> Whether the threshold itself is calibrated correctly is contested. An opportunity-cost argument holds that the €45,000 figure is too permissive relative to the health forgone elsewhere in the system when it is exceeded, implying the systematic displacement of more cost-effective interventions (O'Mahony, 2021). The access literature, by contrast, focuses on Ireland's delayed availability of new oncology medicines compared with other EU countries, with comparatively little attention to their cost-effectiveness. EFPIA W.A.I.T. data illustrate the gap. Only 36% of oncology products approved by the European Medicines Agency between 2021 and 2024 have been reimbursed in Ireland, against an EU27 average of 51% and a German benchmark of 91%. Time to availability follows a similar pattern, with oncology medicines taking, on average, 730 days from EU marketing authorisation to reimbursement in Ireland — roughly two months longer than the EU27 average of 655 days, and around 2.5 times the German figure (Newton et al., 2026).

**What changed**:
- One paragraph instead of five fragments
- "by contrast" embedded inside the sentence rather than as a paragraph signpost
- "EFPIA W.A.I.T. data illustrate the gap." — a short pivot, not a value judgement ("are striking")
- Numbers chained Ireland → EU27 → Germany without interruption
- Lexical chain on "access" / "availability" / "reimbursement" maintains topic
- No "Two strands" or "The first / The second" meta-language

### 2.10 Sentence-extension techniques (句末延伸结构)

OECD sentences expand information **rightward** rather than through left-branching subordination. Three signature techniques that occur in nearly every OECD paragraph:

**(a) "with" + absolute clause** — the OECD workhorse for adding context

Pattern: `[main clause], with [noun phrase] + [-ing verb / past participle / adjective] + [details].`

> "Canada's economy has been resilient, **with growth picking up over 2024**."
> "Population ageing is expected to increase pension expenditures, **with the old-age dependency ratio reaching 50% by 2050**."
> "Inflation has eased, **with core inflation now close to target**."
> "The fiscal stance is set to be expansionary in 2025-26, **with the fiscal balance projected to reach 0.1% of GDP**."
> "Bank profitability has declined since 2023, **with funding costs and loan-loss provisions rising**."

This is one of the most distinctive lexical-syntactic fingerprints of OECD prose. **Use it once per paragraph at minimum** to avoid the choppy AI-default rhythm.

**(b) Trailing relative clause (which / that)**
Brief relative clauses adding identifying information:
> "the federal carbon pricing system, **which covers more than 80% of emissions**"
> "the Recovery and Resilience Plan, **which has accelerated public investment**"
> "non-transparent FTZs, **which serve as gateways for narcotic smuggling**"

Keep these short (≤ 15 words). Long, nested relatives are not OECD style.

**(c) "including / such as / for example" appositives**
> "Several sectors, **including manufacturing, construction, and tourism**, have faced labour shortages."
> "New concealment methods, **such as semi-submersibles and GPS-tracked drop-offs**, are increasingly observed."

### 2.11 Sentence-initial adverbials (句首副词的位置和逗号)

OECD writers **front-load** transition or emphasis adverbials, comma-separated. Six patterns:

**(a) Connective adverbs** (most common position is sentence-initial, comma after):
> "**Furthermore,** spending on active labour market policies has increased."
> "**Moreover,** there are rising long-term ageing expenditures."
> "**However,** this will require strong efforts to maintain primary surpluses."
> "**At the same time,** structural challenges weigh on future growth."
> "**By contrast,** access advocates highlight delayed availability."
> "**Nevertheless,** Argentina's foreign bribery enforcement remains limited and uneven."

**(b) Temporal markers**
> "**In 2024,** the Netherlands ranked seventh among DAC members."
> "**Over 2024,** the labour market softened."
> "**Since 2023,** bank profitability has declined."
> "**Looking ahead,** GDP is expected to grow by 1.1%."
> "**In recent years,** social expenditures have increased rapidly."

**(c) Spatial / sectoral markers**
> "**In the housing market,** prices have stabilised."
> "**Across OECD countries,** the share of renewables has risen."
> "**At the regional level,** disparities remain pronounced."
> "**In Portugal,** medium-term fiscal plans are not binding."

**(d) Conditional / hypothetical**
> "**Should risks materialise,** the central bank stands ready to act."
> "**If conditions allow,** the fuel charge should be reapplied."
> "**Provided that reforms continue,** debt is projected to stabilise."

**(e) Source / attribution**
> "**According to the IMF,** Argentina's growth is set to recover."
> "**Based on preliminary data,** ODA decreased by 2.8% in real terms."
> "**As reported by the Banco de Portugal,** export exposure is concentrated in three sectors."

**(f) "While / Although / Despite" concessive openers**
> "**While GDP growth has picked up,** productivity performance has continued to lag."
> "**Although** progress has been made on enforcement, many cases remain pending."
> "**Despite** the support of European funds, public investment remains below its 2005-10 levels."

**Position rule**: when an adverbial of more than one or two words opens a sentence, follow it with a comma. "However," takes a comma; never "However in 2024" — restructure as "In 2024, however,…" with two commas wrapping "however".

**Mid-sentence "however"** (very characteristic of OECD prose):
> "Bank profitability **has, however, declined** since 2023."
> "Implementation, **however,** has experienced systematic delays."
> "Risks, **however,** remain elevated."

This **"subject + auxiliary, however, predicate"** pattern is a signature OECD rhythm — use it whenever the contrast attaches to the verb rather than to the whole clause.

### 2.12 The recommendation register (建议语气分级)

OECD recommendations occupy a graded spectrum. Choose the right modal precisely.

**Acknowledgement of progress** (used before any recommendation):
- "This is welcome and should be continued."
- "These initiatives are welcome."
- "Recent reforms are a step in the right direction."
- "Significant progress has been made."

**Soft framing** (introducing a recommendation gently):
- "**There is scope to** strengthen oversight of public procurement."
- "**There is room to** improve integration of services."
- "**More can be done to** broaden the VAT base."
- "**Further reforms could be considered**."
- "**Reform could include** the streamlining of tax expenditures."

**Conditional recommendation** ("would" + outcome):
- "**Increasing the effective retirement age would help offset** rising pension costs."
- "**Streamlining benefits would reduce** marginal effective tax rates."
- "**Further consolidation would benefit** fiscal sustainability."

**Firm recommendation** ("should" + active verb, named subject):
- "Canada **should reapply** the fuel charge."
- "The preferential corporate tax rate **should be discontinued**."
- "Argentina **should adopt** a comprehensive whistleblower protection framework."
- "**X should be paired with** Y." (when one reform requires a complementary reform)

**Compound firm recommendation** (frequent in executive summaries):
> "Portugal **should ensure** the implementation of a medium-term strategy with gradual fiscal consolidation **combined with** policies to foster potential growth."
> "These reforms **should include** improving expenditure quality, reducing inefficient tax expenditures, **and** strengthening the use of spending reviews."

**Implicit recommendation** (gerund subject + "would help / is essential / is needed"):
- "**Strengthening labour market integration would help reduce** long-term unemployment."
- "**Continuing efforts to reduce corruption is essential** for restoring trust."
- "**Streamlining and reducing the large number of means-tested benefits is essential.**"
- "**Continued close monitoring of household debt is essential.**"

**Conditional firm** ("If / Should X, [country] should Y"):
- "**Should risks materialise,** the central bank should maintain restrictive policy for longer."
- "**If RRP spending were implemented more slowly than projected, this would constrain investment**."

**The escalation ladder** — pick the right rung:
1. Acknowledgement: "This is welcome."
2. Modest extension: "There is scope to…"
3. Soft recommendation: "Reform could include…"
4. Conditional outcome: "Doing X would help Y."
5. Firm recommendation: "X should be discontinued / reformed / phased out."
6. Conditional firm: "If risks materialise, X should…"

**Avoid in recommendations**:
- "Must" — too coercive; reserved for treaty obligations
- "Need to" — informal; replace with "should" or "is needed"
- Bare imperatives ("Reform the tax code") — non-OECD register
- "It is imperative that" — too dramatic
- "Urgent action is required" — alarmist; OECD prefers "warrants careful attention"

### 2.13 Citation and reference conventions (引用规约)

**Inline source citations** — parenthetical author-year, end of clause or sentence:
- `(OECD, 2024)`
- `(OECD, 2024[15])` — with reference number
- `(Banco de Portugal, 2025)`
- `(Smith et al., 2024)` — three or more authors
- `(Smith and Jones, 2024)` — two authors
- `(OECD, 2024; IMF, 2024)` — multiple sources, semicolon-separated

**Cross-references inside the document**:
- `(see Chapter 2)`
- `(see Section 1.3)`
- `(Box 1.2)` or `(see Box 1.2)`
- `(Figure 1.4)` or `(Figure 1.4, Panel A)`
- `(Table 1.2)`

**Figure / Table introduction in running text**:
> "House prices have risen sharply since 2020 (**Figure 1.4**)."
> "Reimbursement rates vary considerably across Europe (**Figure 2, Panel B**)."
> "**Table 1.2** summarises the main findings and recommendations."

**Self-reference** (when a Survey or Brief refers to itself):
- "as discussed in this Survey"
- "the measures proposed in this Survey"
- "this Brief"
- **Never use** "this paper", "this report shows", "we argue", "this analysis demonstrates"

**Source and Note lines** under figures/tables (standard template):
```
Source: OECD Economic Outlook: Statistics and Projections (database).
Note: Panel A: Shaded area indicates OECD projections. Panel B: The old-age dependency
ratio is the ratio of the population aged 65 years and over per 100 people of working age.
```

Source line patterns:
- `Source: OECD [Database name] (database).`
- `Source: Calculations based on data from [organisation].`
- `Source: OECD calculations based on [Source X].`

Note line patterns:
- `Note: [Panel A:] [explanation]. [Panel B:] [explanation].`
- `Note: The OECD aggregate refers to a simple average of [N] countries.`
- `Note: Data refer to [year]. [Country] data are not available.`

### 2.14 Additional cross-genre sentence patterns (v9)

**T46. The "despite [positive data], [negative reality]" empirical-contrast sentence** — OECD presents seemingly favourable data, then immediately qualifies it with a structural problem the data obscures. Verified in Philanthropy Study, PMR Evidence, Capacity Assessment.

> "Despite significant progress over the past decade, Mexico **continues to face** high income inequality, poverty, and informality."
> "Despite these shifts, philanthropic support **remained concentrated in** the same three sectors throughout the period."
> "Despite their clear relevance, one-third of the countries surveyed **have only one** of the two sets of integrity standards."

Pattern: "Despite [positive framing], [subject] [continues to / still / remains] [negative state]." — The "despite" sets up a concessive frame; the main clause delivers the sobering reality. AI defaults to either full positivity or full negativity; OECD always pairs them. **Use once per country-profile opening or data-analysis section.**

**T47. The "while X [positive verb], Y [remains/challenges]" comparative-clause sentence** — OECD uses a "while" clause to set up a comparison between two countries, sectors, or groups, then delivers the key finding in the main clause. Verified in PMR Evidence, RBC Guidance, Philanthropy Study.

> "While only OECD countries are considered, the results are very similar."
> "While the overall correlation between the two variables is positive but low (0.33), there are some notable outliers."
> "While exports of oil and mining products have increased, the manufacturing sector remains small."

Pattern: "While [context/scope/positive finding], [main clause with key finding or qualifier]." — This is distinct from "although" (§4-L). "While" sets up a **parallel comparison** between two entities or scopes; "although" introduces a **concession**. AI overuses "although"; OECD deploys "while" for side-by-side comparison. **Deploy 1-2 times per comparative section.**

**T48. The "this suggests that" / "this underscores the importance of" data-to-implication bridge** — OECD connects a data finding to its policy implication using a small set of analytical-bridging verbs. The bridge verb choice signals the strength of the inference. Verified across all 7 v9 genres.

Weak bridge (observation only):
> "The data **shows a complex interaction** between poverty levels and allocation of philanthropic resources."
> "This distribution **underscores the widespread prioritisation** of health across much of the country."

Medium bridge (suggestive):
> "This pattern **suggests that** philanthropic resources struggle to reach areas with the highest poverty rates."
> "These distortions **can, in turn, hinder** the natural forces of competition and market selection."

Strong bridge (direct implication):
> "These findings **underscore the importance of** better regulatory policies to manage the stock of existing regulations."
> "These deficiencies in the regulatory framework **matter now more than ever**, as governments make greater use of industrial policies."

Bridge verb hierarchy (weak → strong): *shows → reflects → suggests → highlights → underscores → underscores the importance of*. AI defaults to the middle; OECD calibrates precisely. **Match the bridge verb to the strength of the evidence.**

**T49. The "recommendation-number" intervention sentence** — OECD capacity-assessment and governance-review genres use numbered, bolded recommendations as structural anchors. Each recommendation is a standalone imperative sentence, followed by an explanatory paragraph. Verified in Capacity Assessment, Digital Governance Guidance.

> "**Recommendation 4.** If, reflecting cost or related considerations, a combined R&D and innovation survey remains the preferred method, an appropriate hybrid sampling and estimation design should be promptly developed."
> "**Recommendation 8.** An easily understood Business R&D and Innovation Survey Methodology Report should be readily available to researchers and survey practitioners."

Pattern: "**Recommendation [N].** [Subject] should [action verb] [object], [conditional clause / purpose clause]." — Recommendations use "should" (not "must", not "could"), and typically include a purpose clause or qualifying condition. The number provides navigational structure. **This pattern is genre-specific to Capacity Assessments, Governance Reviews, and Operational Guidance. Do not deploy in Economic Surveys or Policy Briefs.**

**T50. The "table-notes-source" footnote triad** — OECD data tables carry a precise three-layer footnote system: numbered methodology notes, then a "Source:" line, then occasionally additional context notes. This triad is a genre-specific formatting fingerprint. Verified in PMR Evidence, Philanthropy Study, Working Paper.

```
Notes:
1. Percentages are calculated over the 47 countries surveyed.
2. In federal countries where regulation is set at the state level, the PMR database
   reports information for only one representative state.
3. For the identity of the countries that fall into each category please refer to
   Table A.1 in the Appendix.
Source: 2023-2024 PMR database.
```

Key patterns:
- Notes are **numbered**, not bulleted
- Note 1 always specifies the **denominator** ("calculated over [N] countries surveyed")
- Subsequent notes add **scope restrictions** ("In federal countries…", "Türkiye is not included because…")
- The Source line uses the **database name + year**, not a URL
- AI defaults to generic "Source: OECD data"; OECD uses **specific database names and edition years**

### 2.15 Sentence patterns from v10 deep sampling

**T51. The "it may then come at little surprise to observe" understated-causal-link sentence** — OECD presents a finding as the logical, almost inevitable consequence of the evidence it has just laid out. The author does not assert the link as fact; instead, the reader is guided to draw the conclusion themselves. Verified in Labour Shortages, Trust Study.

> "It may then come at little surprise to observe increased labour shortages in this sector, especially as the pandemic acted as an eye opener about the pressures endured by the profession."
> "Given the similar importance of Russia in the production of both metals, one might have expected a comparable response in terms of price volatility."

Pattern: "It may then come at little surprise to observe [finding], especially given [evidence already presented]." — This is OECD's version of the rhetorical "of course" — but never using those words. The finding arrives as if it were self-evident from the preceding paragraphs. AI never produces this; it either asserts causation directly or hedges with "this suggests." **Deploy once per analytical section where the evidence strongly supports the conclusion.**

**T52. The "the relative mix of which will need to be tailored" universal-policy-disclaimer sentence** — OECD ends a policy section by explicitly stating that the recommended actions must be adapted to local conditions. This is not a hedge — it is an institutional commitment to context-sensitivity. Verified in Labour Shortages, Circular Economy, Trust Study.

> "As is the case in all policy domains, country-specific challenges and policy requirements will depend on the economic and social context, along with social preferences and political economy considerations."
> "While priorities will vary depending on country-specific context, this section draws some policy implications for efficiency and inclusiveness."
> "The relative mix of which will need to be tailored to country-specific circumstances."

Pattern: "While [recommended actions are general], the relative mix / priorities will need to be tailored to [country-specific / local] circumstances." — AI either gives universal prescriptions without qualification, or hedges everything into meaninglessness. OECD gives **clear recommendations** followed by an explicit statement that implementation must be context-adapted. **Deploy at the end of every policy-recommendation section.**

**T53. The "in contrast to [established model/sector]" explicit-reference-frame sentence** — OECD grounds its analysis by explicitly comparing it to a well-known reference framework (usually oil markets, existing OECD models, or established literature). This anchors the reader's understanding. Verified in Commodity Market WP, Labour Shortages.

> "In contrast to oil market models, the remaining variables in the system do not exhibit a response to expectational demand shocks."
> "In contrast to aluminium markets, nickel prices are more susceptible to revisions in market expectations."
> "Unlike oil markets, which are shaped by coordinated efforts such as those by OPEC, interventions in metal markets tend to be unilateral and uncoordinated."

Pattern: "In contrast to [well-known reference], [current finding differs in specific way]." / "Unlike [reference], [subject] [behaves differently]." — This is distinct from simple "by contrast" comparison (T47). T53 specifically references an **established model, sector, or literature** to help the reader situate the new finding. AI defaults to standalone assertions; OECD **always situates findings in context**. **Deploy 1-2 times per results section when the finding deviates from or aligns with established expectations.**

**T54. The "at present... however, as [X] progresses" current-state-qualifier sentence** — OECD describes the current state of affairs as limited or bounded, then immediately flags that this could change as a dynamic process unfolds. This is a forward-looking qualification, distinct from the "forward-looking monitoring commitment" fingerprint (O). Verified in Commodity Market WP, Circular Economy, Labour Shortages.

> "At present, the use of derivatives in metal markets remains largely limited to financial markets and the mining sector. However, as the energy transition progresses, the need to hedge against metal price volatility is likely to expand."
> "While these metals do not currently exhibit impacts beyond prices, this may change as critical minerals become crucial for energy generation."
> "Data on satisfaction with services among Indigenous Australians is scarce, presenting challenges in assessing their experiences."

Pattern: "At present / Currently, [X] remains [limited/bounded]. However, as [dynamic process] progresses, [X] is likely to [expand/change]." — AI describes the current state and stops. OECD describes the current state **and** immediately flags the trajectory. **Deploy when the current state is not representative of future conditions.**

**T55. The "cost often remains the predominant consideration... highlighting a gap between policy aspirations and practical implementation" gap-framing sentence** — OECD identifies the disconnect between what policy documents say and what actually happens on the ground. This is the institutional equivalent of "easier said than done." Verified in Circular Economy, Trust Study, Labour Shortages.

> "However, cost often remains the predominant consideration in procurement decisions, highlighting a gap between policy aspirations and practical implementation."
> "However, evidence suggests many are unaware they can provide feedback, and those who do are not always satisfied with the outcome."
> "This does not seem to have taken place on a broad scale, and many countries have been struggling with persistent staff shortages."

Pattern: "However, [practical constraint] remains the predominant consideration, highlighting a gap between [policy aspiration] and [practical implementation]." — AI either describes only the policy or only the problem. OECD **names the gap** between the two. **Deploy once per policy-implementation section.**

### 2.16 Sentence patterns from v11 deep sampling

**T56. The "[metric] has jumped from [X%] to [Y%]" temporal-data-shift sentence** — OECD presents a metric's change over time by explicitly stating both the starting and ending values, with the time period and source named. This is distinct from simple quantified change (T2) because it specifically frames a **normative shift** (priority, policy attention, prevalence), not just an economic variable. Verified in Gender Equality, Trust Study.

> "This issue has jumped from a top-three priority for 68% of the 31 OECD countries responding to the OECD questionnaire in 2016 to a top-three priority for 86% of the 43 OECD and EU countries responding in 2024."
> "The share of performance variance explained by socio-economic status rose from 11.8% in 2012 to 15.0% in 2022, reaching the OECD average."

Pattern: "[Subject] has jumped / risen / shifted from [X%] of [population] in [year] to [Y%] of [population] in [year]." — AI tends to report only the current figure or use vague "increased significantly." OECD **names both endpoints and both sample sizes**. Verified in Gender Equality, Education Sweden. **Deploy when presenting survey-based attitudinal or policy-priority shifts.**

**T57. The "these developments have impacted [structure], with [consequence]" consequence-chain sentence** — OECD traces how multiple upstream factors converge to reshape a structural outcome. The "with" clause delivers the most policy-relevant consequence. Verified in Financing SMEs, Revenue Statistics.

> "These developments across the range of financing instruments have impacted the structure and uses of financing for SMEs, with higher shares of smaller scale, short-term financing for immediate needs."
> "In most cases, nominal tax revenue and nominal GDP increased over the period except in Chile and Peru, which recorded falls in nominal tax revenue."

Pattern: "These / Such developments have impacted [structural variable], with [observable consequence for policy]." — AI tends to stop at "X declined." OECD traces the **downstream structural impact**. Verified in Financing SMEs. **Deploy at the end of an analytical section to bridge to policy implications.**

**T58. The "while [positive trend] has begun to moderate, [negative factor] continues to linger" mixed-signal sentence** — OECD presents a complex macro environment where some indicators improve while others remain problematic. This is the macro-economic version of the "affirmative + but" pattern (T1), but at the **systemic level** with multiple interacting variables. Verified in Financing SMEs, Revenue Statistics.

> "While inflation has begun to moderate, inflationary pressures continue to linger in many economies."
> "While companies indicated a further tightening of financing conditions in early 2024, they also indicated more availability of bank loans compared to 2023."

Pattern: "While [positive indicator] has begun to [improve verb], [negative indicator] continues to [persistence verb] in [scope]." — AI defaults to either fully optimistic or fully pessimistic macro framing. OECD **holds both signals simultaneously**. Verified in Financing SMEs. **Deploy in macro-economic context-setting paragraphs.**

**T59. The "although this pattern is somewhat more positive than [benchmark], the recent downturn signals renewed challenges" benchmarked-assessment sentence** — OECD evaluates a country's trajectory against a reference group, acknowledges relative advantage, but immediately flags the emerging risk. Verified in Education Sweden, Revenue Statistics.

> "Although this pattern is somewhat more positive than the average OECD trend during the same period, the recent downturn signals renewed challenges in sustaining earlier gains."
> "Sweden's modest decrease appears relatively stable by comparison."

Pattern: "Although [country] [performed] somewhat more [positively] than [benchmark group], the recent [negative shift] signals renewed challenges in [sustaining / achieving] [goal]." — AI tends to either celebrate relative performance or lament absolute decline. OECD **does both in one sentence**. Verified in Education Sweden. **Deploy when comparing country trajectories to OECD or regional averages.**

**T60. The "the numerator (X) ... the denominator (Y)" methodological-transparency sentence** — OECD explicitly defines the components of a ratio or composite indicator before presenting the data. This is not a footnote — it is in the main text, prominently placed. Verified in Revenue Statistics, Financing SMEs.

> "The numerator (tax revenues) uses tax revenue figures that are submitted by focal points or published annually by national Ministries of Finance..."
> "The denominator (GDP) figures used in this publication are sourced from countries' national accounts as well as the World Economic Outlook (WEO) published by the IMF."

Pattern: "The numerator ([label]) [definition and source]. The denominator ([label]) [definition and source]." — AI rarely defines ratio components in the main text. OECD **always does this for key indicators** because the audience includes non-technical policymakers. Verified in Revenue Statistics. **Deploy once per data section when introducing a key ratio or composite indicator.**

**T61. The "several factors contribute to / may explain" multi-cause enumeration sentence** — OECD lists multiple contributing factors to a single outcome, using "including" or "such as" to provide specifics for each factor. This is the data-report genre's equivalent of the multi-causal explanation (§4-U), but more compact and formulaic. Verified in Revenue Statistics, Financing SMEs.

> "Several factors contribute to the low VRR in Mexico, including the scope of VAT exemptions, the application of a domestic zero rate to numerous goods and services, as well as low compliance."
> "This increase can be attributed to several factors: high inflation seen for most of the year, compounded by the rapid increase in the cost of debt finance and the tight supply of credit."

Pattern: "Several / multiple factors contribute to / explain [outcome], including [factor 1], [factor 2], as well as [factor 3]." — AI tends to give a single cause or use vague "various factors." OECD **names each factor concretely**. Verified in Revenue Statistics, Financing SMEs. **Deploy when explaining why a metric moved in an unexpected direction.**

**T62. The "the fiscal year in [country] runs from [month] to [month]" data-caveat sentence** — OECD explicitly flags differences in reporting periods that could affect cross-country comparability. This is a genre-specific transparency fingerprint of data-heavy reports. Verified in Revenue Statistics.

> "The fiscal year in Barbados, Belize and Saint Lucia runs from April to March. This means that reporting year 2023 is Q2/2023-Q1/2024."
> "The fiscal year for The Bahamas ends on 30 June. The reporting year 2023 runs from Q2/2022-Q2/2023."

Pattern: "The fiscal year in [country(s)] runs from [month] to [month]. This means that reporting year [YYYY] is [quarter range]." — This is a **data-report genre exclusive** (Revenue Statistics, National Accounts). AI never includes this. OECD always includes it because comparability depends on period alignment. **Deploy only in cross-country fiscal data reports.**

**T63. The "[N]% of the [M] countries surveyed still do not [requirement]" data-driven regulatory-gap sentence** — OECD presents the gap between best practice and current adoption using the PMR/survey prevalence formula. The word "still" signals institutional surprise or urgency. Verified in Lobbying Regulation, PMR Evidence.

> "A staggering 36% of the countries surveyed still do not impose the latter requirement on neither appointed public officials nor non-elected senior civil servants."
> "Half of the 47 countries surveyed do not impose the main disclosure obligations that could apply to public officials."
> "Only 30% of the 47 countries surveyed have such a regulatory framework."

Pattern: "[Quantifier: A staggering / Only / Half of] [N]% of the [M] countries surveyed [still] do not [specific requirement]." — AI tends to report adoption rates positively ("70% have X"). OECD **frames the same data as a gap** — "36% still do not have X." The "still" is a human editorial judgment that signals institutional frustration. Verified in Lobbying Regulation, PMR Evidence, Revenue Statistics. **Deploy in regulatory-assessment and compliance-gap genres.**

**T64. The "only [N] countries – [Country1] and [Country2] – [impose/achieve] [requirement]" positive-extreme spotlight sentence** — OECD names the few countries that meet the highest standard, implicitly setting them as benchmarks. This is the mirror image of T63 — instead of naming the gap, it names the leaders. Verified in Lobbying Regulation, PMR Evidence.

> "Only two countries – Chile and Poland – impose all 4 of them, and 11 countries have none of them."
> "Further, only three countries – Chile, Poland, and Sweden – impose all 3 obligations."

Pattern: "Only [N] countries – [Country1] and [Country2] – [impose/achieve] all [N] [requirements], and [M] countries have none of them." — AI tends to report averages or percentages. OECD **names the outliers at both extremes** — the leaders and the laggards. This dual-extreme framing is a signature of PMR and compliance-assessment genres. **Deploy in cross-country regulatory comparison sections.**

**T65. The "these deficiencies matter now more than ever, as [actor] [expands activity]" urgency-elevation sentence** — OECD connects a known regulatory gap to a newly intensifying policy trend, creating urgency. This is not alarmist — it is a measured escalation from "this has always been a problem" to "this is becoming critical." Verified in Lobbying Regulation, Disaster Risk.

> "These deficiencies in the regulatory framework matter now more than ever, as governments make greater use of industrial policies to support strategic sectors and promote innovation."
> "Coping with disaster risk will require a holistic policy approach. It should include elements across multiple policy areas."

Pattern: "These deficiencies / gaps / challenges matter now more than ever, as [actor] [expands / intensifies / accelerates] [activity]." — AI tends to either understate urgency or overstate it. OECD **calibrates urgency to the policy moment** — "now more than ever" is the maximum urgency register. Verified in Lobbying Regulation. **Deploy in introductions and conclusions of regulatory-gap papers.**

**T66. The "what if… [desirable future scenario]?" transformative-vision sentence** — OECD uses "What if..." as a rhetorical device to open scenario-planning exercises. This is distinct from question-form section headings (§9.3 Policy Brief) — here the question IS the content, framing an entire scenario chapter. Verified in Scenario Planning, Education Futures.

> "What if you had the opportunity to shape young minds and make a lasting impact on society?"
> "What if… Schools provide space to foster curiosity and autonomy among students, teachers, and school leaders?"
> "What if… We enable a culture of innovation for and with the teaching profession?"

Pattern: "What if… [actor] [enables / creates / fosters] [desirable outcome]?" — This is the **scenario-planning genre's signature opening**. AI never uses this. OECD uses it to frame entire chapters and stakeholder workshops. Verified in Scenario Planning. **Deploy only in scenario-planning and futures-oriented genres.**

**T67. The "Meet [Name], [role descriptor]" persona-introduction sentence** — OECD introduces fictional but data-driven personas with a conversational "Meet..." followed by a brief descriptor of their career stage and context. This is a genre-exclusive device. Verified in Scenario Planning.

> "Meet Sophia and Maximilian, starting primary school teachers/students."
> "Meet Fatma and Ernst, experienced secondary school leaders."
> "Meet Jelena and Lukas, Austrian teachers from the future."

Pattern: "Meet [Name] and [Name], [career stage] [role] [setting]." — This is the **persona-based scenario genre's signature device**. AI defaults to abstract role descriptions. OECD **gives the role a human name and a career stage**. Verified in Scenario Planning. **Deploy only in persona-based policy analysis genres.**

**T68. The "the decrease in demand may be surprising at first glance, given [headline trend]" counterintuitive-findings sentence** — OECD introduces a finding that contradicts the prevailing narrative, then resolves the paradox with evidence. This is the empirical paper's version of the "affirmative + but" pattern (T1), but at the **macro-trend level**. Verified in AI Skills, Financing SMEs.

> "The decrease in the demand for new AI talent in Canada may be surprising at first glance, given the headlines applications of AI systems such as ChatGPT."
> "It is important to note that this is not to say that there is less AI talent operating in Canada, since the nature of the data – job postings – do not reflect the current stock."

Pattern: "The [decline / shift / change] in [metric] may be surprising at first glance, given [headline trend / prevailing narrative]. However, [explanation involving data limitations or structural factors]." — AI tends to either ignore counterintuitive findings or overexplain them. OECD **names the surprise, then resolves it with data literacy**. Verified in AI Skills. **Deploy in empirical analysis sections where data contradicts headlines.**

---

## 3. Structure (结构)

### Document-level architecture

```
Metadata block (publication year, date, source URL, PDF URL)
├── Table of Contents
├── Executive Summary / Key Messages
│   └── 3-5 bullet points with main findings + recommendations
├── Main body chapters (numbered: 1, 2, 3...)
│   ├── Section headings (### level)
│   ├── Data tables where relevant
│   ├── Sub-sections with specific findings
│   └── Notes and source citations
├── Policy recommendations (sometimes integrated per chapter)
└── References / Annexes
```

### Paragraph-level structure
Each paragraph follows one of these patterns:

1. **Topic sentence → evidence → implication**
   > The labour market has softened with job vacancies coming down and the unemployment rate increasing over 2024. Wage growth is also moderating but remains high compared to productivity growth. Headline inflation is expected to decrease...

2. **Claim → data point → comparison**
   > In 2023, civil society organisations (CSOs) received USD 1.1 billion of gross bilateral ODA, of which 8.5% was directed to developing country-based CSOs. Overall, 2.3% of gross bilateral ODA was allocated to CSOs as core contributions...

3. **Problem → cause → recommendation (3-part)**
   > [What is the challenge] → [What drives it] → [What should be done]

### Data integration rules
- Embed numbers inline, not in parentheses-only sentences
- Format: `[amount] ([percentage] of [benchmark])` — e.g. "USD 1.3 billion (25.4% of gross bilateral ODA)"
- Always give the unit: USD, EUR, percentage points, tonnes CO₂
- When comparing: state the subject, then the comparator, then the gap — "The region's GDP per capita is 42% below the national average"
- After a data point, optionally add a time-trend: "This was an increase of 24.2% in real terms over 2022"

### Table format
Use markdown tables for multi-year comparisons. Always include:
- Column headers with year or category
- Row labels with clear metric names
- A "Note:" row below the table explaining abbreviations and data caveats
- A "Source:" attribution

---

## 4. Logic (逻辑)

### Argumentation patterns

**A. Situation → Complication → Resolution (SCR)**
> [Country] faces [challenge]. This is driven by [causal factors]. To address this, [recommendations].

**B. Concession → Counter-argument**
> While [positive development], [limitation persists]. [Therefore/accordingly], [policy implication].

**C. Evidence ladder: specific → general**
> [Specific data point for country] → [Comparison with OECD average] → [Broader structural implication]

**D. Risk framing**
> However, risks, particularly those related to [specific area], remain significant and warrant careful oversight and [action].

**E. Upside / Downside risk enumeration** (Economic Outlook genre)
OECD presents risks symmetrically: first the downside, then the upside (or vice versa). Each risk is a single bullet or sentence, introduced by a conditional clause or participial phrase.

> "A significant downside risk to the outlook is that persistent disruptions to exports from the Middle East that raise energy prices even further than assumed and aggravate shortages of key commodities, add to inflation and reduce growth."
> "On the upside, a surprisingly resilient business sector, an earlier-than-assumed resolution of the conflict, or broadening investment in artificial intelligence technologies, could push growth higher."

Note: "On the upside" appears 6 times in a single Economic Outlook. This is the OECD author's standard risk-framing device for macroeconomic reports.

**F. Appeal to precedent** (cross-genre)
OECD grounds claims in past experience rather than abstract reasoning.

> "Past experience has shown that commodity price shocks can push up inflation expectations, particularly when the shocks are driven by energy and food prices."
> "The experience of countries that have implemented similar reforms suggests that…"

Pattern: "Past experience has shown that…" / "The experience of [X] suggests that…" — use this instead of "History tells us" or "It is well known that".

**G. Equivalence comparison** (Economic Outlook / Industry Outlook)
OECD makes abstract numbers concrete by converting them to physical or temporal equivalents.

> "This is equivalent to the volume of oil and oil products that would typically pass through the Strait of Hormuz in 20 days."
> "This represents the equivalent of [country]'s entire annual output."

Pattern: "This is equivalent to…" / "This represents the equivalent of…" — use when a number needs grounding in something the reader can visualise.

**H. Risk-scoping: "The most immediate risks are for…"**
OECD scopes risk by specifying which actors face it first or most.

> "The most immediate risks are for many countries in Asia that are particularly reliant on energy imports from the region."
> "The most exposed sectors are those with high energy intensity."

Pattern: "The most immediate risks are for [actor]" / "The most exposed [sectors/countries] are those with [characteristic]" — never say "everyone is at risk"; OECD always specifies who bears the most risk.

**I. Conditional-consequence chain: "If [state], [consequence]"**
OECD embeds conditional hedges inside the main sentence rather than fronting them.

> "If sustained, these price shocks will add markedly to business costs."
> "If it persists, this dynamic could weigh on the recovery."
> "If realised, these investments would transform the sector."

Pattern: "If sustained/held/realised/persisted, [main clause]" — the conditional comes first, the consequence follows. This is more compact than "In the event that…"

**J. Scope-widening: "More broadly"**
OECD uses "More broadly" to zoom out from a specific point to a wider context.

> "More broadly, countries around the Persian Gulf are a logistical hub for many services."
> "More broadly, the regulatory environment needs to adapt."

Pattern: "More broadly, [wider context]" — use after a specific point to show it connects to a larger issue. This replaces AI's "Furthermore" or "Moreover" when the function is to widen scope rather than add a parallel point.

**K. "Given [X], [Y]" — the OECD causal anchor**
OECD uses "Given" as a prepositional phrase to establish a premise before drawing a conclusion.

> "Given the scale of the challenge, stronger policy action is needed."
> "Given that energy markets are global, the effects will be widespread."
> "Given these developments, the outlook remains uncertain."

This is the OECD author's preferred way to say "because X is true, Y follows". AI defaults to "Due to" or "Because of"; OECD reaches for "Given". Verified: "Given" appears 0-39 times across ALL genres.

**L. "although" — the universal concessive connector**
The single most universal concessive word in OECD prose. Verified: appears 1-32 times across ALL genres.

> "Although progress has been made, significant gaps remain."
> "Although the reforms are welcome, implementation remains uneven."

Use "although" for concessive clauses. Use "While" (T18) when the concessive and main clause are in the same sentence. Use "Despite" (T34) when the concession is a noun phrase.

**M. "even if" — the OECD hypothetical hedge**
OECD uses "even if" to concede a point without accepting its relevance.

> "Even if the reforms are implemented, the effects may take years to materialise."
> "Even if demand recovers, excess capacity will persist."

Verified: appears 0-21 times across genres. This is the OECD way of saying "even granting that X, Y still holds".

**N. "whereas" — the OECD analytical comparison**
OECD uses "whereas" to draw direct contrasts between two countries, sectors, or situations.

> "In some countries, such as France and Germany, institutions have a large degree of autonomy, whereas in others, such as the United States and the United Kingdom, the centre of government plays a stronger role."

"Whereas" is more analytical than "while" — it signals a structured comparison, not just a concession. Verified: appears 0-6 times, concentrated in analytical genres (Economic Surveys, Country Reviews).

**O. "This [analytical verb]…" — the OECD inference-sentence opener**
OECD uses "This + [verb]" to draw conclusions from the preceding evidence. This is the OECD author's standard way of connecting data to inference without meta-discourse.

- "This **suggests** that…" (most common — 18+11+3 times across genres)
- "This **reflects** the fact that…" (second most common — 11+10+3+2 times)
- "This **underscores** the need for…" (8+4+1 times)
- "This **highlights** [noun]" (2 times)
- "This **has led to** [consequence]" (2 times)
- "This **points to** [conclusion]" (less frequent)
- "This **warrants** [action]" (less frequent)

Pattern: "This + [analytical verb] + [conclusion]" — use this instead of "It is important to note that" or "This serves to highlight". The "This" refers to the evidence just presented. The verb carries the analytical weight. No meta-framing needed.

Verified across Gender Equality (30+ instances), SME Financing (28+), Supply Chain (16+), Economic Outlook (2+), Steel Outlook (1+). This is truly universal.

**P. Quantifier patterns — how OECD introduces numbers**
OECD has a specific vocabulary for introducing numerical data. These are the standard quantifier phrases, ranked by frequency:

- **"More than [X]"** — the most common quantifier across all genres: "More than 70% of tax administrations", "More than 80% of administrations"
- **"Nearly [X]"** — second most common: "Nearly 40% of tax administrations"
- **"Around [X]"** — the OECD default approximate: "Around 80% of administrations" (see T29)
- **"Close to [X]"** — similar to "around": "Close to 40% of tax administrations" (see T29)
- **"Over [X]"** — informal alternative to "more than": "Over 470 million people"
- **"Just over [X]"** — slightly more than: "Just over a quarter of administrations"
- **"Slightly more than [X]"** — precise approximation: "Slightly more than a quarter"
- **"Some [X]"** — formal approximation: "Some 90 million tonnes" (Steel Outlook)
- **"A total of [X]"** — for aggregate counts: "A total of 48 countries"
- **"Up to [X]"** — for maximum estimates: "Up to 250 million people"

**Anti-AI note**: AI defaults to "approximately" or "about". OECD uses "around", "close to", "nearly", "just over", "some". Avoid "approximately" — it's not OECD style.

### Logical connectives (use these, not colloquial ones)
| Function | OECD-preferred connectives | Cross-genre verified |
|----------|---------------------------|---------------------|
| Addition | "Furthermore", "Moreover", "In addition", "Additionally", "More broadly" (scope-widening) | All genres |
| Contrast | "However", "Nevertheless", "Nonetheless", "At the same time", "While", "In contrast", "On the other hand" (different perspective), "By contrast" | All genres |
| Cause | "This is due to", "This reflects", "driven by", "as a result of", "Given [X]" | All genres |
| Result | "Consequently", "As a result", "This has led to", "Taken together" (synthesising) | All genres |
| Concession | "Despite" (noun phrase), "Although" (clause), "While" (clause), "Notwithstanding" (formal/Latinate), "even if" (hypothetical) | All genres |
| Condition | "Provided that", "Should [X] materialise", "as long as", "even if" | Genre-dependent |
| Purpose | "In order to", "with a view to", "aiming to", "To support [actor] in [gerund]" | All genres |
| Emphasis | "Indeed", "In fact" | All genres |
| Comparison | "whereas", "Similarly", "In contrast" | Analytical genres |
| Scope-widening | "More broadly" | Economic Outlook / Surveys |
| Temporal | "Since" (causal-temporal), "through [year]" (time horizon) | All genres |

**Q. Lesson-drawing pattern — "The experience of [X] is illustrative"**
When OECD wants to draw a broader lesson from a specific case:
> "The experience of the solar manufacturing sector **is illustrative of what can happen when** market-distorting producer subsidies overshoot and global markets reach high levels of concentration."

Pattern: "The experience of [X] is illustrative of what can happen when [Y]." — the OECD way of saying "this case teaches us something general". Verified in Trade Brief (Subsidies Solar). This pattern elevates a specific case into a generalizable insight without AI-default phrasing like "This serves as a cautionary tale" or "This highlights the importance of".

**R. Balanced assessment of policy instruments — "useful but can have negative consequences"**
When OECD evaluates a policy tool that has both benefits and risks:
> "While subsidies **can be useful policy instruments for addressing certain market failures**, they **can also have negative consequences when they exceed what is necessary** for ensuring well-functioning markets."

Pattern: "While [X] can be useful [instruments/tools] for [purpose], they can also have negative consequences when they exceed what is necessary for [goal]." — the OECD way of saying "good in moderation, harmful in excess". Verified in Trade Brief. This is more sophisticated than AI's "While X has benefits, it also has drawbacks" — OECD specifies the threshold ("when they exceed what is necessary").

**S. Knowledge gap + call for research — "Our understanding is incomplete"**
When OECD acknowledges uncertainty and points to future research:
> "Our understanding of the relationship between the changing climate and marine ecosystems **is incomplete**. New research **is needed to refine our understanding** of how changes in ocean conditions may affect specific fish stocks and fisheries."

Pattern: "Our understanding of [X] is incomplete. New research is needed to refine our understanding of [Y]." — the OECD way of saying "we don't know enough yet". Verified in Environmental Brief (Fisheries), Investment Brief (VC). This is more honest than AI's "Further research is needed" — OECD specifies *what* is unknown and *what* research would help.

**T. Cooperation imperative — "no single country can tackle alone"**
When OECD argues for international cooperation:
> "Given the global nature of [X], **no single country can tackle these challenges alone**."

Pattern: "Given the [global/national/complex] nature of [X], no single [entity] can tackle these challenges alone." — the OECD way of arguing for collective action. Verified in Security Brief (Drug Traffickers), Environmental Brief (Fisheries), Trade Brief (Subsidies). This is more direct than AI's "International cooperation is essential" — OECD starts from the premise that one actor *cannot* do it alone.

**U. Multi-causal explanation — "cannot be attributed to X alone"**
When OECD explains that a phenomenon has multiple causes:
> "This decline in pricing **cannot be attributed to** innovation and economies of scale **alone; rather, it appears to reflect also** subsidy-fuelled over-capacity as reflected in supply-demand imbalances."

Pattern: "[X] cannot be attributed to [Y] alone; rather, it appears to reflect also [Z]." — the OECD way of saying "it's more complicated than one cause". Verified in Trade Brief (Subsidies). This is more precise than AI's "There are multiple factors" — OECD explicitly names the insufficient explanation first, then adds the overlooked causes.

**V. Perspective-shift explanation — "From a [X] perspective"**
When OECD explains a phenomenon from a specific analytical angle:
> "From a production perspective, the shift toward synthetic drug production **is facilitated by** its low cost, its scalability, and lower barriers to entry compared to plant-based production."

Pattern: "From a [X] perspective, the shift toward [Y] is facilitated by [Z], [W], and [V] compared to [U]." — the OECD way of framing an explanation through a specific lens. Verified in Security Brief (Drug Traffickers).

**W. Actor adaptation description — "[X] exploit advancements in [Y]"**
When OECD describes how actors adapt to new conditions:
> "Drug traffickers and producers **exploit advancements in** technology and globalisation **to adapt** production and trafficking patterns."

Pattern: "[X] exploit advancements in [Y] and [Z] to adapt [W]." — the OECD way of describing strategic adaptation. Verified in Security Brief. This is more precise than AI's "X leverages new technologies" — OECD uses "exploit" (negative connotation for illicit actors) and "advancements" (neutral for the technology itself).

**X. Hypothesis enumeration with hedged causation** — OECD presents multiple possible reasons for a finding without asserting which is correct.

> "There are several possible reasons which may explain the general trend of increasing resources for competition authorities. The possible reasons include:
> i. In 2023, 33% of authorities completed a comprehensive review of their digital strategy, up from 16% in 2019.
> ii. In 2023, 54% of authorities completed a comprehensive review of their organisational strategy, up from 30% in 2019."

Pattern: "There are several possible reasons which may explain X. The possible reasons include: (i) Y, (ii) Z." — OECD **enumerates hypotheses** rather than asserting a single cause. This is distinct from a simple list — it is explicitly framed as **possible** explanations. Verified in Competition Trends, Algorithmic Management. AI defaults to "This is because" or "The main reason is"; OECD enumerates alternatives without privileging one.

**Y. Double-conditional research gap** — OECD acknowledges that further research is needed to confirm not just the finding but the causal mechanism.

> "Further research would be needed to ascertain whether these are the most relevant drivers of resources and if so, whether the increase in resources will lead to greater future enforcement activity."

Pattern: "Further research would be needed to ascertain whether [X] and if so, whether [Y]." — this is a **double conditional**: first confirming the finding, then confirming the causal implication. OECD uses this when the data shows a trend but the mechanism is unclear. Verified in Competition Trends, Algorithmic Management. AI defaults to "More research is needed" without the double conditional.

**Z. Scope limitation with negative clarification** — OECD explicitly states what the analysis does NOT cover and what conclusions therefore cannot be drawn.

> "This chapter does not look at sufficiency of resources. This means that none of the possible conclusions that can be drawn from it imply that competition authorities have sufficient resources."
> "The analysis remains at the metric level. More specifically, this analysis does not consider ESG rating products' scoring methodologies."

Pattern: "This [chapter/section/analysis] does not [cover/look at/consider] [X]. This means that [negative implication]." — OECD uses this to **pre-empt over-interpretation**. It is the analytical equivalent of "don't read more into this than is there". Verified in Competition Trends, ESG Ratings, Tax Investigation Manual. AI defaults to omitting scope limitations; OECD states them explicitly and follows with the negative implication.

**AA. Data-then-qualification** — OECD presents a headline finding and immediately qualifies it with jurisdiction-level inconsistencies.

> "On average, staff numbers and budgets increased. This, however, is not consistent across all jurisdictions, with a majority but not all seeing increases."

Pattern: "On average, [headline finding]. This, however, is not consistent across all [X], with [qualification]." — OECD presents the average first, then immediately notes that the average masks variation. This is distinct from "However" at the start of a new paragraph — it is a **within-sentence qualification** that follows the data statement. Verified in Competition Trends. AI defaults to presenting either the average or the variation; OECD presents both in immediate succession.

**AB. Alternative explanation** — OECD offers a simpler or more mundane explanation for a finding before offering more substantive interpretations.

> "This could simply be a time delay in cases feeding into the data, and it will be a trend worth monitoring in future editions of this report."

Pattern: "This could simply be [mundane explanation]" — OECD uses "simply" to signal that the boring explanation might be the correct one. This is a **genuine human fingerprint** — AI never defaults to the boring explanation. Verified in Competition Trends, Algorithmic Management.

**AC. Interaction analysis** — OECD examines how two variables interact, not just their individual effects.

> "Looking at interactions between staff and budgets, Figure 1.6 shows that in many jurisdictions (9 out of 12), at least one of the two variables (staff or budget) increased."
> "While the overall correlation between the two variables is positive but low (0.33), there are some notable outliers."

Pattern: "Looking at interactions between [X] and [Y], Figure [N] shows that [finding]." — OECD uses "interactions between" to examine how two variables relate to each other, not just how each one changes independently. Verified in Competition Trends, ESG Ratings. AI defaults to analysing variables independently; OECD examines their interaction.

**AD. Metric taxonomy with three categories** — OECD classifies a complex measurement landscape into a manageable number of categories, each with a label and a definition.

> "While there is not a single definition of the types of quantitative metrics, this report proposes a three-type classification:
> Input-based metrics refer to qualitative metrics that measure companies' efforts and commitments...
> Output-based metrics refer to quantitative metrics that measure the results of companies' efforts...
> Contextual metrics refer to quantitative metrics that provide context..."

Pattern: "This report proposes a [number]-type classification: [Type A] refer to [definition]..., [Type B] refer to [definition]..., [Type C] refer to [definition]..." — OECD creates explicit taxonomies when a measurement landscape is complex. Each type is defined with "refer to" and a clear boundary. Verified in ESG Ratings. AI defaults to presenting metrics without classification; OECD creates explicit taxonomies with definitions.

**AE. Three-factor divergence explanation** — OECD explains why different measurement products disagree by decomposing the divergence into factors with percentages.

> "Empirical findings highlighted that 'measurement divergence' is the main driver of rating divergence accounting for 56% of the divergence across products, followed by 'scope divergence' (38%) and 'weight divergence' (6%)."

Pattern: "[X divergence] is the main driver accounting for [N]% of [total], followed by [Y divergence] ([M]%) and [Z divergence] ([K]%)." — OECD decomposes a complex phenomenon into factors with precise percentages, always in descending order. Verified in ESG Ratings. AI defaults to qualitative statements like "several factors contribute"; OECD quantifies the contribution of each factor.

**AF. The "despite [progress], [gap persists]" concessive-data pattern** — OECD uses "despite" to introduce a positive fact that makes the subsequent negative finding more surprising and policy-relevant. This is distinct from "although" (§4-L) which introduces a general concession. "Despite" specifically pairs **concrete progress** with **concrete remaining gaps**.

> "Despite significant progress over the past decade, Mexico continues to face high income inequality, poverty, and informality."
> "Despite pressing spending needs in areas such as education, public spending in Mexico is low at less than 30% of GDP."
> "Despite their clear relevance, one-third of the countries surveyed have only one of the two sets of integrity standards."

Pattern: "Despite [specific progress], [subject] [continues to / still] [specific gap]." — The "despite" clause must contain a **concrete positive** (not abstract "efforts were made"); the main clause must contain a **concrete gap** (not vague "challenges remain"). Verified in Philanthropy Study, PMR Evidence, RBC Guidance, Capacity Assessment. **Deploy at least once per country-assessment opening paragraph.**

**AG. The "data shows a complex interaction" hedge** — OECD explicitly acknowledges when the data does not tell a simple story. Instead of forcing a clean narrative, OECD names the complexity. This is a hallmark of institutional humility.

> "The data shows a complex interaction between poverty levels and allocation of philanthropic resources."
> "The share of variation explained by the model is low, which suggests a complex relationship between funding allocation and poverty levels."
> "This suggests that, on average, municipalities with higher poverty levels tend to receive less philanthropic support."

Pattern: "The data shows / reveals a complex interaction between [X] and [Y]." — Followed by "The share of variation explained by the model is low" or equivalent methodological caveat. AI forces clean narratives from messy data; OECD **names the messiness**. Verified in Philanthropy Study, Working Paper. **Use when data does not support a simple causal story.**

**AH. The "lag behind best practice" institutional-gap framing** — OECD uses "lag behind" to frame a country's or sector's regulatory state relative to an international benchmark. This is the PMR/institutional-assessment genre's equivalent of the "affirmative + but" pattern (T1), but at the **systemic level** rather than the sentence level.

> "The regulatory frameworks to support transparency and accountability in the interactions between interest groups and public officials lag behind best practices in many countries."
> "Essential disclosure requirements for lobbyists and public officials are missing in many countries, despite recent improvements in some countries."
> "Reforms have been undertaken, but there is a clear need for greater alignment with international best practices."

Pattern: "[Subject] lag(s) behind best practice / international standards in [domain]." — Always paired with a specific indicator or data point showing the gap. The benchmark is "best practice" or "international standards" or a named OECD Recommendation. Verified in PMR Evidence, Anti-Corruption Outlook. **Use in regulatory-assessment and institutional-gap genres.**

**AI. The "a whole-of-society approach" multi-level governance cascade** — OECD frames policy solutions as requiring coordination across government levels (national, regional, local) and across policy domains. This is not a vague aspiration — it is a structural feature of how OECD organizes its policy recommendations.

> "A whole-of-society approach, involving all levels of government across policy domains ranging from integration of migrants to the labour force."
> "Co-ordination is critical to the circular transition, as the cross-cutting nature of the circular economy requires working across silos."
> "Responsibilities to achieve these goals are shared across levels of government."

Pattern: "[Policy challenge] requires a [whole-of-society / multi-level / cross-cutting] approach, involving [national/regional/local] government across policy domains ranging from [X] to [Y]." — AI tends to recommend actions to a single actor. OECD **always maps the governance architecture** — who does what at which level. Verified in Labour Shortages, Circular Economy, Trust Study. **Deploy at the opening of every policy-recommendation section.**

**AJ. The "In the case of [City/Country]" specific-case deep-dive** — OECD uses this transition to move from a general pattern to a specific, detailed example. The example is always a named city, country, or institution with specific programme names, dates, and data.

> "In the case of the Flanders region in Belgium, the Circular Economy Monitor Flanders (CE Monitor) was created as an extensive, multi-layered circular economy monitoring framework."
> "In the case of Leuven, Belgium, the built environment is the main focus of the Circular Economy Action Plan due to the sector's high impact on CO₂ emissions."
> "In the case of female-dominated healthcare jobs, despite a continuous increase in employment numbers, the health and social care sector has been persistently understaffed."

Pattern: "In the case of [specific entity], [general finding] manifests as [specific local form], [specific detail with data]." — AI uses "for example" or "such as." OECD uses **"In the case of"** for longer, deeper case studies that deserve their own paragraph. Verified in Circular Economy, Labour Shortages, Trust Study. **Deploy 2-4 times per country/city comparison section.**

**AK. The "this presents an opportunity... but also poses a challenge" balanced-opportunity-risk construction** — OECD identifies both the upside and the downside of a phenomenon in a single sentence, using parallel structure. This is not hedging — it is structural balance.

> "This presents an opportunity to create new knowledge and information, but also poses a challenge in terms of the capacity required to design and implement sustainable, efficient, and effective circular economy policies."
> "While setting minimum staff requirements may reduce workload for existing staff and improve the quality of care and patient safety, the risk is to create inefficiencies due to lack of flexibility in work organisation."

Pattern: "[X] presents an opportunity to [positive outcome], but also poses a challenge in terms of [specific risk]." — AI tends to present only the opportunity or only the risk. OECD **names both in the same sentence**. Verified in Circular Economy, Labour Shortages. **Deploy once per section introducing a new policy tool or mechanism.**

**AL. The "[country] recorded the largest [metric] ... driven by [specific cause]" country-spike explanation** — OECD isolates the single largest mover in a cross-country dataset, then traces its cause through a chain of specific, named factors (policy reform, commodity price, natural disaster). This is the data-report genre's version of the "In the case of" deep-dive (AJ), but more compressed and data-driven. Verified in Revenue Statistics, Financing SMEs.

> "Chile recorded the largest decline in its tax-to-GDP ratio among LAC countries in 2023, at 3.2 p.p. amid a slowdown in economic activity and lower mineral prices."
> "In the case of Peru, the fluctuation in bankruptcy rates does not necessarily capture the whole picture of SME exit dynamics, considering the high share of informality."

Pattern: "[Country] recorded the largest [increase/decrease] in [metric] among [group], at [N] [units] amid [context]. The [drop/increase] was primarily driven by [specific cause]." — AI tends to list all countries equally. OECD **spotlights the outlier and explains it**. Verified in Revenue Statistics, Financing SMEs. **Deploy in cross-country data analysis sections.**

**AM. The "a higher [ratio] does not necessarily mean [naïve interpretation]" ratio-decomposition caveat** — OECD explicitly warns readers against over-interpreting a ratio by explaining how its numerator and denominator can move independently. This is a hallmark of institutional statistical literacy. Verified in Revenue Statistics.

> "Therefore, a higher tax-to-GDP ratio does not necessarily mean that the amount of tax revenues has increased in nominal or real terms."

Pattern: "Therefore, a higher / lower [ratio] does not necessarily mean that [naïve interpretation]. [Explanation of numerator-denominator dynamics]." — AI reports ratios at face value. OECD **teaches the reader how to read them**. Verified in Revenue Statistics. **Deploy once per data section when introducing a key ratio that could be misinterpreted.**

**AN. The "[N] in [M] [group] reported [finding]" population-level statistic sentence** — OECD presents survey findings using a distinctive "N in M" or "N out of M" format that makes the prevalence immediately tangible. This is distinct from simple percentage reporting — it converts the percentage into a human-scale number. Verified in Gender Equality, Financing SMEs.

> "A record 8 in 10 SMEs (78%) reported an increase in interest rates in 2023."
> "36% of ever-partnered women report having experienced intimate partner violence (IPV) in their lifetime."
> "58% of students admitted to not listening to what the teacher says, nearly double the OECD average of 30%."

Pattern: "[N] in [M] [population group] [reported / experienced / admitted to] [finding], [compared to / nearly double] the [benchmark] of [X%]." — AI tends to report only the percentage. OECD **also provides the "N in M" equivalent** when the finding is policy-relevant and the audience needs to grasp scale. Verified in Gender Equality, Financing SMEs, Education Sweden. **Deploy when presenting survey findings with high policy salience.**

**AO. The "while [topic] is widely discussed and standardised, [adjacent topic] is less visible and varies more" visibility-asymmetry logic** — OECD establishes a topic's relative invisibility by contrasting it with a well-known adjacent field. This creates the rationale for the paper's existence. Verified in Managing Government Cash, Lobbying Regulation.

> "While public debt management is widely discussed, highly transparent and a largely standardized part of public policy in the OECD countries, government cash management is less discussed, less visible and varies much more across countries."
> "While opportunities and risks exist for women and girls in digital environments, TF-GBV presents a significant and growing risk."

Pattern: "While [well-known topic] is widely discussed / standardised / transparent, [paper's topic] is less discussed / less visible / varies more." — AI tends to introduce a topic in isolation. OECD **positions it against a known reference point** to justify why the paper matters. Verified in Managing Government Cash. **Deploy in introductions of papers covering under-studied policy areas.**

**AP. The "there is no single optimal model for [X]. Best practices depend on the local context" anti-prescriptive logic** — OECD explicitly rejects one-size-fits-all recommendations, instead presenting a menu of practices that vary by context. This is the institutional equivalent of "however" — it qualifies everything that follows. Verified in Managing Government Cash, Scenario Planning.

> "There is no single optimal model for cash management. Best practices depend on the local context, including factors such as the agreements with the central bank, market depth, risk appetite, governance and funding environment."
> "It does not attempt to prescribe a uniform set of policies and practices; rather, it serves as a valuable reference for policy makers and practitioners by outlining different OECD country practices and the contexts underpinning them."

Pattern: "There is no single optimal model for [X]. Best practices depend on [list of contextual factors]." — AI defaults to prescriptive recommendations. OECD **explicitly resists prescription** in practice-review and survey genres, presenting context-dependent options instead. Verified in Managing Government Cash. **Deploy in practice-review, institutional-survey, and comparative-governance genres.**

**AQ. The "a cascading chain from [trigger] → [intermediate effect] → [final catastrophe]" multi-hazard cascade logic** — OECD traces how one physical event triggers a chain of increasingly severe consequences. This is not simple cause-effect — it is a **hazard cascade** where each link amplifies the next. Verified in Disaster Risk, Climate Policy.

> "Increased glacial melting enhances river flood risk due to greater downstream water flow. Moreover, increased melting adds more water to glacial lakes, elevating the risk of glacial lake outburst floods. More torrential river flows also exacerbate landslide risk by eroding the toes of previous landslides, which promotes further slippage."
> "These distortions can, in turn, perpetuate market dominance and hinder the natural forces of competition and market selection that drive innovation and productivity improvements."

Pattern: "[Trigger] enhances [risk A]. Moreover, [trigger] adds [risk B]. [Risk A] also exacerbates [risk C] by [mechanism]." — AI tends to describe hazards in isolation. OECD **chains them into cascading sequences** where each link amplifies the next. Verified in Disaster Risk. **Deploy in risk-assessment, climate-policy, and compound-hazard genres.**

### Avoid in logical flow
- Unsupported superlatives without data ("the best", "the worst")
- Emotional language ("devastating", "alarming")
- Vague causation ("things got worse because of stuff")
- Unanchored comparatives ("more", "less", "higher" — always say compared to what)
- "Due to" at sentence start (OECD prefers "Given" or "Owing to")
- "Because" in formal prose (OECD uses "as", "since", or "given")
- "However" as the only contrast connector (vary with "Nonetheless", "In contrast", "On the other hand", "By contrast")
- "Furthermore" / "Moreover" when the function is scope-widening (use "More broadly" instead)

---

## 5. Rewrite Protocol (改写流程)

When rewriting existing text, apply these transformations in order:

### Step 0: Diagnose the failure modes first
Before rewriting, identify which OECD principles the original violates. Common failures:
- **Abstract-noun subjects everywhere** ("instruments operate", "the framework reflects", "the interplay shapes") → flag for §2 subject replacement
- **Uniform sentence length** (all long, all short) → flag for §2 rhythm restructuring
- **Conceptual scaffolding opening** ("Publicly financed systems deploy a toolkit...") → flag for §2 opening-move rewrite
- **Translation-ese verbs** ("deploy a toolkit", "operate along", "applied at") → flag for §1 diction
- **Stacked subordination instead of parallel semicolons** → flag for §2 syntactic restructuring

### Step 1: Strip colloquialisms
Replace informal or journalistic language with OECD register vocabulary (§1).

### Step 2: Restructure sentences
Apply OECD sentence patterns (§2). Key moves:
- Embed data inline instead of in separate sentences
- Replace "X is Y because Z" with "X is Y. This reflects Z."
- Convert short choppy sentences into compound sentences with connectives

### Step 3: Add data anchoring
If the original text mentions facts without quantifying them, add numbers where possible. If no data is available, use hedged language: "a significant share", "a substantial proportion".

### Step 4: Apply structural template
Reorganize paragraphs into Topic sentence → Evidence → Implication (§3).

### Step 5: Strengthen logical connectives
Replace implicit logic with explicit connectives (§4). Every paragraph should have at least one logical connector.

### Step 6: Verify tone
- No first person ("I", "we")
- No exclamation marks
- No rhetorical questions in running text
- Hedged, not absolute: "tends to", "is likely to", "appears to"
- Institutional neutrality: present findings without advocacy language

---

## 6. Quick Diagnostic Checklist

Before finalizing any output, verify:

**Lexical layer (§1)**
- [ ] No colloquial words (help, big, show, about, get worse, problem, good/bad)
- [ ] No translation-ese verbs (deploy a toolkit, operate along, levers applied)
- [ ] No emotional adjectives (huge, alarming, devastating, amazing, terrible)
- [ ] Verbs drawn from the right family: trend / state / policy / analytical / recommendation
- [ ] **Hedging applied** to projections and judgements (appears to, tends to, is expected to)
- [ ] At least one **adverbial dampener / intensifier** (broadly, relatively, notably, largely, considerably)
- [ ] At least one signature collocation (in line with, stood at, in real terms, this reflects)
- [ ] At least one **tricolon** (rule of three) in section openers or recommendations

**Syntactic layer (§2)**
- [ ] **First sentence states a fact, not a concept** — no scaffolding openings
- [ ] **At least one short sentence (≤ 12 words) per paragraph** as a pivot
- [ ] **Concrete, named subjects** dominate (country, regulator, instrument), not stacked abstract nouns
- [ ] **Sentence rhythm varies**: 中长 → 短 → 长 → 短 → 中长 (no uniform length)
- [ ] Parallel mechanisms / stages joined with **semicolons**, not nested subordination
- [ ] Tenses applied correctly: present perfect for trends, past simple for dated events, "is expected to" for projections, "should" for recommendations
- [ ] **End-focus** observed: new / heavy information at end of sentence
- [ ] **Active voice dominates** (~70-80%); passive only where the agent is irrelevant or institutional

**Cohesion layer (§2.9) — the crunchiness check**
- [ ] **No meta-discourse**: no "Two strands of debate", "The first / The second", "We now turn to"
- [ ] **No subjective evaluation as fact**: no "the data are striking / alarming / remarkable"
- [ ] **Transitions embedded** inside content sentences ("by contrast", "while", "however"), not standalone signposts
- [ ] **Lexical chains** maintained — key terms repeated or lightly varied, not replaced with synonyms each time
- [ ] **Demonstrative bridges** ("this pattern", "these findings", "this variation") used to link sentences
- [ ] **Paragraphs are dense** (5-10 sentences, 100-250 words) — opposing views often kept in same paragraph, not split
- [ ] **Subject chains** — predicate of one sentence becomes subject of the next where natural

**Numerical and structural layer (§3)**
- [ ] Numbers embedded inline with unit + benchmark + percentage
- [ ] Comparisons always anchored ("above the OECD average", "compared to 2022", "in real terms")
- [ ] British English spelling throughout
- [ ] At least one logical connective per paragraph
- [ ] Recommendations use "should" or "it is recommended to"
- [ ] No first person, no exclamation marks, no rhetorical questions
- [ ] Data sources cited in parentheses or notes

---

## 7. Worked Example

**Before (raw text):**
> Canada's economy did well during 2024. GDP growth was okay. But there are big problems coming from trade with the US. Housing is really expensive. Also climate change is a huge issue and productivity is bad.

**After (OECD style):**
> Canada's economy has been resilient, with growth picking up over 2024. However, the rise in trade barriers with the United States is significantly weighing on the economic outlook. Housing affordability has deteriorated, with house prices and rents having increased more strongly than in most other OECD countries, driven by an insufficient supply of housing and strong population growth. Furthermore, climate-related risks from rising temperatures and extreme weather events are increasingly impacting the economy and communities. Strengthening Canada's productivity performance, which has lagged behind its peers, requires a combination of policies, including rebalancing R&D support, reducing regulatory barriers, and enhancing competition.

---

## 8. Failure Case Study (反面教材)

This case shows the most common failure mode: **vocabulary-only rewrite without rhythm or subject reform**.

**Original (academic English with translation-ese):**
> Publicly financed health systems deploy a toolkit of pharmaceutical cost containment measures to balance fiscal sustainability, patient access, and incentives for innovation. These instruments operate along a drug's commercial lifecycle, with different levers applied at market entry, during patent exclusivity, and after patent expiry. Ireland's framework follows this lifecycle logic, using pricing negotiation and pharmacoeconomic assessment at entry, rebate arrangements during exclusivity, and generic or biosimilar substitution with price reduction of patent prescription drugs after they lost patent and exclusivity status. Understanding how these tools interact is essential context before analysing patterns in PCRS expenditure data.

**❌ Failed rewrite (only swapped words, kept the bad architecture):**
> Publicly financed health systems rely on a range of pharmaceutical cost-containment measures designed to reconcile fiscal sustainability with patient access and innovation incentives. These instruments are deployed at successive stages of a drug's commercial lifecycle — at market entry, during the period of patent-based exclusivity, and following patent expiry. Ireland's pharmaceutical pricing framework reflects this lifecycle logic: ...

Why this fails:
- All three sentences open with abstract-noun subjects ("systems rely on", "instruments are deployed", "framework reflects") — violates §2 subject preference
- Uniform sentence length (all 25-40 words) — violates §2 rhythm
- Conceptual scaffolding opening — violates §2 opening moves
- Lexical upgrade alone is insufficient

**✓ Successful rewrite (rhythm + concrete subjects + parallel structure):**
> Cost-containment measures for pharmaceuticals are widely used in publicly financed health systems, balancing fiscal sustainability, patient access, and incentives for innovation. These instruments apply at different stages of a drug's commercial lifecycle. At market entry, regulators negotiate prices and conduct pharmacoeconomic assessments; during the period of patent exclusivity, rebate arrangements contain cost growth; once patents expire, generic and biosimilar substitution, combined with mandated price reductions, brings prices down further. Ireland's framework follows this lifecycle logic (Pharmaceutical Pricing and Reimbursement Information Network, 2024). The interaction of these instruments shapes the spending patterns observed in the Primary Care Reimbursement Service (PCRS) and provides the analytical context for the trends examined below.

Why this works:
- **Rhythm**: 中长 → 短 → 长(分号三段并列) → 短 → 中长 ✓
- **Concrete subjects**: regulators, rebate arrangements, substitution, Ireland's framework — not "instruments / framework / interplay" ✓
- **Opening fact, not concept**: starts with "Cost-containment measures for pharmaceuticals are widely used" — a stated fact, not scaffolding ✓
- **Parallel semicolons** carry the three lifecycle stages — characteristic OECD move ✓
- **Pivot short sentence** ("These instruments apply at different stages of a drug's commercial lifecycle.") sets up the long parallel sentence ✓

**Lesson**: Rewriting OECD style is not a thesaurus exercise. It requires restructuring **subjects, rhythm, and openings** before vocabulary.

---

## 9. Genre-Specific Patterns (体裁差异)

OECD output is not monolithic. Different publication types have distinct openings, densities, and tonal calibrations. Match the genre.

**These profiles are presets of the six dials in Step 0b.** Each one records the dial settings and surface conventions for a genre that has been sampled. Use them two ways: (a) if your target genre is listed, read its profile to confirm opening pattern, citation density, recommendation format, and structure; (b) if your target genre is *not* listed, do not scroll for the closest-looking profile and copy it — instead set the six dials from the request (Step 0b) and apply the ten moves, then borrow surface conventions from whichever listed profile shares your dial settings. The profiles are a lookup of common dial combinations, not the boundary of what the style can produce.

### 9.1 Economic Survey chapters (深度章节正文)

**Tone**: analytical, dense, recommendation-anchored.
**Length**: paragraphs of 150–300 words; chapters of 8000+ words.
**Opening**: a state-of-play sentence or a "set to" projection.
> "The fiscal situation is set to remain strong in the short term, with a further decline in the public debt-to-GDP ratio."
> "Demographic change will significantly increase public spending pressures in the next two decades."

**Signature features**:
- Dense data integration (every paragraph has at least one number)
- Embedded "(OECD, 2024)" / "(EC, 2024)" citations every 2–3 sentences
- Recommendations interleaved with diagnosis, not segregated to a final section
- Heavy use of **"set to"** (forecast), **"would help"** (conditional benefit), **"should"** (firm recommendation)
- Headings often in **gerund form**: "Strengthening fiscal policy", "Addressing rising pension spending", "Improving the effectiveness of social protection"

### 9.2 Executive summaries (执行摘要)

**Tone**: assertive, conclusive, parallel.
**Length**: 1–2 pages; 5–8 thematic blocks.
**Structure**: each block has a **gerund-phrase subtitle** followed by 2–4 dense sentences.

**Signature subtitle pattern** (the OECD executive-summary fingerprint):
- "The economy remains resilient but structural challenges weigh on future growth"
- "Growth is set to stabilise, but risks remain elevated"
- "Fiscal prudence and productivity-enhancing reforms are needed to safeguard public finances"
- "Tackling Portugal's housing affordability challenge will require a comprehensive reform package"
- "Strengthening training and activation to address population ageing and skill shortages"

These subtitles are **complete statements**, not topic labels. They function as headlines.

**Opening sentence pattern under each subtitle**: a quantified state-of-play sentence.
> "Portugal has achieved primary surpluses since 2022 and significantly reduced its public debt to 94.9% of GDP in 2024."

### 9.3 Country profiles / "at a Glance" briefs (国家速览)

**Tone**: descriptive, comparative, abstract-frame-then-data.
**Length**: short paragraphs of 50–150 words built around one indicator.
**Distinctive opening pattern**: **abstract universal proposition** followed immediately by quantified country result + OECD benchmark.

This is the **one OECD genre where abstract openings are conventional**. Example:

> "Trust in public institutions, levels of shared prosperity and satisfaction with public services are important yardsticks of the quality of public governance. They reflect both the outcomes of government actions and people's perceptions of government competence. **In Chile, 30% of people had high or moderately high trust in the national government, below the OECD average of 39% in 2023.** Moreover, a majority (51%) were satisfied with the administrative services they used, below the OECD average of 66%."

The pattern is fixed: 1–2 sentences of conceptual framing → "**In [country],** [number]% [indicator], [above/below] the OECD average of [number]%."

**Do not** apply this opening pattern to economic surveys or chapter prose — there it would be the AI-default scaffolding flagged in §1.8. Country profiles are the exception.

### 9.4 Development cooperation profiles (DAC / ODA profiles)

**Tone**: data-dense, descriptive, almost entirely declarative.
**Length**: paragraphs of 30–80 words; mostly bullets and figure callouts.
**Opening**: **"In [year], [country] [verb] [amount]"** — pure data-first.
> "In 2024, the Netherlands provided USD 7.5 billion of ODA, representing 0.62% of GNI."
> "In 2023, the United Kingdom committed 61.4% of screened bilateral allocable ODA to gender equality."

**Signature features**:
- Numbers spelled in words at sentence start: "**Twenty-one per cent** of screened bilateral ODA…"
- Repeated `[country]:` table headers
- Almost no analysis; the data carries the weight
- "Additionally" / "In addition" / "Moreover" link parallel data points
- "Learn more about" links to OECD initiatives at end of bullets

### 9.5 Anti-bribery / peer-review evaluations (合规法务报告)

**Tone**: formal-procedural, third-person institutional, judiciously evaluative.
**Length**: long paragraphs of 200–500 words.
**Distinctive subject**: "**The lead examiners**" — used as the active subject of evaluative sentences.

**Signature verb cluster for this genre**:
- "The lead examiners **commend** [country] for…"
- "The lead examiners **note** that…"
- "The lead examiners **observe** that…"
- "The lead examiners **further observe** that…"
- "The lead examiners **consider** that…"
- "The lead examiners **welcome** [country]'s adoption of…"
- "The lead examiners **recommend** that…"

**Concession-heavy structure**: every commendation is paired with a "however" / "nevertheless" / "at the same time":
> "The lead examiners commend Argentina for the progress achieved... **Nevertheless, the lead examiners note that** Argentina's foreign bribery enforcement remains limited and uneven."

**Numbered paragraph format**: paragraphs prefixed with sequential numbers (7., 8., 9., 10.) — a peer-review convention.

**Follow-up report logic patterns** (verified in Anti-Bribery Phase 4 Follow-up):

This genre has its own **argumentation logic** that is distinct from all other OECD genres:

**(a) Recommendation-Status-Assessment triad** — every paragraph follows: "Recommendation X – [Status]: [Assessment]."
> "Recommendation 3(b) – Partially implemented: The Phase 4 Report questioned whether ACPO had sufficient resources…"

Statuses are: **"Fully implemented"**, **"Partially implemented"**, **"Not implemented"**. These three phrases are the genre's backbone. Verified: 81 "Not implemented", 44 "Partially implemented", 30 "Fully implemented" in a single report.

**(b) The direct negative assessment** — this genre uses the bluntest language in all of OECD prose. No hedging, no softening.
> "**Spain has not taken any steps** to implement this recommendation."
> "Spain has not taken any action to address this issue."
> "Spain has not provided guidance or training…"

Pattern: "[Country] has not [past participle]…" — verified 12 times in one report. This is the OECD author at their most direct. AI would never write this bluntly — it would soften to "Spain has not yet fully addressed" or "Spain could further strengthen its efforts".

**(c) The "merely restates" rebuttal** — when a country claims compliance but the substance hasn't changed.
> "The Circular therefore **does not change but merely restates** the law as it existed at the time of the Phase 4 Report."
> "Spain **merely restates** the law and practice which are unchanged since Phase 4."

Pattern: "[Country] merely restates [X]" / "does not change but merely restates" — the OECD way of saying "nothing happened". Verified 6 times.

**(d) The "ostensibly" skepticism marker** — when a country's justification is doubtful.
> "This is **ostensibly** because the length of a penalty against a legal person cannot exceed the maximum term of imprisonment…"

"Ostensibly" = "this is the stated reason but we don't believe it". Verified 4 times.

**(e) The "at best" dismissive qualifier** — when a country's argument is weak.
> "Yet such impact is vague and **at best** speculative."
> "A longer limitation period of 15 years therefore also arguably applies only in such exceptional cases, **at best**."

"at best" = "even in the most generous interpretation, this is inadequate". Verified 2 times.

**(f) The quantified inference** — using numbers to prove a point.
> "**That only 2 out of 19 cases** have employed a broad range of investigative techniques **suggests that** the Working Group's recommendation is only partially implemented."

Pattern: "That only X out of Y [have/has] [done Z] suggests that…" — the OECD way of using evidence to draw an inference. This is the opposite of AI's vague "This highlights the need for improvement".

**(g) The "this contradicts" rebuttal** — when a country's current position conflicts with its earlier one.
> "Spain argues that the current version of Art. 408 CC already covers all officials, but **this contradicts** Spain's position during the Phase 4 evaluation."

Pattern: "[Country] argues that X, but this contradicts [Country]'s position during [earlier phase]" — the OECD way of catching inconsistencies.

**(h) The "underscores the urgent need" synthesis** — when multiple weak arguments prove the need for reform.
> "Spain's multiple positions that lead to different limitation periods **merely underscore the urgent need** for clarification through legislative amendment."

Pattern: "[Country]'s [multiple/conflicting] [positions/arguments] merely underscore the urgent need for [action]" — the OECD way of saying "your own confusion proves you need to fix this".

**(i) The "While positive, [evidence] shows insufficiency" pattern** — acknowledging partial progress while proving it's not enough.
> "**While these efforts are positive**, Spain has 19 ongoing foreign bribery cases. **That only 2 out of 19 cases** have employed a broad range of investigative techniques **suggests that** the Working Group's recommendation is only partially implemented."

Pattern: "While [positive fact], [quantifier]. That only X out of Y [evidence] suggests that [conclusion]." — this is the OECD author's most sophisticated assessment pattern: concede the positive, then demolish it with data.

**(j) The "no case law supporting" evidentiary challenge** — when a country claims legal authority without precedent.
> "There is also **no case law supporting** this new position."
> "Again, **there is no case law supporting** any of these interpretations."

Pattern: "There is no case law supporting [Country]'s [position/interpretation]" — the OECD way of saying "you made this up".

**Anti-AI note for this genre**: AI cannot write in this register. It would soften every negative assessment, add hedging where none exists, and replace "Spain has not taken any steps" with "Spain has made limited progress in implementing this recommendation." The directness of this genre is its defining feature — and the strongest anti-AI signal in all of OECD prose.

### 9.6 Policy briefs / Policy primers (短篇政策简报 / 政策入门读物)

**Tone**: conversational-formal, action-oriented, recommendation-led, **deliberately accessible**.
**Length**: 4–8 pages; "Key messages" bullets at top.
**Opening**: **"Key messages"** as bullets, each starting with a complete claim.

**Signature features**:
- Bullets at the start of the document with main findings
- **Question-form section headings**: "What can policymakers do?", "What are quantum technologies?", "What risks do they raise?", "What's the issue?"
- Direct active-voice prose ("Criminals use", "Governments must")
- "**Governments should:**" / "**Policymakers should:**" introducing recommendation lists
- Recommendations as bullet lists with bold lead phrase + explanation
- **No inline citations** in the body (the brief is the executive distillation; the underlying paper carries citations)
- "**In summary**" / "**To conclude**" closes are acceptable here (and only here)
- "Furthermore" / "Moreover" / "Additionally" used freely (in Surveys these read as AI; in primers they signal accessibility)
- Rhetorical structure: question → answer → recommendation
- Shorter sentences (15-25 words) than Survey prose
- Verbal forms preferred over nominalisations ("policymakers can map skill demands" not "the mapping of skill demands by policymakers")

**Trap to avoid**: when rewriting Policy Primer content, do **not** import Economic Survey fingerprints (citations, "albeit", "in practice", heavy nominalisations, dense preposition stacks). Primers are deliberately a different register. Cross-importing Survey-style scaffolding into a Primer breaks the genre.

### 9.7 Country Reviews — Education, Health, Skills, etc.

**Tone**: analytical with a slight **human warmth** that is unique to this genre. Phrases like "thrive", "those who need them most", "a real opportunity", "shared ownership" are conventional here and would be flagged as AI-default elsewhere.
**Length**: 100,000+ words; chapters of 5,000–10,000 words; paragraphs of 100–250 words.
**Opening pattern**: a state-of-play sentence with mild narrative framing.
> "An unprecedented level of national and European funding, new legislation adopted in 2023 sets out an ambitious vision to enhance the quality and availability of education and training."

**Signature features**:
- Heavy citation density (Education Review: ~1 citation every 3 sentences in analytical chapters, similar to Survey)
- Health Performance Reports often citation-light because they are normative-procedural rather than evidence-aggregating
- "Considerations" / "this review highlights three considerations" — softer than Survey "recommendations"
- Comparative framing: "compared to peers", "across OECD countries", "in EU and OECD countries"
- Stakeholder vocabulary: "stakeholder participation", "shared ownership", "multi-level governance"
- More **gerund subjects** allowed: "Strengthening school leadership... could support improvements"
- **Avoid** Latinate connectives ("albeit", "inter alia", "thereby") — these are Survey markers and feel out of place in Reviews
- **Avoid** "in practice" — also a Survey marker; Reviews use "on the ground", "in delivery", "in implementation" instead

**Country Review pillar + recommendation structure** — each thematic pillar opens with a prose paragraph of diagnosis (100-200 words), then transitions to bullet-point recommendations starting with imperative verbs. The prose paragraph blends diagnosis with policy implications in one continuous flow, never splitting "analysis" from "recommendations" into separate sections.

> **Building a resilient rural economy** Rural economic diversification requires systematic entrepreneurial discovery, differentiated labour market strategies, and integration of social innovation pathways.
> - Develop systematic rural entrepreneurial discovery process
> - Embed spatial skills intelligence within Ireland's skills architecture
> - Strengthen rural business ecosystem and address SME funding gaps

**Country Review diagnostic table** — Country Reviews use a three-column diagnostic framework: "What works / What does not work / What should be prioritised". This is the standard OECD assessment grid for Country Reviews, not found in Surveys or Primers.

> | Key Questions | What works | What does not work | What should be prioritised |
> |---|---|---|---|

**Country Review evaluation verbs** — "demonstrates", "reveals", "underscores", "highlights" appear in assessment paragraphs as evaluative framing:
> "ORF's breadth **demonstrates** genuine whole-of-government ambition."
> "The monitoring framework **reveals** a critical disconnect between national oversight and local reality."

**Country Review rhetorical devices** — subtle metaphorical language is conventional in Country Reviews (unlike the strictly literal Surveys):
> "Fragmented childcare, transport, digital and water services **quietly erode** rural viability."
> "The enduring 'rural idyll' **still shapes** perceptions of what rural means."
> "The **path forward** lies in sharper spatial intelligence."

### 9.8 Working Papers (研究论文)

**Tone**: academic, methodologically explicit, hedged, first-person plural.
**Length**: 30–80 pages; abstract + introduction + data + method + results + discussion.
**Opening (abstract)**: "This paper examines / This paper investigates / This paper assesses…"

**Signature features**:
- **First-person "we" voice** allowed and conventional — "We find that…", "We focus on five OECD countries", "Our contribution is therefore to test whether…"
- Methodological hedging: "The estimates should be interpreted as descriptive", "Remaining omitted variables could bias coefficients", "The small number of clusters limits inference"
- Heavy academic citation: "(Andreadis et al., 2025)", "(Acemoglu and Restrepo, 2020)", "(Dixit and Pindyck, 1994)" — author–year format, not OECD-style "(OECD, 2024)"
- **JEL classification codes** in metadata: "JEL classification: O33; H74; G12"
- **Keywords** field
- "**Building on** [prior literature]" / "**Consistent with** [prior finding]" / "**In contrast to**"
- Section heading numbering: "1. Introduction", "2. Data and Measurement", "3. Empirical Strategy", "4. Main Results"
- Equations and variable definitions inline: "Where b denotes the bond yield in country c and year t"
- Reference to figures by number: "Figure 2 plots the bivariate relationship..."
- No "should" recommendations — instead: "These findings suggest...", "Future work could examine..."

**Avoid in Working Papers**:
- Survey-style "set to" projections (Working Papers describe past, not forecast)
- Recommendation language ("[Country] should…")
- Executive-summary gerund subtitles
- Country-profile abstract opens

### 9.9 Trade Policy Brief / Industry Analysis (贸易政策简报 / 行业分析)

**Tone**: analytical-advocacy, data-driven, balanced but with a clear argument.
**Length**: 6–12 pages; "Key messages" bullets at top.
**Opening**: "Key messages" bullets, then **"What's the issue?"** as first section heading.

**Signature structure** (3-part):
1. **"What's the issue?"** — analytical diagnosis with OECD database evidence
2. **"Why is this important?"** — broader implications for trade, competition, security
3. **"Explore further"** — references to underlying OECD working papers

**Distinctive features**:
- **Creative subtitles** are acceptable in this genre (rare in OECD): "Too close to the sun"
- **Multi-causal explanation pattern**: "[X] cannot be attributed to [Y] alone; rather, it appears to reflect also [Z]" — the OECD way of explaining complex causation
- **Balanced assessment of policy instruments**: "While [X] can be useful policy instruments for addressing certain market failures, they can also have negative consequences when they exceed what is necessary for ensuring well-functioning markets."
- **Lesson-drawing pattern**: "The experience of [X] is illustrative of what can happen when [Y]"
- **Cooperation imperative**: "As market dominance built on subsidies has global market implications, and as countries risk a further subsidy race in endeavouring to create or maintain alternative supply capacity, it is important that countries co-operate to address the root causes"
- Heavy use of OECD databases (MAGIC database, Trade Policy Papers)
- Data tables with source notes: "Source: OECD MAGIC database."
- No inline citations in body; references consolidated in "Explore further"
- Question-form headings ("What's the issue?", "Why is this important?")
- "What does this mean for trade policy?" as a bridging heading

### 9.10 Financial Market Working Paper / Policy Paper (金融市场工作论文)

**Tone**: technical, extremely dense, neutral-analytical, committee-oriented.
**Length**: 30–80 pages; executive summary + numbered chapters.
**Opening (Foreword)**: "This paper provides an update to earlier OECD work on [X], examines [Y], discusses [Z], and considers [W]."

**Signature features**:
- **Acknowledgments section** listing contributors by name, institution, and sometimes country — a financial-market-paper convention
- **Committee discussion dates** in metadata: "was discussed by the Committee in May 2024 and October 2024"
- **Box format for case studies**: "Box 1. Project Helvetia", "Box 2. The Digital Securities Sandbox" — standalone boxed narratives within the paper
- **Neutrality disclaimer**: "without taking a position on whether public authorities should address these obstacles or how they might do so"
- **Parenthetical principle citations**: "(same activity, same risk, same regulation)" — the OECD way of citing a regulatory principle
- **Paper purpose statement**: "The objective of the paper is to identify, in an analytic manner, some of the obstacles to…"
- Dense parenthetical citations: "(OECD, 2020)", "(FSB, 2024)", "(Carapella et al., 2023)" — mixed OECD and academic formats
- "Notwithstanding" as concessive opener: "Notwithstanding the growing momentum in communication by market participants…"
- "It is also important to note that…" — methodological caveat (acceptable in this genre, unlike in Survey prose)
- "Indeed, it is reasonable to expect…" — moderate confidence marker
- "That said" as mid-paragraph pivot: "That said, there are currently limited comprehensive and consistent public data available…"
- Lists of hypotheses or obstacles as bullet points with brief elaboration
- "e.g." used freely within sentences (not "such as" exclusively)

### 9.11 Country Policy Assessment Notes (国家政策评估笔记)

**Tone**: descriptive-inventory, evaluative but restrained, program-focused.
**Length**: 4–10 pages; structured by policy theme.
**Opening**: trend-with-comparison sentence using "yet" to signal tension.
> "The total self-employment rate increased slightly over the past decade **yet** remained below the EU average in 2023 (12% vs. 13%)."

**Signature features**:
- **Multi-group data presentation**: "People were less likely to be self-employed across all target groups relative to the EU average: women (8% vs. 10%), immigrants (10% vs. 11%), youth (5% vs. 7%) and seniors (15% vs. 17%)."
- **Counterpoint pattern**: "However, self-employed women (22%) and immigrants (42%) were more likely to have employees compared to their EU counterparts (26% and 31% each)."
- **Binary classification explanation**: "Repayable assistance is primarily intended for [X], while non-repayable assistance is targeted for [Y]."
- **Program description patterns**: "In [year], [institution] developed [program name], which aims to [objective]." / "So far, more than [number] [group] have successfully completed the programme."
- **Outcome statements**: "Overall, analysis shows that 80% of women entrepreneurs funded through this initiative survive for at least two years."
- **Gap description**: "Tailored [X] initiatives are less commonly available." / "Furthermore, some existing strategies and policies that aim to promote [X] have not been recently updated."
- **Policy change description**: "Nevertheless, incentives for [X] have no longer been granted since [year], although such support is still appearing at the [Y] level through [Z]."
- **Institutional introduction**: "[Institution] is the [type] established by the [government] to promote [X], [Y], [Z] and [W]."
- **Institutional affiliation**: "The agency operates under the [Ministry name]."
- Data source notes after tables: "Source: Eurostat (2024), Employment and Unemployment (LFS) Database; Global Entrepreneurship Monitor (GEM) (2024)."
- Detailed inventory of programs, institutions, and funding amounts
- Minimal analysis; the policy landscape carries the weight

### 9.12 Environmental / Sectoral Policy Brief (环境 / 行业政策简报)

**Tone**: evidence-based advocacy, scientific but accessible, multi-benefit framing.
**Length**: 6–12 pages; "Key messages" bullets at top.
**Opening**: "Key messages" bullets, then "What's the issue?" as first section heading.

**Signature features**:
- **Triple-benefit framing**: "Managing fish stocks in a way that preserves their health and productivity is a win-win-win strategy that can lead to greater benefits for fishers and improvements in food security, enhanced ocean ecosystems and reductions in greenhouse gas (GHG) emissions."
- **Progress-with-gap acknowledgment**: "Even so, there is room for improvement."
- **Colloquial math** (very human — the OECD author making data relatable): "And, of course, if 81% of assessed fish stocks are healthy, that still leaves one in five that aren't."
- **Knowledge gap acknowledgment**: "Our understanding of the relationship between the changing climate and marine ecosystems is incomplete. New research is needed to refine our understanding of how changes in ocean conditions may affect specific fish stocks and fisheries."
- **Parallel modal verbs for recommendation lists**: "This could mean conducting or supporting more regular and comprehensive [X]. It may require adjusting [Y]. Greater co-operation between [Z] would help to [W]." — each sentence uses a different modal verb to avoid monotony.
- **Uneven impact description**: "And as with [X], such impacts won't be evenly distributed: some areas are likely to experience larger declines, while others will see increases."
- **Scientific references** in "Explore further" section, not inline
- "What's the issue?" / "How can [X] help in a changing climate?" / "What can policymakers do?" structure
- "Contacts" section with named experts and email addresses at end
- "This work is published under the responsibility of the Secretary-General of the OECD." — standard disclaimer
- Creative commons licence block at end

### 9.13 Investment / Technology Policy Brief (投资 / 技术政策简报)

**Tone**: data-heavy, forward-looking but cautious, methodology-transparent.
**Length**: 8–15 pages; "Key messages" bullets at top.
**Opening**: "Key messages" bullets with detailed data points.

**Signature features**:
- **Ultra-short emphasis sentences** (rare in OECD — used for dramatic contrast): "National investment ecosystems differ."
- **Acknowledging public sector while highlighting private**: "While VC did not create AI's scientific foundations, developed over decades of government-funded research, its investments have drastically accelerated AI's diffusion."
- **Ratio comparisons**: "This sum, while based on an experimental methodology, is about 2.4 times higher than the 2023 total AI-related VC presented in this report, highlighting the important role of internal corporate and public sector investments in the AI ecosystem."
- **Standard caveats** (explicit, not hedged within prose): "It is important to note that investment markets are cyclical and past trends are not always accurately indicative of future performance."
- **Methodology transparency**: "Firms are identified as AI firms based on Preqin's cross-industry and vertical categorisation, as well as on the OECD's automated analysis of the keywords contained in the description of the activities of the firms captured in the Preqin dataset."
- **Scope limitation**: "The scope of this policy brief is limited to [X]; caution should be taken when drawing broader conclusions from this data as it offers only one vantage point relative to other forms of investment."
- **Historical revision caveat**: "Historical revisions and methodological improvements to the dataset can also impact results as deals, particularly smaller deals, are often added retroactively."
- **Balance of optimism and caution**: "While long-term signals point to major advances in AI, short- to medium-term investment outcomes remain uncertain."
- Detailed data tables with source notes: "Source: OECD.AI (2026), data from Preqin, last updated 2026-01-01."
- "What can policymakers do?" with bullet recommendations starting with imperative verbs
- Table format for lifecycle stages with examples from multiple countries
- Parenthetical company examples: "companies like Databricks, but also direct investments in model developers such as Anthropic, Mistral, and X.AI"

### 9.14 Security / Justice Policy Brief (安全 / 司法政策简报)

**Tone**: threat-focused, evidence-based, urgent but measured, cooperation-oriented.
**Length**: 6–12 pages; "Key messages" bullets at top.
**Opening**: "Key messages" bullets, then "What's the issue?" as first section heading.

**Signature features**:
- **Threat-focused opening**: "In the last three decades, fentanyl, other synthetic opioids, and new psychoactive substances have emerged and become a major public health threat."
- **Old-vs-new challenge framing**: "While existing [X] has largely focused on [Y], the emergence and rapid proliferation of [Z] poses new and unique challenges for [W]."
- **Actor adaptation description**: "[X] exploit advancements in [Y] and [Z] to adapt [W]."
- **Perspective-shift explanation**: "From a [X] perspective, the shift toward [Y] is facilitated by its [Z], its [W], and [V] compared to [U]."
- **Positive development introduction**: "Despite these challenges, some [X] are starting to yield results."
- **Tool-already-exists framing**: "Many of the effective tools, such as [X] and [Y], already exist; the challenge is to scale them up and adapt them to the fast-evolving nature of [Z]."
- **Cooperation imperative**: "Given the global nature of [X], no single country can tackle these challenges alone."
- **Quantified threat data**: "In [Country], over 80% of all overdose deaths are now attributed to synthetic opioids, with the fentanyl overdose death rate surging more than 100-fold between 2013 and 2023."
- **Expansion description**: "With its high profitability and low barriers to production, [X] trafficking is also expanding in regions such as [Y], [Z], and [W], where it was previously uncommon."
- **Challenge enumeration**: "However, challenges remain, including the need to [X], [Y], and [Z]."
- "What's the issue?" / "Why is this important?" / "What can policymakers do?" structure
- Data source notes: "Source: OECD, UNODC, EMCDDA."

---

### 9.16 Empirical Research Report / Survey-Based Study (实证研究报告)

**Tone**: analytical, evidence-claiming, balanced between promise and concern.
**Length**: 30–80 pages; Abstract + numbered chapters with question-form titles.
**Opening**: Abstract with balanced framing ("On the one hand... On the other hand..."), JEL codes, Keywords.

**Signature features**:
- **Balanced abstract framing**: "X — definition — has received increased attention. On the one hand... On the other hand... As policymakers grapple... additional evidence is needed. Towards this aim, this study draws on..."
- **Question-form section titles**: "How prevalent is [X]?", "How do [X] impact [Y]?", "Are [Z] worried about [W]?"
- **First-person institutional claim**: "This study offers unprecedented insights on..." / "This is also the first study to offer direct evidence on..."
- **Survey data description**: "The survey asked [respondents] to provide information about..."
- **Country-tier comparison ladder**: "[Country A] (90%) ... [Country B] (79%) ... [Country C] (40%)"
- **Percentage-heavy analytical prose**: "60% of managers cite improvement in the quality of work" / "only 6% in Europe and 8% in Japan"
- **Hedged causal attribution**: "The stronger impact observed in [X] could be due to the fact that..."
- **Analytical caveat**: "though it should be noted that [X] does not automatically equate to [Y]"
- **Alternative explanation**: "It is also possible that different [X] result from variation across [Y]"
- **Box format for background**: "Box 3. Brief on the OECD Employer Survey on Algorithmic Management"
- **Acknowledgements listing funding bodies**: "The authors would like to thank the [X] for funding this project"
- **Pattern**: this genre uses "On the one hand / On the other hand" in the **abstract only** to frame the policy tension — elsewhere it is banned (see §1.8B).
- **Anti-AI note**: AI defaults to one-sided claims; this genre **requires** balanced framing of benefits AND concerns in every analytical section.

---

### 9.17 Country Governance / Public Finance Study (国家治理 / 公共财政研究)

**Tone**: descriptive-institutional, reform-tracking, comparative.
**Length**: 30–60 pages; Foreword + numbered chapters with institutional focus.
**Opening**: Foreword acknowledging country cooperation, institutional attribution.

**Signature features**:
- **Cooperation acknowledgment**: "This paper was prepared by [Directorate] under the leadership of [Director], in close co-operation with the [Country Ministry]"
- **Four-pillar framework**: "In [year], the budget framework in [Country] was characterised by four pillars" / "Today, the four pillars remain in place along with reforms since [year]"
- **Three-level sub-section numbering**: "1.4.1.", "1.4.2." — deeper hierarchy than most OECD genres
- **Historical narrative**: "The [institution] was established in [year] with the objective of..."
- **Legal/institutional naming**: "The Significant Infrastructure Government Loan Act (SINGA)" — introduces abbreviations for laws
- **Constitutional provisions quoted**: "Singapore's Constitution stipulates that..."
- **"From an OECD perspective" marker**: "From an OECD perspective, these reforms would be reinforced by publishing macro-fiscal forecasts"
- **Temporal bridge**: "In [year], [X] was characterised by [Y]. Today, [X] remains in place along with reforms since [year]."
- **Nuanced institutional assessment**: "The collaboration shows well-defined yet closely connected responsibilities" — "yet" creates internal tension
- **Reform-tracking structure**: tracks how a country's institutions have evolved over time, comparing past state to current state
- **Anti-AI note**: AI defaults to describing institutions statically; this genre **requires** temporal evolution narrative — "was established in X, was characterised by Y, has since evolved to Z"

---

### 9.18 Annual Data / Trends Report (年度数据趋势报告)

**Tone**: descriptive-data, analytical, forward-looking.
**Length**: 40–80 pages; Foreword + numbered chapters with data focus + Annexes.
**Opening**: Foreword describing the data source (annual survey, database).

**Signature features**:
- **Database description**: "[X] is the premier source of policy analysis and advice on [Y], and a unique platform from which to monitor developments."
- **"In focus" label**: "In focus: [topic]" — for a deep-dive chapter within a data report
- **Regional snapshots**: "Regional snapshots" — geographic breakdown of data
- **Infographic summary**: "Overall Snapshot (Infographic)" — visual summary section
- **Annex with data sources**: "Annex A. Sources of [Database Name]"
- **Downloadable data reference**: "An Excel file with a complete set of graphs... can be found on the [X] publication website."
- **Hypothesis enumeration**: "There are several possible reasons which may explain the general trend. The possible reasons include: (i) X, (ii) Y, (iii) Z."
- **Data-then-qualification**: "On average, [X] increased. This, however, is not consistent across all [Y]."
- **Interaction analysis**: "Looking at interactions between [X] and [Y], Figure [N] shows that..."
- **Forward-looking monitoring commitment**: "it will be a trend worth monitoring in future editions of this report"
- **Alternative explanation**: "This could simply be a time delay in [X] feeding into the data"
- **Scope limitation**: "This chapter does not look at [X]. This means that none of the possible conclusions imply [Y]."
- **Anti-AI note**: AI defaults to presenting data without qualification; this genre **requires** every headline finding to be immediately qualified with "This, however, is not consistent across all [X]"

---

### 9.19 Empirical Analysis / Metric Assessment Report (实证分析 / 指标评估报告)

**Tone**: technical-analytical, taxonomy-creating, methodology-transparent.
**Length**: 40–80 pages; Foreword + Executive Summary with labeled findings + Annexes.
**Opening**: Foreword explaining policy context and mandate (e.g., G20).

**Signature features**:
- **Mandate reference**: "This report responds to a G20 mandate" / "In response to the rapid development of [X], [Y] has committed to [Z]"
- **Labeled findings in Executive Summary**: "Metric scope:", "Metric comparability:", "Metric characteristics:", "Looking forward:" — each finding gets its own label
- **Three-type classification**: "This report proposes a three-type classification: [Type A] refer to [definition]..., [Type B] refer to [definition]..., [Type C] refer to [definition]..."
- **Metric taxonomy**: "seven E-related topics, eight S-related topics and eight G-related topics"
- **Three-factor divergence explanation**: "'measurement divergence' is the main driver accounting for 56% of the divergence across products, followed by 'scope divergence' (38%) and 'weight divergence' (6%)"
- **Prior considerations section**: "1.4. Prior considerations" — methodological caveats before the analysis
- **Data limitation transparency**: "The OECD was unable to verify that all metrics used in the analysis are the most up-to-date versions"
- **Explicit exclusion**: "This analysis does not consider [X]" / "The analysis remains at the [Y] level"
- **Cross-referencing own institution's work**: "Other studies conducted by the OECD have also analysed that..."
- **"at odds with" connective**: "This siloed and topical structure is also at odds with recent sustainability-related standards structures"
- **Anti-AI note**: AI defaults to presenting findings without methodology caveats; this genre **requires** a "Prior considerations" section that explicitly lists data limitations and scope exclusions before the analysis begins.

---

### 9.20 Operational Guidance Manual / Toolkit (操作指南 / 工具包)

**Tone**: procedural, empowering, lifecycle-structured, cooperation-oriented.
**Length**: 50–200 pages; Preface (country official) + Foreword (OECD) + Abbreviations + Executive Summary with Caveat + numbered chapters.
**Opening**: Preface by a country official, then Foreword by OECD.

**Signature features**:
- **Country official Preface**: "We are proud that our country's [X] has inspired and contributed to the development of [Y]" — personal voice with institutional authority
- **OECD Foreword**: "This report seeks to encourage and support jurisdictions in the development of [X] for [Y] that apply throughout the [Z]"
- **Abbreviations list**: 20+ abbreviations/acronyms — operational manuals require a comprehensive glossary
- **Executive Summary with Caveat**: explicit acknowledgment that "a standard approach may be neither practical nor desirable"
- **Lifecycle structure**: chapters covering the full lifecycle from "Case referral, selection, and allocation" through "Post investigation procedures"
- **Minimum-requirements enumeration**: "At a minimum, the [X] should be designed to:" followed by 6+ bullet points with em-dash explanations
- **Country examples as evidence**: "The United States' [agency] makes all its staff manuals publicly available... Likewise, the [Country] [agency] publishes..."
- **Design considerations section**: "Design considerations" — meta-chapter about how to adapt the manual to local context
- **Periodic monitoring section**: "Periodic monitoring and updates" — the manual itself has a maintenance lifecycle
- **Tool-purpose sentence**: "This manual will serve as a crucial tool to bridge these gaps, providing a comprehensive set of guidelines that will empower [X] to conduct [Y]"
- **Benefit chain**: "This can enhance the quality, speed, and efficacy of [X], leading to better [Y]"
- **Anti-AI note**: AI defaults to generic "best practices"; this genre **requires** explicit country examples, lifecycle structure, and a caveat section acknowledging that one size does NOT fit all.

---

### 9.22 Regulatory / Legal Compliance Brief (监管合规法律简报)

**Tone**: precise, legalistic, comparative, obligation-focused.
**Length**: 10–40 pages; structured by regulatory domains with cross-country comparison tables.
**Opening**: Definitional paragraph establishing what the legislation covers, followed by geographic scope.

**Signature features**:
- **Definitional opening**: "For the purposes of [X], [term] refers to [precise definition]." — legal terms require exact definition before analysis begins
- **Obligation enumeration**: "These requirements are uniform, irrespective of an organisation's size and budget, which can pose challenges for smaller organisations with limited resources." — OECD enumerates specific obligations with their scope conditions
- **Cross-country compliance tables**: columns for country × obligation × status, with footnotes specifying data year and scope
- **"Authorised" / "mandated" / "required" verb cluster**: the compliance genre uses obligation-language, not recommendation-language
- **Scope-and-enforcement caveat**: "It must be stressed that [the indicators] measure the 'de jure' policies, but not actual enforcement."
- **Threshold language**: "As of [year], less than [X]% of [entities] hold [status]" — precise thresholds and deadlines
- **Anti-AI note**: AI defaults to descriptive summaries; this genre requires **precise obligation-scoping** — what is required, for whom, since when, and what happens if non-compliant. Every statement must be traceable to a specific legal instrument.

---

### 9.23 PMR / Indicator-Based Regulatory Evidence Paper (指标驱动监管证据论文)

**Tone**: empirical, data-anchored, reform-tracking, institutionally cautious.
**Length**: 20–50 pages; abstract + introduction + indicator analysis + reform tracking + conclusions + appendix with data tables.
**Opening**: Abstract stating the indicator finding, followed by JEL codes and keywords.

**Signature features**:
- **Indicator-driven structure**: sections organized by PMR sub-indicators, not by country or by policy area — the indicator IS the organizing principle
- **"X% of the N countries surveyed" data anchoring**: every claim carries an exact denominator — "Only 30% of the 47 countries surveyed have such a regulatory framework"
- **Percentage + count dual format**: "70% (32 countries)" — percentage always paired with absolute count in parentheses
- **Reform-tracking section**: "A comparison with the results obtained in [prior year] for the same [indicator] permits to monitor how the situation has evolved"
- **Scope footnote system**: numbered notes under every table specifying denominator, representative states in federal countries, and appendix cross-references
- **"lag behind best practice" institutional-gap framing**: "the regulatory frameworks supporting transparency and accountability... lag behind best practice in many countries"
- **"room for" reform language**: "suggesting room for stronger obligations to foster the quality of policies"
- **Conclusions with policy urgency**: "As governments make greater use of [X], there is a growing risk that [Y] may undermine the intended benefits"
- **Anti-AI note**: AI defaults to narrative description of findings; this genre requires **data-first presentation** — every paragraph opens with or contains a specific data point, and the denominator is always explicit.

---

### 9.24 Development / Capacity Assessment (发展能力评估)

**Tone**: constructive, evidence-based, recommendation-dense, cooperative.
**Length**: 30–80 pages; structured by statistical domains (R&D, innovation, HE, government) with numbered recommendations.
**Opening**: Context paragraph on the country's statistical infrastructure, followed by assessment objectives.

**Signature features**:
- **Numbered recommendations (20+)**: each bolded, standalone, with "should" and qualifying conditions — "Recommendation 4. If... a combined R&D and innovation survey remains the preferred method... an appropriate hybrid sampling and estimation design should be promptly developed."
- **Frascati / Oslo Manual alignment language**: "seeks to align with latest OECD and OECD/Eurostat guidance in the Frascati and Oslo Manuals"
- **Data reliability concerns stated directly**: "which appears to indicate some potential data reliability issues in terms of expenditure and personnel data coherence"
- **"One possible source of concern" hedge**: introduces methodological worries without accusing the country of error
- **"It is unclear to the OECD team whether" diplomatic ignorance**: OECD admits it could not verify a claim, rather than asserting or denying
- **Box inserts for methodological context**: "Source: OECD analysis of ESTIO data and statistics" — analysis boxes with their own source lines
- **Outreach event description**: mission days with stakeholders described as evidence of engagement
- **Anti-AI note**: AI defaults to generic "capacity building" language; this genre requires **specific technical critique** of sampling designs, estimation methods, and data collection instruments — with concrete numbered recommendations for each.

---

### 9.25 Multi-Country RBC / Thematic Guidance Report (多国负责任商业行为指导报告)

**Tone**: evaluative, balanced (progress + gaps), policy-recommendation-oriented, cross-country comparative.
**Length**: 80–200 pages; Introduction + Country chapters (each with thematic subsections) + Conclusions.
**Opening**: Scope paragraph defining the countries and policy domains covered.

**Signature features**:
- **Country-chapter structure**: each country gets a full chapter with identical thematic subsections (human rights, labour rights, environment, anti-corruption, sustainable finance) — enabling cross-country comparison
- **"highlights the importance" / "important concern" evaluative language**: OECD evaluates significance without emotional colour
- **Legal framework inventory**: enumeration of laws, conventions, and strategies with dates — "Since 2006-2007, Mongolia has had a dedicated law on anti-corruption"
- **"Gaps include" negative-inventory pattern**: "Gaps include the absence of a requirement for a resettlement plan, consideration for persons without formal title, lack of compensation for loss of livelihood"
- **Good-practice callout boxes**: "As a good practice, Mongolia conducted a review of how EIAs are implemented" — positive examples highlighted with explicit "good practice" label
- **"It will be important that" forward-looking recommendation**: softer than "should" — used for implementation-dependent recommendations
- **Massive references section**: 100+ references mixing OECD publications, government documents, academic papers, NGO reports, and news articles
- **Anti-AI note**: AI defaults to either full praise or full critique; this genre requires **balanced country assessment** — every positive finding is followed by a remaining challenge (T1 "affirmative + but" at the chapter level). References must include government sources, not just OECD publications.

---

### 9.26 Country Philanthropy / Survey-Based Development Study (国家慈善调查发展研究)

**Tone**: empirical, survey-methodology-transparent, data-visualisation-heavy, policy-pragmatic.
**Length**: 40–80 pages; Country context + Methodology + Data analysis + Organisational findings + Conclusions.
**Opening**: Socioeconomic context paragraph establishing why the country matters.

**Signature features**:
- **Response-rate transparency**: "62 responded to the organisational survey and 30 to the financial survey... requiring caution when drawing definitive conclusions" — survey limitations stated in the main text, not buried in annexes
- **"indicative insights" qualification**: "the overall sample size is comparable to OECD studies in other emerging economies and offers valuable indicative insights"
- **Machine-learning methodology note**: "the OECD used the supervised machine learning algorithm ModernBERT... to analyse text from both the project title/description and the reported beneficiary" — explicit AI/ML methodology transparency
- **"funding is highly concentrated" distribution finding**: concentration analysis is a structural feature of philanthropy studies
- **"The data shows a complex interaction" analytical humility**: when poverty and funding do not correlate simply, OECD names the complexity (fingerprint P)
- **Survey question direct quotation**: "Answer to the question: 'Which role best describes your organisation?'" — the exact survey question is quoted
- **Network/co-financing analysis**: collaborative relationships mapped as networks, not just counted
- **Anti-AI note**: AI defaults to clean summary statistics; this genre requires **methodological transparency** — response rates, sample limitations, ML classification details, and explicit caveats about what the data can and cannot support. Every data claim must be traceable to a specific survey question or database field.

---

### 9.27 Digital Governance / Procurement Strategy (数字政府 / 采购战略指导)

**Tone**: strategic, technology-aware, user-centric, cooperation-oriented.
**Length**: 30–80 pages; Preface + Foreword + Executive Summary + numbered chapters with strategic objectives.
**Opening**: Preface by a country official establishing the digital transformation context.

**Signature features**:
- **End-to-end, user-centric framing**: "an end-to-end, user-centric approach to digital public procurement" — the full procurement lifecycle as the organizing principle, not just technology adoption
- **Data as critical enabler**: data positioned as infrastructure, not as output — "data as a critical enabler" rather than "data shows that"
- **AI technology discussion with stakeholder evidence gap**: "Irish stakeholders expressed interest in applying these technologies to public procurement but lacked the resources or guidance to do so with confidence" — OECD reports the interest-to-capability gap explicitly
- **Monitoring + directed support framework**: "allows the government to monitor GPP uptake by institutions and direct support to sectors and institutions that are lagging behind" — the government as coordinator, not just regulator
- **Healthy competition tool description**: "The tool creates healthy competition between buyers and helps them cross-reference the green technical specifications of goods and services they are planning to buy with past procurements" — tool effectiveness described through behavioural mechanisms
- **Coordinated technology deployment**: "By providing coordinated support in deploying these technologies and connecting to broader Irish and European strategies, the strategy can help all stakeholders benefit from these opportunities and avoid common pitfalls" — technology strategy framed as coordination problem
- **Green procurement cross-referencing**: tools that enable institutional learning from past procurement data
- **Cross-institutional benchmarking**: government monitoring of individual institution uptake to direct support where needed
- **Anti-AI note**: AI defaults to generic "digital transformation" language; this genre requires **specific tool descriptions** with named behavioural mechanisms (competition, cross-referencing, monitoring) and explicit evidence of stakeholder capacity gaps.

---

### 9.28 Empirical Economics Working Paper (实证经济学工作论文)

**Tone**: academic, econometrically precise, hypothesis-driven, data-intensive.
**Length**: 40–100 pages; Abstract + Introduction + Literature Review + Methodology + Results + Conclusions + References.
**Opening**: Abstract stating the research question, methodology, and key findings.

**Signature features**:
- **Task-based methodology**: "task-based evidence" — analysis organized by regulatory tasks, not by industry or by regulation type — the task IS the unit of analysis
- **Econometric specification transparency**: VAR models, impulse response functions, error bands — "Error Bands for Impulse Responses" cited as methodological reference
- **Regulatory compliance cost estimation**: "The Cost of Regulatory Compliance in the United States" — precise cost estimation with named sources (Trebbi & Zhang, 2022)
- **Productivity growth and business dynamism linkage**: regulatory costs connected to productivity and dynamism outcomes — not just compliance costs in isolation
- **Noncompete clause analysis**: labour market restrictions as a regulatory cost channel — "Noncompetes in the U.S. Labour Force" cited
- **Green vs brown occupation classification**: "The green side of productivity: An international classification of green and brown occupations" — occupational taxonomy as analytical framework
- **Methodological nuance in counting**: "Counting regulations and measuring regulatory impact: a call for nuance" — the paper explicitly critiques simplistic regulation counts
- **Dense academic bibliography**: 50+ references mixing OECD working papers, NBER papers, and peer-reviewed journals — standard academic citation format with DOIs
- **JEL codes and keywords**: standard economics paper metadata
- **Anti-AI note**: AI defaults to generic policy recommendations; this genre requires **econometric precision** — named models, specific estimation techniques, error bands, and explicit discussion of identification challenges. Every causal claim must be supported by a named estimation strategy.

---

### 9.29 Employment / Labour Market Policy Evidence Paper (就业劳动力市场政策证据论文)

**Tone**: empirical, data-rich, policy-relevant, demographically disaggregated.
**Length**: 50–120 pages; Introduction + Literature Review + Data Overview + Sociodemographic Analysis + Job Quality Analysis + Policy Implications + References.
**Opening**: Context paragraph on labour market tightness with data on vacancy rates and unemployment.

**Signature features**:
- **Dual framing of shortages**: "not only in terms of pay but also, and possibly even more, non-pay conditions" — the paper frames labour shortages through BOTH pay and non-pay dimensions (job security, working hours, flexibility, health risks), never one without the other
- **Sociodemographic disaggregation**: "the paper also uncovers the sociodemographic composition of these jobs, in particular their incidence among women, migrants, and older workers" — every finding is disaggregated by population group
- **Measurement caveat upfront**: "In a context of measurement issues associated with the use of job vacancy data, this paper provides a cautious assessment" — data limitations stated before any findings
- **Country examples as policy evidence**: "[Country] offers a relevant example of [policy action]: [specific detail with date and data]" — every recommendation backed by a specific country example with implementation details
- **"A whole-of-society approach" multi-level governance frame**: "involving all levels of government across policy domains ranging from [X] to [Y]" — policy solutions framed as requiring coordination across government levels
- **"It may then come at little surprise to observe" understated causal link**: finding presented as the logical consequence of the evidence already laid out
- **"This does not seem to have taken place on a broad scale" understated negative**: OECD names what HASN'T happened without dramatizing the gap
- **"to good extent undervalued" restrained analytical judgment**: value judgment delivered without emotional colour
- **"Zooming again on [X]" informal analytical transition**: specific focus re-engaged with a clear but informal signal
- **Box inserts for methodology deep-dives**: "Box 1 offers an overview of such patterns" — boxes used for supply-demand analysis, not just examples
- **Anti-AI note**: AI defaults to generic "workforce challenges" language; this genre requires **disaggregated data** — every claim must be broken down by gender, migration status, age group, skill level, and industry. Country policy examples must include specific dates, programme names, and implementation details.

---

### 9.30 Country Trust / Governance Perception Study (国家信任治理感知研究)

**Tone**: evaluative, survey-data-driven, balanced (strengths + gaps), institutionally constructive.
**Length**: 80–200 pages; Foreword + Executive Summary + Assessment & Recommendations + Country Context + Trust Levels + Competence Analysis + Values Analysis + Conclusions.
**Opening**: Context paragraph on the country's governance position relative to OECD peers, with key survey data.

**Signature features**:
- **Dual conceptual framing**: "Public trust plays a dual role in democratic governance, serving as both an essential input and a crucial indicator" — trust framed as both cause and effect, never one-dimensional
- **"Areas of opportunity" structured recommendations**: findings paired with "Areas of opportunity" (never "weaknesses" or "failures") — positive framing of gaps
- **Assessment-and-recommendations table**: two-column format (Main findings | Areas of opportunity) with specific, actionable bullets — the table IS the executive summary
- **"not yet common or institutionalised" gap-framing**: OECD names what a country has NOT yet done without calling it a failure
- **"rather positive compared to OECD peers" calibrated evaluation**: positive findings always contextualized against OECD average
- **"52-percentage point difference" precise gap quantification**: trust gaps measured in exact percentage points, not vague "significant disparities"
- **"correlates with trust" evidence-based causal link**: governance dimensions linked to trust using survey regression evidence, not assertion
- **Time-series trust narrative**: trust levels traced from historical peak through decline to current level, with causal attribution to specific events (COVID-19, elections, policy changes)
- **Population-group disaggregation**: trust levels broken down by gender, education, financial stress, political affiliation, Indigenous status — every finding disaggregated
- **Historical-legacies section**: colonial history, institutional reform history, and their ongoing effects on trust — "Historical legacies of colonialism continue to impact [X]'s lives"
- **References mix**: OECD surveys, Gallup World Poll, World Values Survey, national election studies, Edelman Trust Barometer, academic literature — diverse source ecosystem
- **Anti-AI note**: AI defaults to generic "governance challenges"; this genre requires **survey-data precision** — exact percentages, exact question wordings, exact OECD comparison figures, and population-group breakdowns. Every claim must be traceable to a specific survey question and wave.

---

### 9.31 Commodity Market / Structural Price Analysis Paper (大宗商品市场结构价格分析论文)

**Tone**: econometrically rigorous, hypothesis-driven, sector-specific, risk-aware.
**Length**: 40–80 pages; Abstract + Literature Review + Methodology + Results and Discussion + Conclusions + References.
**Opening**: Abstract stating the three-part analysis structure (macroeconomic, medium-term, short-term).

**Signature features**:
- **Three-part analytical structure**: the paper explicitly lays out its methodology in three sequential parts (macroeconomic approach → medium-term trade interventions → short-term event study) — each part builds on the previous
- **"The first segment adopts... The second part considers... The final section focuses on" methodology roadmap**: the results section opens by restating what each analytical segment does — the reader is never lost
- **Metal-by-metal comparison**: findings presented side-by-side for aluminium, copper, and nickel — "Aluminium and copper prices appear to be mainly driven by aggregate demand shocks... By contrast, nickel prices appear to be substantially affected by most of the shocks"
- **"This may reflect" causal explanation with "may"**: findings explained with "may reflect" + specific mechanism — "This may reflect the broad uses of both aluminium and copper across the global economy"
- **"A key distinction to note is that" analytical spotlight**: OECD highlights a critical analytical distinction for the reader
- **"In contrast to [established model/sector]" reference-frame comparison**: findings positioned against oil market models or other established benchmarks
- **Technical acronym introduction**: "cumulative abnormal returns (CAR)", "impulse response functions (IRFs)" — acronyms introduced once, then used consistently
- **Confidence band discussion**: "The blue brackets represent the 68 per cent of responses closest to the median response" — uncertainty quantified and visualized, not just mentioned
- **"Beyond the scope of this paper" scope boundary**: explicit statement of what the analysis does NOT cover — "the impact of higher commodity prices on low-carbon technologies is yet to be concretely analysed and is beyond the scope of this paper"
- **"Future research is needed to: (i)... (ii)... (iii)..." numbered future-research agenda**: conclusions include a numbered list of specific research gaps
- **Anti-AI note**: AI defaults to descriptive summary of findings; this genre requires **econometric methodology transparency** — every finding must be accompanied by the estimation technique, the identification strategy, and the confidence bands. The three-part structure must be explicit.

---

### 9.32 Regional / Subnational Thematic Policy Review (区域 / 地方主题政策评估)

**Tone**: survey-based, institutionally detailed, best-practice-sharing, multi-level-governance-aware.
**Length**: 60–200 pages; Preface + Foreword + Executive Summary + Thematic chapters + Country/City tables + Policy recommendations.
**Opening**: Definitional paragraph establishing the policy concept, followed by survey methodology and sample.

**Signature features**:
- **Survey-driven analysis with explicit sample**: "The analysis builds on the results of the OECD Survey across 64 cities and regions" — every finding carries the sample size and response source
- **Three-tier institutional mapping**: national → regional → city responsibilities enumerated with specific entity names — "At the national level, ministries of the environment... At the regional level, public environmental organisations... In surveyed cities, the environmental departments"
- **Country/city comparison tables**: massive multi-column tables mapping every country and city to their strategy status, level of advancement, and dedicated budget — the table IS the inventory
- **"Not yet, but under development" three-stage progress taxonomy**: "Advanced" / "In progress" / "Emerging" + "Not yet, but under development" — OECD uses a precise multi-stage taxonomy, never binary
- **"e.g., [City], [Country]" inline city examples**: every general claim is immediately followed by 2-4 specific city/country examples in parentheses
- **"In the case of [City], [Country]" specific-case deep-dive**: transitions from general patterns to specific case studies using "In the case of"
- **"For example, [City] has set goals to [specific action]"**: city-level policy described with exact programme names, dates, and quantitative targets
- **Sector-by-sector instrument inventory**: instruments classified by sector (building, infrastructure, consumer goods, food, etc.) with specific examples for each
- **"This presents an opportunity... but also poses a challenge" balanced framing**: every opportunity comes with an explicit challenge
- **"cost often remains the predominant consideration... highlighting a gap between policy aspirations and practical implementation"**: institutional gap explicitly named
- **Pilot/experiment language**: "Circular economy projects often begin as pilots and experiments to test ideas and quickly learn from successes and failures" — innovation framed as iterative, not one-shot
- **Anti-AI note**: AI defaults to generic "best practices"; this genre requires **exhaustive institutional mapping** — every country, every city, every entity named, with specific programme names, dates, and progress status. The inventory tables are the core deliverable, not the prose.

### 9.33 Gender Equality Policy Roadmap / Strategy Report (性别平等政策路线图)

**Genre identity**: A comprehensive policy roadmap that combines data analysis, policy recommendations, and institutional framework descriptions. Typically commissioned by a supranational body (EU, OECD) and aimed at member-state governments. Covers multiple policy domains (education, labour, health, GBV, digital/green transitions) with a life-course approach.

**Opening style**: "Achieving gender equality requires not only looking at past outcomes – it also means looking ahead at where gaps are likely to emerge." / "This report illustrates and applies the concept of [framework]..."

**Key structural features**:
- **Bullet-dominant recommendation sections**: Recommendations are dash-prefixed multi-line items, each covering a distinct policy action. Recommendations can span 3-5 lines with embedded examples in parentheses.
- **"EU Member States and OECD Member States are encouraged to act on, and the European Commission is encouraged to support progress at the EU and Member State level in:"** — the canonical recommendation-header sentence for EU/OECD co-jurisdiction documents.
- **"Going forward, the European Commission is encouraged to focus on..."** — forward-looking transition for EU-specific actions.
- **"are areas that could be strengthened or enhanced in the follow-up to [strategy name]"** — soft recommendation pointing to the next strategy cycle.
- **"In a context of [emerging priorities]"** — political-context positioning.
- **Em-dash expansions**: "including by updating legal frameworks, enhancing law enforcement and judicial capacity, ensuring digital platforms implement robust safety and reporting mechanisms, and expanding support services" — long em-dash-enclosed expansions within bullet points.
- **"is incumbent upon [actor] to seize this moment"** — rare aspirational close (acceptable in this genre as a strategy-inauguration device).
- **Feedback-loop framing**: "Gender gaps in one area have repercussions in other areas" — explicit cross-domain causal chains.
- **Policy tables**: structured as policy-goal × policy-option matrices.
- **Case studies**: country-specific examples following policy tables.
- **Anti-AI note**: This genre's heavy bullet-point structure and recommendation density are unlike any other OECD genre. AI tends to write continuous prose; this genre is **structurally discontinuous** — long bullet lists with minimal connective tissue between items.

### 9.34 Education Diagnostic Review / PISA Country Study (教育诊断评估 / PISA 国别研究)

**Genre identity**: A diagnostic review commissioned by national authorities, using PISA (or similar international assessment) data to analyse specific educational challenges. Combines quantitative trend analysis with qualitative stakeholder interviews. Structured around 2-3 diagnostic themes.

**Opening style**: "Over the last decade, [Country]'s performance in [Assessment] has revealed both progress and persistent challenges in its education system."

**Key structural features**:
- **Mixed-pattern data narrative**: "[Subject] performance has undergone visible shifts over the past two decades. Following a significant decline..., [Country] recorded its lowest [score] in [year]. A period of recovery followed..." — the rise-fall-recovery arc.
- **"Although this result remains above the OECD average of [X], it represents a reversal of prior gains"** — relative-position + absolute-loss framing.
- **Country-comparison ladder**: "In the Nordic region, Finland recorded the steepest drop (from X to Y), while Denmark and Norway also experienced declines. In this context, Sweden's modest decrease appears relatively stable by comparison."
- **"these results highlight a need to address [problem] while sustaining [strength]"** — balanced assessment close.
- **"It should also be noted that [country] received one of the highest numbers of [factor]..."** — demographic/contextual qualifier.
- **PISA table-note conventions**: "Note: Statistically significant values are indicated in bold. The OECD average is based on data from 35 member countries. The average decennial trend is the average change, per 10-year period, between the earliest available measurement in PISA and PISA 2022, calculated by a linear regression."
- **Methodology section with "Approach" and "Limitations" sub-sections**: explicit acknowledgment of PISA's cross-sectional nature, self-reported data biases, and domain coverage gaps.
- **"Strategies that could be considered to address these challenges are presented at the end of this chapter"** — within-chapter forward reference.
- **"Guided by [N] principles ([list])"** — framework-driven policy analysis.
- **Anti-AI note**: This genre's heavy use of PISA table-notes with statistical significance conventions, and its explicit "Limitations" section distinguishing association from causation, are genre-defining. AI tends to overclaim from correlational data; this genre **systematically prevents that**.

### 9.35 Revenue Statistics / Tax Data Comparative Report (税收统计 / 税收数据比较报告)

**Genre identity**: An annual or biennial data report comparing tax-to-GDP ratios, tax mixes, and tax structures across a defined group of countries (typically LAC, OECD, or a regional grouping). Extremely data-dense with extensive tables, figures, and methodological notes.

**Opening style**: "The average tax-to-GDP ratio in [region] was [X]% in [year]." / "After a strong rebound from the initial impact of [shock], economic growth has remained weak in many [region] countries."

**Key structural features**:
- **"The tax-to-GDP ratio reflects the portion of [denominator] that comes from [numerator]"** — ratio definition before data presentation.
- **"The [region] average represents the unweighted average of [N] countries included in this publication and excludes [country] due to data availability issues"** — average-scope caveat.
- **"The decrease in the tax-to-GDP ratio from [year] to [year] exceeded 1.0 p.p. in [N] countries: [list]"** — threshold-based outlier identification.
- **Country-by-country bullet-point analysis**: each bullet opens with "- [Country] recorded [change]...", followed by a 2-3 sentence explanation with specific tax category breakdowns.
- **Sub-regional comparison tables**: "In the Caribbean, revenue from [category] increased... In Central America and Mexico, [category] revenues decreased..."
- **"Several factors contribute to / may explain" multi-cause enumeration** (T61): "Several factors contribute to the low VRR in Mexico, including the scope of VAT exemptions, the application of a domestic zero rate..., as well as low compliance."
- **"The numerator (X) ... the denominator (Y)" methodological transparency** (T60): explicit definitions of ratio components.
- **"The tax-to-GDP needs to be treated with caution"** — ratio-interpretation warning.
- **StatLink 2 URLs** after every figure/table — OECD-specific data access convention.
- **Box-format methodology explanations**: "Box 1.1: The tax-to-GDP ratio" — dedicated methodology boxes.
- **Anti-AI note**: This genre's defining feature is the **exhaustive country-by-country analysis** with specific reform names, dates, and tax category breakdowns. AI tends to summarise; OECD **itemises every country that moved by more than 1.0 p.p.** The "Note:" blocks after every figure are mandatory, not optional.

### 9.36 SME Financing Scoreboard / Annual Trends Report (中小企业融资计分卡 / 年度趋势报告)

**Genre identity**: An annual data-driven report tracking SME access to finance across multiple instruments (debt, equity, asset-based finance), with country-level data, survey evidence, and policy response analysis. Published by OECD's Centre for Entrepreneurship.

**Opening style**: "The paper comes at a particularly crucial moment. In recent years businesses and especially SMEs... have faced significant challenges from [shock]."

**Key structural features**:
- **"While [positive indicator] has begun to [improve], [negative indicator] continues to [persist]"** (T58) — mixed-signal macro framing.
- **"These developments across the range of [instruments] have impacted the structure and uses of [outcome], with [consequence]"** (T57) — structural-consequence tracing.
- **"SME [metric] [verb] in [N] out of [M] countries"** — cross-country prevalence with explicit denominator.
- **"The Scoreboard median of [metric] [verb] by [N]%"** — median-based (not mean) cross-country summary.
- **Quarter-by-quarter temporal granularity**: "In Q4 2023, the rejection rates for SMEs were at their highest since Q1 2022."
- **Box-format country spotlights**: "Box 2 provides additional information on country developments..."
- **"However, [metric] remained broadly unchanged"** — the "however" pivot to stability amid decline.
- **"although [positive fact], [negative consequence]"** — concessive structure at paragraph level.
- **Government policy response section**: structured as "Government-guaranteed loans... Government participation in VC... Financing programmes..."
- **"Looking ahead"** — forward-looking section header.
- **Anti-AI note**: This genre's defining feature is the **median-based cross-country summary** (not mean, not weighted average) combined with quarter-level temporal precision. AI tends to use "average" loosely; OECD specifies "Scoreboard median" and distinguishes it from mean. The institutional investor classification in VC tables (pension funds, insurance companies, asset managers, other) is a genre-specific taxonomy.

### 9.37 Regulatory Monitoring / Indicator-Based Compliance Assessment (监管监测 / 指标合规评估)

**Genre identity**: A data-driven paper that uses quantitative indicators (typically from a cross-country database like PMR) to assess the state of regulation in a specific policy domain. Combines literature review, indicator methodology description, cross-country prevalence statistics, reform tracking, and policy recommendations. The paper's authority derives from the indicator database, not from case studies or fieldwork.

**Opening style**: "[Topic] has become an issue of growing concern..." / "A staggering X% of countries still do not..."

**Key structural features**:
- **"Only X% of the N countries surveyed have [requirement]"** (T63) — the standard prevalence formula, used repeatedly throughout.
- **"Only two countries – [Country1] and [Country2] – impose all 4 of them, and 11 countries have none"** (T64) — dual-extreme outlier enumeration.
- **Roman numeral enumeration in running text**: "i) the obligation to... ii) the obligation for... iii) the obligation to..." — not bullet points, but inline roman numerals.
- **"It must be stressed that the PMR indicators measure the 'de jure' policies, but not actual enforcement"** (fingerprint W) — de jure/enforcement caveat.
- **"These deficiencies matter now more than ever, as governments make greater use of [X]"** (T65) — urgency elevation.
- **"Hence, it is essential to prevent, identify, and address [X]"** — transitional sentence from evidence to imperative.
- **Box-format methodology explanation**: "Box 1: The PMR indicators" — dedicated methodology box at the start.
- **"For EU member states, the PMR database only considers national registries"** — scope limitation for EU-specific data.
- **Reform comparison table**: showing indicator values at two time points (e.g., 2018 vs 2024) for selected countries.
- **"A staggering X%"** — rare evaluative language for shocking statistics. OECD uses "staggering" only for truly exceptional findings.
- **Anti-AI note**: This genre's defining feature is the **roman numeral enumeration in running text** (not bullet points) and the **dual-extreme outlier framing**. AI tends to use bullet points for lists; OECD uses inline roman numerals in this genre. AI also tends to report averages; OECD names the leaders AND the laggards.

### 9.38 Scenario Planning / Futures Methodology Study (情景规划 / 未来方法论研究)

**Genre identity**: A participatory futures study that uses scenario-planning methodologies (personas, ambition loops, "What if..." statements) to co-create preferred future visions with stakeholders. Typically commissioned by a national ministry and conducted with OECD's Centre for Educational Research and Innovation (CERI) or similar body. Combines literature review, methodology description, stakeholder survey results, persona development, scenario construction, and OECD cross-country analysis.

**Opening style**: "What if you had the opportunity to [desirable outcome]?" / "The concept of a profession evolves over time."

**Key structural features**:
- **Preface by national official + Foreword by OECD director** (dual preface): the national official's Preface is personal and policy-oriented; the OECD Foreword is institutional and research-oriented.
- **Acknowledgements section listing all contributors by name and role** — extensive, often 20+ names.
- **"What if… [desirable scenario]?"** (T66) — transformative-vision sentence, used as chapter headings and scenario titles.
- **"Meet [Name] and [Name], [career stage] [role]"** (T67) — persona-introduction sentence.
- **"The study in [Country] is the third in a series of three"** — series positioning.
- **"Of course, this study in no way aims to be representative or comprehensive"** — explicit scope limitation.
- **"It draws on the work of a group of willing professionals with a stake in [domain]"** — participant-sampling caveat.
- **Persona-based stress testing**: "How would the teacher personas react to this scenario?" — each scenario ends with persona validation.
- **Ambition loops**: structured as "[Actor] [action statement]" — e.g., "Teachers protect and promote a healthy working environment."
- **"Spotlight focus"** — mid-chapter textboxes with deeper dives.
- **Stakeholder survey with percentage findings**: "All respondents (100%) rated this as a high priority ambition and 73% judged this would require transformation."
- **Three-tier action structure**: "Ideas for transformation (long-term change)" → "The first steps: building on current strengths" → "Specific actions for change."
- **Anti-AI note**: This genre is **unlike any other OECD genre**. The "What if..." headings, persona-based stress testing, and ambition-loop structure are genre-defining. AI defaults to analytical prose; this genre is **participatory, narrative-driven, and co-creative**. The Preface by a national official with personal voice is a mandatory structural element.

### 9.39 Disaster Risk / Climate Vulnerability Assessment (灾害风险 / 气候脆弱性评估)

**Genre identity**: A Working Paper (with JEL codes) that assesses natural hazard risks for a specific region or country pair, combining physical science descriptions, climate modelling, institutional analysis, and policy recommendations. Typically co-authored by OECD Development Centre staff and academic experts. The paper's authority derives from its integration of geophysical data, climate projections, and institutional analysis.

**Opening style**: "The [region] stretches across several [countries] and its [natural feature] provide a [resource] and way of life for millions of people."

**Key structural features**:
- **"The [region] is one of the most [superlative] and [adjective] dynamic regions of the world, and home to [N] million people"** — geographic-superlative opening.
- **Dense geographic-physical description in the introduction**: 2-3 paragraphs of pure physical geography before any policy content. This is genre-defining — the physical context IS the policy context.
- **Specific scientific measurements**: "uplifting at 14-16 mm per year," "storing over 6,000 km³ of fresh water," "8,848 m" — extreme precision for physical facts.
- **"On the one hand... on the other"** — balanced geological/process framing.
- **"By contrast"** — transition between geographic sub-regions.
- **Multi-hazard cascade chains** (AQ): "Increased glacial melting enhances river flood risk... Moreover, increased melting adds more water to glacial lakes, elevating the risk of GLOFs."
- **Specific disaster event citations**: "The 2014 Sunkoshi River was blocked by landslides, killing 156 people, damaging the Kathmandu-Lhasa Arniko highway" — exact casualty counts, infrastructure names, dates.
- **Compound hazard framing**: "Major earthquakes need to be considered in compound hazard risk assessments."
- **"In the short term... In the long term"** (T51) — temporal horizon explicit comparison.
- **Data tables with return periods**: "Annual exceedance probability | Return period (years) | % Population exposed" — probability-based risk tables.
- **"It had been speculated that [X], but this has been largely discounted"** — correcting prior scientific understanding.
- **Policy section structured by country**: "4.1 The case of Nepal" → "4.2 The case of Bhutan" — parallel country-by-country policy analysis.
- **Anti-AI note**: This genre's defining feature is the **2-3 paragraphs of pure physical geography in the introduction** before any policy content. AI tends to rush to policy; OECD **establishes the physical context first** because in disaster-risk genres, the geography IS the policy. The extreme scientific precision (mm/year, km³, m elevation) is a genre signature that AI rarely replicates.

### 9.40 AI Skills Demand / Labour Market Technology Analysis (AI 技能需求 / 劳动力市场技术分析)

**Genre identity**: An empirical Working Paper that uses online job postings (OJP) data to analyse technology-related skills demand across occupations, industries, and time periods. Combines methodology description, trend analysis, occupational decomposition, skills co-occurrence networks, and policy recommendations. Typically co-authored with national ministry support and validated through expert workshops.

**Opening style**: "[Technology] is profoundly reshaping the world and the future of work." / "This paper provides a comprehensive analysis of the demand for [skills] in [country], drawing from a dataset of over [N] million [data source]."

**Key structural features**:
- **"The data suggests that, while [positive trend], [negative factor] has slowed down its pace"** — the "while X, Y" mixed-signal opening.
- **"Despite this deceleration, [metric] is still expected to grow rapidly"** — forward-looking qualifier after negative data.
- **"Some [N]% of the demand for [talent]... is for [occupation]"** — concentration-statistic sentence.
- **"Despite an overall growing trend, demand remains relatively small within individual occupations"** — the "despite growth, still small" qualification.
- **"The decrease in demand may be surprising at first glance, given [headline]"** (T68) — counterintuitive finding introduction.
- **"It is important to note that this is not to say that [misinterpretation]"** — preemptive clarification against misreading.
- **Methodology comparison section**: explicitly listing and comparing 3-4 alternative approaches (data-driven, skill-list, semantic, supervised ML) before justifying the chosen one.
- **"However, some caveats apply when using [data source]"** — explicit data-limitation caveat before results.
- **"Annex [X] shows that, on average, [data source] represent [N]% of the total [official statistic]"** — representativeness validation.
- **"Figure [N] shows that the slowdown is driven by [factor A] and that it is shared with other countries"** — cross-country validation of national trend.
- **"Three reasons relate to [factor 1], [factor 2], and [factor 3]"** — numbered expert-reasoned explanations.
- **Skills co-occurrence network analysis**: "An analysis of skills co-occurrence shows that 'communication' is strongly linked to core technical skills."
- **Bullet-point policy pathways**: "The findings and exchanges with AI experts consulted during a workshop suggest the following pathways..."
- **JEL codes and keywords** in the abstract.
- **Anti-AI note**: This genre's defining feature is the **explicit methodology comparison section** and the **"some caveats apply" data-limitation disclaimer**. AI tends to present methodology as settled; OECD **shows the reader the menu of alternatives and justifies the choice**. The cross-country validation of national trends ("shared with other countries") is a genre-specific credibility device.

### 9.41 Government Cash / Liquidity Management Practice Review (政府现金 / 流动性管理实践评估)

**Genre identity**: A practice-review report produced by an OECD Working Party or Ad Hoc Group, surveying institutional arrangements across 20+ countries. Combines contextual analysis, institutional taxonomy, comparative tables, case studies, and glossary. The report's authority derives from its multi-country expert group composition and the precision of its institutional taxonomy.

**Opening style**: "The core aim of [activity] is consistent across countries — [shared objective] — but practices differ significantly."

**Key structural features**:
- **"There is no single optimal model for [X]. Best practices depend on the local context"** (AP) — anti-prescriptive disclaimer.
- **"Despite differences, common practices typically include: 1. ... 2. ... 3. ..."** — numbered common-practices list after divergence acknowledgment.
- **"While [well-known topic] is widely discussed, [paper's topic] is less discussed, less visible and varies more"** (AO) — visibility-asymmetry logic.
- **"It does not attempt to prescribe a uniform set of policies; rather, it serves as a valuable reference"** — anti-prescriptive positioning.
- **"Countries diverge on the basic definitions such as [X], [Y] and [Z]"** — definitional-divergence framing.
- **"The relationship between [X] and [Y] is the most critical factor shaping [Z]"** — factor-priority ranking.
- **Country-comparison tables with institutional taxonomy**: "Dedicated team/unit at the Treasury | Dedicated team/unit at the DMO | Non-dedicated team/unit" — precise institutional classification.
- **"Best practice will necessarily entail differing combinations of these depending on the local context"** — context-dependent best-practice caveat.
- **Glossary section with agreed definitions** — not a footnote, but a full glossary chapter.
- **Foreword by dual directors** (national + OECD) — e.g., "Carmine Di Noia, Director for Financial and Enterprise Affairs, OECD" + "Thomas Anthony Linehan, Deputy Director, Funding and Debt Management, NTMA, Ireland."
- **Case study annexes**: "Annex 3.A. Portugal case study: the impact of being in an IMF-EU programme on cash management."
- **Staff-size data**: "Sweden 11 | Germany 10 | Portugal 6 | Netherlands 6" — precise headcount comparison.
- **Anti-AI note**: This genre's defining feature is the **explicit anti-prescriptive positioning** — "does not attempt to prescribe," "no single optimal model," "best practice will necessarily entail differing combinations." AI defaults to prescriptive recommendations; this genre **systematically avoids them**. The dual Foreword (national + OECD) and the glossary chapter are structural signatures.

### 9.42 Behavioural Science in Policy / Nudge Evidence Review (行为科学在政策中的应用 / 助推证据评估)

**Genre identity**: A policy report that applies behavioural science insights (nudge theory, cognitive biases, choice architecture) to a specific policy domain. Combines literature review, experimental evidence, institutional case studies, and implementation guidelines. The report's authority derives from its integration of academic behavioural research with OECD policy expertise.

**Opening style**: "Behavioural insights have become an increasingly important tool for policy makers..." / "This paper examines how [behavioural concept] can be applied to [policy domain]."

**Key structural features**:
- **"Behavioural insights" as a term of art** — never "behavioural science" alone in policy contexts.
- **"Choice architecture" / "nudge" / "default options"** — specific behavioural-economics vocabulary.
- **Experimental evidence citation**: "A randomised controlled trial found that..." / "In a field experiment..."
- **"While [intervention] showed promising results in [context], its effectiveness may vary across [factors]"** — context-dependency caveat for experimental findings.
- **"This highlights the importance of [factor] in determining the effectiveness of [intervention]"** — generalisation from specific experiments.
- **Implementation guidance**: structured as "Step 1: Identify the behavioural problem" → "Step 2: Design the intervention" → "Step 3: Test and evaluate."
- **Anti-AI note**: This genre requires **specific experimental citations** (RCTs, field experiments, A/B tests) rather than general claims about behavioural science. AI tends to make generic claims about "nudges"; OECD **cites specific experiments with specific findings in specific contexts**. The implementation guidance is structured as a step-by-step process, not as abstract principles.

---

### 9.21 Quick genre-matching guide

| Genre | Opening style | Paragraph length | Recommendation format | Tone | Citations |
|-------|---------------|------------------|----------------------|------|-----------|
| Economic Survey chapter | "[X] is set to / has [past part]" | 150–300 words | Interleaved, "should" + named subject | Analytical, dry | Very dense |
| Executive summary | Gerund subtitle + quantified state | 60–120 words | At end of each thematic block | Conclusive | None / few |
| Country profile (GaaG, Cancer) | Abstract concept → "In [country], …%" | 50–150 words | Often absent | Descriptive | Light |
| Development cooperation profile | "In [year], [country] [verb] [amount]" | 30–80 words | Absent (pure data) | Data-only | Light |
| Peer-review evaluation | "The lead examiners commend / note / observe" | 200–500 words | Numbered, "Argentina should" | Procedural-evaluative | Dense |
| Policy brief / Primer | "Key messages" bullets / Question heads | 80–200 words | Bullet-led | Action-oriented, accessible | None |
| Country Review (Education / Health) | State-of-play with mild warmth | 100–250 words | "Considerations", softer | Analytical with warmth | Variable |
| Working Paper | "This paper examines…" + "we find…" | 100–250 words | "These findings suggest…" | Academic, hedged | Academic citations |
| Trade Policy Brief / Industry Analysis | "Key messages" + "What's the issue?" | 80–200 words | "What does this mean for trade policy?" | Analytical-advocacy | None (refs in "Explore further") |
| Financial Market Working Paper | "This paper provides an update to…" | 150–400 words | Neutral ("without taking a position") | Technical, dense | Very dense (mixed OECD + academic) |
| Country Policy Assessment Notes | Trend + "yet" + comparison | 50–150 words | Absent (program inventory) | Descriptive-inventory | Light (data source notes) |
| Environmental / Sectoral Brief | "Key messages" + "What's the issue?" | 80–200 words | "What can policymakers do?" bullets | Evidence-based advocacy | None (refs in "Explore further") |
| Investment / Technology Brief | "Key messages" with detailed data | 80–200 words | "What can policymakers do?" bullets | Data-heavy, cautious | Methodology notes + source tables |
| Security / Justice Brief | "Key messages" + "What's the issue?" | 80–200 words | "What can policymakers do?" bullets | Threat-focused, measured | None (refs in "Explore further") |
| Empirical Research Report / Survey Study | Balanced abstract ("On the one hand...") + JEL codes | 100–250 words | "These findings suggest…" / hedged | Analytical, balanced | Academic + OECD working papers |
| Country Governance / Public Finance Study | Foreword + cooperation ack. + 4-pillar framework | 100–300 words | "From an OECD perspective..." | Descriptive-institutional | Variable |
| Annual Data / Trends Report | Foreword + database description | 80–200 words | "it will be a trend worth monitoring" | Descriptive-data, forward-looking | Data source annexes |
| Empirical Analysis / Metric Assessment | Foreword + mandate ref + labeled findings | 100–300 words | "Looking forward:" bullets | Technical-analytical | Very dense (methodology notes) |
| Operational Guidance Manual / Toolkit | Country Preface + OECD Foreword + Caveat | 150–400 words | "At a minimum, the [X] should be designed to:" | Procedural, empowering | Country examples as evidence |
| Regulatory / Legal Compliance Brief | Definitional paragraph + geographic scope | 100–300 words | Obligation enumeration ("must", "is required") | Precise, legalistic | Specific legal instruments |
| PMR / Indicator-Based Evidence Paper | Abstract + JEL codes + indicator finding | 80–200 words | "suggesting room for stronger obligations" | Empirical, reform-tracking | Very dense (data tables + footnotes) |
| Development / Capacity Assessment | Context paragraph + assessment objectives | 100–300 words | Bolded numbered "Recommendation N" with conditions | Constructive, cooperative | Academic + OECD manuals |
| Multi-Country RBC / Thematic Guidance | Scope paragraph + countries listed | 100–300 words | "It will be important that" + "Gaps include" | Balanced (progress + gaps) | Government + OECD + NGO refs |
| Country Philanthropy / Survey Study | Socioeconomic context + why country matters | 80–250 words | "indicative insights" + "complex interaction" | Empirical, pragmatic | Survey data + ML methodology notes |
| Employment / Labour Market Evidence | Context paragraph on labour market tightness | 150–300 words | "not only in terms of pay but also, and possibly even more, non-pay conditions" | Empirical, demographically disaggregated | Very dense (survey + labour force data) |
| Country Trust / Governance Perception Study | Governance position vs OECD peers + key survey data | 150–400 words | "Areas of opportunity" paired with main findings | Evaluative, balanced | OECD Trust Survey + Gallup + WVS + national studies |
| Commodity Market / Structural Price Analysis | Abstract stating three-part analysis structure | 100–250 words | "A key distinction to note is that" + numbered future research | Econometrically rigorous | Academic + OECD working papers + market data |
| Regional / Subnational Thematic Policy Review | Definitional paragraph + survey methodology + sample | 80–200 words | "Not yet, but under development" progress taxonomy | Survey-based, institutionally detailed | OECD surveys + city government documents |
| Digital Governance / Procurement Strategy | Country Preface + digital transformation context | 100–300 words | "end-to-end, user-centric" objectives + monitoring framework | Strategic, technology-aware | Tool descriptions + stakeholder evidence |
| Empirical Economics Working Paper | Abstract + research question + JEL codes | 100–250 words | "These findings suggest…" + hedged | Academic, econometric | Very dense (NBER + OECD WP + DOIs) |
| Gender Equality Policy Roadmap | "Achieving [goal] requires not only looking at past outcomes" | 100–300 words | Bullet-dominant multi-line items, "are encouraged to act on" | Aspirational, institutional | OECD/EU instruments + country evidence |
| Education Diagnostic Review / PISA Study | "[Country]'s performance has undergone visible shifts" | 150–300 words | "Strategies that could be considered" at chapter end | Diagnostic, balanced | PISA data tables + methodology notes |
| Revenue Statistics / Tax Data Report | "[Region] average [metric] was [X]% in [year]" | 80–200 words | "Several factors contribute to" + country-by-country bullets | Data-descriptive, cautionary | Very dense (StatLink 2 + methodology boxes) |
| SME Financing Scoreboard | "The paper comes at a particularly crucial moment" | 100–250 words | "Looking ahead" section + government response inventory | Data-driven, measured | OECD Scoreboard + national survey data |
| Regulatory Monitoring / Indicator-Based Compliance | "[Topic] has become an issue of growing concern" | 100–250 words | "Only X% of countries surveyed" + roman numeral lists | Data-driven urgency, reform-tracking | PMR database + survey data + methodology box |
| Scenario Planning / Futures Methodology Study | "What if you had the opportunity to [outcome]?" | 150–400 words | "What if…" scenarios + persona stress testing | Participatory, co-creative, aspirational | OECD working papers + stakeholder survey data |
| Disaster Risk / Climate Vulnerability Assessment | Geographic superlative + "home to N million people" | 200–500 words | Country-by-country parallel structure ("The case of Nepal") | Scientific-precise, cascading-risk | Very dense (academic + IPCC + OECD + national data) |
| AI Skills Demand / Labour Market Technology Analysis | "[Technology] is profoundly reshaping the world" | 100–300 words | Bullet-point policy pathways from expert workshops | Empirical, methodologically transparent | Very dense (OJP data + academic + expert workshops) |
| Government Cash / Liquidity Management Practice Review | "The core aim is consistent — but practices differ" | 150–400 words | "No single optimal model" + context-dependent options | Anti-prescriptive, institutional-taxonomic | Working Party survey + country case studies |
| Behavioural Science in Policy / Nudge Evidence Review | "Behavioural insights have become an increasingly important tool" | 100–300 words | Step-by-step implementation guidance | Evidence-based, experimental | RCT/field experiment citations + OECD policy papers |

When generating, **identify the genre first** and match its opening style, paragraph density, and recommendation format. When rewriting, infer the source genre and preserve its conventions.

---

## 10. Final Self-Check Protocol (终极自检协议)

After producing any output, run this check before delivery. **Treat your own first draft as suspect** — AI defaults will leak through unless actively scrubbed.

### Step 0: The ten-move pass (do this first; 60 seconds)

Before the detailed scans below, read the draft once against the Generative Core. This is the fast, generalising check; the eleven detailed steps that follow are the catalog-level verification of the same thing.

- **M1** Does every number carry a comparator (average / peer / prior year / target)? Any bare figure → anchor it.
- **M2** Is every generalisation followed by 2–4 named examples ("such as / including")?
- **M3** Does each analytical paragraph concede *and* qualify — and is the concession marker varied (not "but… but… but…")?
- **M4** Are recommendation modals graded to evidence and addressee, not one modal repeated?
- **M5** Is the logic carried by content sentences ("This suggests…", "On this basis…"), with zero meta-discourse?
- **M6** Are projections hedged and past facts flat?
- **M7** Are subjects concrete named actors, key terms repeated (not synonym-swapped), institutions defined by purpose?
- **M8** Is the rhythm varied (a short and a long sentence per paragraph; one rough/unsplit/imperfect-parallel spot; some flat-fact endings)? **If the prose is perfectly smooth, it will read as AI — roughen it.**
- **M9** Is all colour, meta-narration, and undata'd evaluation removed?
- **M10** Are claims sourced at the genre's D2 density, grounded in precedent, and honest about scope limits?

If M1–M10 pass and the genre dials (Step 0b) are set correctly, the draft is essentially there. Use the steps below to catch residue.

### Step 1: AI-residue scan (60 seconds)
Search the draft for these strings. If any appear, rewrite:
- `it is important to`
- `it is worth noting`
- `it should be noted`
- `plays a crucial role`
- `multifaceted`
- `holistic` / `synergistic`
- `cornerstone` / `bedrock` / `linchpin` / `springboard`
- `tapestry` / `landscape of` / `ecosystem of` (when used as filler)
- `vibrant` / `dynamic` / `thriving`
- `cutting-edge` / `state-of-the-art`
- `navigate the complexities`
- `in today's world` / `in the modern era` / `in an increasingly`
- `boasts` (as verb)
- `showcases` (as verb)
- `sheds light on`
- `paradigm shift` / `game-changer`
- `unprecedented` (unless quantified)
- `ever-evolving` / `rapidly changing`
- `at the end of the day`
- `when it comes to`
- `from X to Y to Z` (rhetorical sweep)
- `on the one hand … on the other hand`
- `not only … but also`
- `in essence` / `essentially`

### Step 2: Tonal smell test (90 seconds)
Read the draft aloud. Flag any sentence that sounds like:
- A TED talk opener
- A LinkedIn post
- A corporate press release
- A consulting deck executive summary
- A textbook trying to teach a concept
- An aspirational closing speech

Rewrite all flagged sentences in plain declarative form.

### Step 3: Concrete-subject census (60 seconds)
Underline the subject of every sentence. Count:
- **Concrete subjects** (country, institution, indicator, instrument): should be ≥ 70%
- **Abstract subjects** ("the framework", "the approach", "the dynamics"): should be ≤ 30%

If abstract subjects dominate, rewrite by promoting the agent.

### Step 4: Voice census
Count active vs passive constructions in main clauses:
- Active should be **70–80%**
- Passive should be **20–30%**, only where the agent is irrelevant

### Step 5: Rhythm scan
Mark each sentence's word count in the margin. Within any single paragraph:
- Should include **at least one short sentence (≤ 12 words)**
- Should include **at least one long sentence (35+ words)** with semicolons or "with" + absolute clause
- Should not have **three consecutive sentences of similar length** (within ± 5 words)

### Step 6: Hedging calibration
- Every projection / forecast hedged ("is set to", "is expected to", "is projected to")
- Every recommendation modal ("should", "would help", "could", "there is scope to")
- Historical facts NOT hedged ("GDP grew by 1.5% in 2024" — no "approximately" needed unless data is genuinely uncertain)
- "Notably", "particularly", "in particular" can appear multiple times per page in dense analytical prose — these are OECD signature softeners, not rationed

### Step 7: Citation and data anchoring
- Every comparative claim has a benchmark ("above the OECD average", "compared with 2022", "in real terms")
- Every projection has a horizon ("by 2030", "over the medium term")
- Every figure callout uses the canonical format: "(Figure X.Y)" or "(Table X.Y)"
- Every source citation in author-year form: "(OECD, 2024)"

### Step 8: Cohesion scan
- No paragraph opens with **meta-discourse** ("Two strands of debate…", "The first concerns…")
- No paragraph ends with a **summary sentence** ("Together, these factors demonstrate…", "In conclusion,")
- No **subjective evaluation** of data ("the data are striking / alarming / remarkable")
- Lexical chains preserved (key terms repeated, not synonym-swapped)
- Transitions embedded in content sentences ("by contrast", "however"), not as standalone signposts

### Step 9: Genre fit
- Confirm the output matches the target genre's opening pattern (see §9)
- Confirm paragraph density matches the genre
- Confirm recommendation format matches the genre

### Step 10: The dryness test
OECD prose is **drier than journalism**. If the output feels punchy, rhetorical, or persuasive — pull it back. Drop the colour. Trust the data.

### Step 11: The human-fingerprint injection (anti-AI-detector pass)
Even after Steps 1-10, the prose may still feel "robotic" to AI detectors. Run §1.9 fingerprints through the draft:

- [ ] **Citation density**: did you add `(OECD, 2024)` / `(IMF, 2024)` / `(Source, year)` every 2-3 sentences in analytical paragraphs? If citations are sparse or absent, **add them**. Use plausible institutional sources (OECD, IMF, World Bank, EC, ILO, UNDP, central banks, national statistics agencies) for the topic.
- [ ] **"such as" / "including" examples**: every general claim followed by 2-4 concrete examples?
- [ ] **"In practice" reflex**: at least one occurrence per page of "in practice", "to date", or "in particular"?
- [ ] **Heavy preposition chains**: at least one sentence with 8+ prepositional phrases left intact (not split)?
- [ ] **Latinate connectives**: did you use at least one of "albeit", "thereby", "notwithstanding", "inter alia", "to that end", "in this regard", "against this background"?
- [ ] **Imperfect parallelism**: is at least one list deliberately not in clean parallel form?
- [ ] **Repeated technical terms**: no synonym-swapping of "CLL", "RRP", country names, or institution names?
- [ ] **Mid-clause parentheticals**: at least one "Subject, however, predicate" pattern?
- [ ] **Heavy nominalisations** ("the implementation of") used in roughly half the cases where AI would default to gerunds?
- [ ] **Flat-fact paragraph endings**: at least half of paragraphs end with a fact, not a synthesising sentence?
- [ ] **Unresolved arguments**: at least one paragraph ends without explicit moral/synthesis?

If any of these are missing, the prose will read as "polished AI". Add the fingerprints. The texture matters more than perfect smoothness.

---

## 11. Closing Reminder

**OECD style is restraint.** It is the absence of:
- evaluative adjectives without data
- meta-discourse about the analysis
- rhetorical questions and aspirational closes
- metaphors and journalistic colour
- AI-default padding ("it is important to note", "plays a crucial role")
- universal-truth openings

It is the presence of:
- concrete named subjects
- present-perfect trends and "is set to" projections
- "should / would / could / there is scope to" graded recommendations
- "with" + absolute clauses extending sentences rightward
- semicolon-joined parallel mechanisms
- comma-fronted adverbials
- benchmarks anchoring every comparison
- citations every 2–3 sentences in dense analytical prose
- lexical chains that anchor, not synonyms that decorate

It is also the **deliberate roughness** that signals human authorship:
- "such as" / "including" examples unfolding constantly
- "in practice", "to date", "in particular" used freely
- "albeit", "thereby", "notwithstanding" appearing once or twice per page
- imperfect parallelism in lists
- preposition-stacked long sentences left intact
- repeated technical terms and country names without synonym-swapping
- mid-clause "however" parentheticals
- heavy nominalisations ("the implementation of") about half the time
- paragraphs ending on a flat fact, not a moral
- arguments left partially unresolved for the reader to complete

**When in doubt, write less and quantify more — but cite more, exemplify more, and resist the urge to smooth.**

---

## 12. Final Note on AI Detectors

AI detectors flag formal institutional prose as "AI-generated" because their training data is biased: their negative examples (human writing) skew toward casual, personal, narrative prose. Real OECD writing — formal, impersonal, technical — registers as "AI" to these tools regardless of who wrote it.

**The goal is not to defeat the detector.** It is to write prose indistinguishable from real OECD output. If real OECD passages also fail the detector, the detector is wrong, not the writing.

That said, §1.9 fingerprints (citation density, "such as" reflex, "in practice", Latinate connectives, imperfect parallelism, mid-clause "however", flat factual closers, heavy nominalisations, repeated technical terms) **do help** — because they push the text further from generic AI defaults toward the specific texture of human-edited institutional prose. Apply them aggressively when an AI detector flags an output as too AI-like.

**Genre diversity is the strongest anti-AI signal.** The v12 sampling round (lobbying regulation, scenario planning, disaster risk, AI skills demand, government cash management, behavioural science) confirmed that OECD's stylistic range is far wider than any single genre. The "Meet Sophia and Maximilian" persona device in Scenario Planning, the "A staggering 36% of countries still do not…" regulatory-gap framing, the 2-3 paragraphs of pure physical geography in Disaster Risk introductions, and the "What if…" transformative-vision headings are all genre-defining signals that AI never produces on its own. **Match the genre, and the anti-AI problem largely solves itself.**
