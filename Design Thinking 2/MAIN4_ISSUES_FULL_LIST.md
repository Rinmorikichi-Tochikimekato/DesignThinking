# Full Issue List — `main 4.docx` ("New Writer's Edit")

Exhaustive, non-summarized list of every problem found in `main 4.docx`, verified against `main2.docx` (the clean, submitted-quality baseline) as ground truth. Every item below was confirmed by direct text comparison, not inferred.

This is not a style-preference list — every category here is either a factual/citation error, an academic-integrity risk, a formatting regression already fixed once before, or a mechanical AI-writing signal (dashes, broken hyphenation) that is very likely part of why the Turnitin AI score did not improve.

---

## 1. Fabricated or hallucinated content (7 instances)

These are statements that do not exist in `main2` and are not supported by any cited source or original interview data.

1. **Invented regulatory detail.** "...is likely to make a direct regulation of manipulative 'dark pattern' interfaces **over the age of 12**" — this age qualifier appears nowhere in `main2`, nowhere in the cited source (Papari et al.), and describes no real provision of the EU Digital Fairness Act.
2. **Fabricated real-participant quote.** `main2`'s author-paraphrase of Ashish — *"a light, low-engagement user (20–30 minutes of YouTube a day, 'open, scroll a little, then close') whose frustration is that the feed feels unhelpful rather than manipulative"* — becomes a fully quoted first-person statement in `main 4`: *"a light user, low engagement: 20-30 minutes per day on YouTube, open, scroll somewhat then close, but I don't think it's manipulative — just unhelpful."* This invents words for a real study participant in a section whose own appendix claims real-user answers are "reported without any editing whatsoever."
3. **Nonsensical term: "Zulia" (instance 1).** "...a delicate balance between proving tiered personalisation and not overstepping the boundaries of user control (as in **the v2 version of Zulia**)" — "Zulia" does not appear anywhere else in the project. No such name, feature, or entity exists.
4. **Nonsensical term: "Zulia" (instance 2).** "...the team decided to flatten the v2 tiered personalisation **in v3 of Zulia** rather than remove user control" — same fabricated term, reused.
5. **Non-sequitur: "in Spanish."** "...based on a prompt from the contents and elements of interaction that the project team had **pre-designed in Spanish** based on the DFP selected concepts..." — nothing in this project involves Spanish language at any point; this is an unexplained, meaningless insertion.
6. **Non-sequitur: "the book was written."** "Calculating it was deemed to be 'easiest to understand', hence **the book was written**." — this sentence does not parse and refers to a "book" that does not exist; the report is not a book and nothing was "calculated."
7. **Invented product terminology: "Autopreset."** "...the very antithesis to what v3's **Autopreset modes** were set up to simplify" — the actual, correct term used consistently everywhere else (including three sentences earlier in the same paragraph) is "preset modes." "Autopreset" is invented and appears exactly once.

## 2. Broken and reverted citations (7 instances)

`main2` fixed the "P et al." rendering bug for the `4807303` reference (Aadithya P et al.) and corrected an `\&amp;` bibliography artifact. `main 4` reverts both, and introduces a new, worse variant.

1. "...reliably override stated choice preferences, due to default bias and loss aversion **(P et al., 2026, p. 2)**" — reverted broken form.
2. "...are likely to measurably reduce the number of privacy-preserving choices **(O. P et al., 2026, p. 2)**" — a new, worse variant of the same bug (adds a spurious "O." initial not present anywhere else).
3. "...which is logically required to de facto exclude dark pattern monetisation by the project's own fact of constraint **(P et al., 2026, p. 8)**" — reverted broken form.
4. "...similar to the findings from consent-banner research regarding interference with the interfaces **(P et al., 2026, p. 4; Gray et al., 2021, p. 2)**" — reverted broken form.
5. "...consistent with previous research that a measurably greater sense of autonomy and control in symmetric opt-in/opt-out designs contributes to greater levels of trust **(P et al., 2026, p. 2)**" — reverted broken form.
6. **Reference-list entry mangled beyond the original bug.** `main2`'s corrected entry reads: *"Aadithya P, Kushal Kumar M, M V Puneeth, Nithesh Gowda G, Devadatta H S, & Gurunath R. (2026)."* `main 4`'s entry reads: *"**P, A., M, K. K., Puneeth, M. V., G, N. G., S, D. H., & R, D. G.** (2026)."* — every author name has been algorithmically inverted into meaningless single-letter fragments; this is materially worse than the original unfixed bug, not merely un-fixed.
7. **Bibliography ampersand artifact reverted.** `main2` fixed `references.bib` so the Mavi (2025) title renders as "...consumer awareness & regulatory mechanism." `main 4`'s reference list shows the raw unescaped artifact: "...consumer awareness **&amp;** regulatory mechanism." (visible literally, not rendered as an ampersand).

## 3. Formatting regressions already fixed once in `main2` (3 instances)

1. **Matriculation number placeholder not filled.** Title page still reads `Matriculation Number: [TBD]`.
2. **Tutor name placeholder not filled.** Same line: `Tutor: [TBD]`.
3. **Tables and figures not relocated to an appendix.** Per the Table of Contents, "Strategic Evaluation and Reflection" doesn't start until page 15 and "Conclusion" ends around page 18–19 — core text is back to roughly 19 pages, above the 12–15 target `main2` was restructured to meet.

## 4. Rhetorical em/en-dashes used as elaboration connectors (33 instances)

Per this project's own Em-Dash Rule (zero should survive in submitted text), every instance below is a violation. `main2` has zero. Three additional dash instances in `main 4` are legitimate numeric ranges (15–20 minutes, ×2; Figures 2–4) and are **not** counted here.

1. "None of this is deception in the crudest sense **–** it works because the mechanisms are fine enough"
2. "erode behavioral autonomy, competence, and relatedness **–** the cornerstones of healthy motivation **–** is extremely difficult" (two dashes in one clause)
3. (second dash of the same clause, counted above)
4. "to create simulated qualitative interview statements **–** where participants were inaccessible"
5. "real quotes typed at the respondent's pleasure **–** as opposed to a transcript"
6. "annoyance with material bubbling up in the system on its own **—** in his case specifically antisemitic material **—** is similar to Meera's concern" (two dashes)
7. (second dash of the same clause, counted above)
8. "but I don't think it's manipulative **—** just unhelpful"
9. "this is not**—**at least not on any consistent basis**—**reported by the two" (two dashes)
10. (second dash of the same clause, counted above)
11. "a less emotional and less conflictual experience **–** where the team viewed this as an indication"
12. "moving away from their intended use**—**checking in on their friends' content**—**and to lower-value" (two dashes)
13. (second dash of the same clause, counted above)
14. "a clear statement of what it was and why **–** a 'diversity dial' rather than a clarity dial alone"
15. "Each concept was scored twice **–** a general score of social media users"
16. "a second score specifically for Priya **–** but just the latter score is shown"
17. "a hierarchy of settings that confused **–** and every one was met by a single intervention"
18. "the more you make it accessible to him to control **–** the very antithesis to what v3's Autopreset modes"
19. "inclined to avoid hard time locks on desirability **–** which the DFP matrix rated low"
20. "which the DFP matrix rated low in the first place **–** and to stick with autonomy preserving"
21. "not just a refutation of the finite-batch-feed approach **—** there is a possibility"
22. "this project was a series of short cycles**—**build, test, redesign, build, test, redesign, build, test, redesign**—**that is, it was not one extended prototyping phase" (two dashes)
23. (second dash of the same clause, counted above)
24. "several changes were implemented simultaneously **–** transitions which lack causal clarity"
25. "transitions which **–** with more time **–** the team will execute differently" (two dashes)
26. (second dash of the same clause, counted above)
27. "documented MindfulFeed's design thinking process **–** from selection of three empathize-phase interviews"
28. "based on documented usability feedback **–** not assumptions"
29. "the specific usability findings made in the table shown as overall findings **–** there has been no unstructured iteration"
30. "Whether MindfulFeed's particular mechanisms**—**batch feeds, tiered consent, etc.**—**will pass muster" (two dashes)
31. (second dash of the same clause, counted above)
32. "the different ways that two real people interacted with the same wireframe prompt**—**and data a plain transcript couldn't show"
33. "as actually entered by the participant **–** unless a paraphrase or summary is explicitly indicated"

## 5. Broken line-wrap hyphenation baked into running text (48 instances)

Every item below is a real word that has been split with a literal hyphen in the middle, confirmed by checking that the joined form appears correctly in `main2` while the hyphenated form does not appear anywhere in `main2`. This is the signature of a PDF/justified-text extraction whose line-wrap hyphens were never stripped before the paraphrase pass ran.

1. state-ment → statement
2. mov-ing → moving
3. prob-lem → problem
4. ex-plicit → explicit
5. observa-tion → observation
6. walk-through → walkthrough
7. algo-rithmic → algorithmic (1st instance)
8. repeti-tive → repetitive
9. under-stands → understands
10. over-enthusiasm → overenthusiasm
11. pro-fessional → professional
12. or-ganiser → organiser
13. engi-neer → engineer
14. up-dated → updated
15. chan-nels → channels
16. person-alised → personalised
17. recommenda-tions → recommendations
18. sug-gested → suggested
19. every-where → everywhere
20. frus-trates → frustrates (1st instance)
21. relax-ation → relaxation
22. invest-ment → investment
23. up-dates → updates
24. plat-forms → platforms
25. pri-oritises → prioritises
26. al-gorithmic → algorithmic (2nd instance)
27. un-derstood → understood
28. con-trols → controls
29. pri-oritising → prioritising
30. con-sent → consent
31. im-plicit → implicit
32. personalisa-tion → personalisation (1st instance)
33. resid-ual → residual
34. re-tention → retention
35. in-terference → interference
36. ob-struction → obstruction
37. ad-vanced → advanced
38. interfer-ence → interference (2nd instance)
39. obstruc-tion → obstruction (2nd instance)
40. mis-direction → misdirection
41. fu-ture → future
42. com-pete → compete
43. navi-gation → navigation
44. walk-throughs → walkthroughs
45. person-alisation → personalisation (2nd instance)
46. understand-able → understandable
47. gram-mar → grammar
48. re-design → redesign

## 6. Broken proper nouns and encoding corruption (6 instances)

1. **"Sak-shi"** — the participant name "Sakshi" split mid-word: *"In v1, Sak-shi commented on the 'cut off mid-thought' feeling..."*
2. **"Mind-fulFeed"** (1st instance) — the product name "MindfulFeed" split mid-word.
3. **"Mind-fulFeed"** (2nd instance) — same product-name break, second occurrence.
4. **"Dog˘ anay"** (1st instance) — author name "Doğanay" (renders correctly in `main2`) corrupted into a broken-diacritic form, in-text citation.
5. **"Dog˘ anay"** (2nd instance) — same corruption, reference-list entry.
6. **"Ilincu¸ta" / "S, unda"** — author names "Ilincuţa" and "Șunda" (both render correctly in `main2`'s reference list) corrupted into meaningless fragments with stray commas and cedilla artifacts.

## 7. First-person voice leaks (2 instances)

This project otherwise maintains strict third-person register throughout (confirmed clean in both `main.tex` and `main2.tex`). `main 4` breaks this twice in the same paragraph:

1. "Another constraint was out of **my** reach for this project: the Recommendation engine."
2. "Generating an accurate and understandable explanation, to a non-technical user **like me**, is not..."

## 8. Grammar and coherence breakdowns (representative sample — the damage is pervasive, not isolated)

1. "**The Stanford d. was selected for the project by the project team.** The contrast in learning outcomes between a school five-stage model..." — "d.School" has been split mid-term across two sentences, destroying the meaning of both.
2. "**This is no fringe, omitting the real limits of the evidence.**" — does not parse as English.
3. "**Where duh' was already set out in Section 6.2.**" — garbled beyond recovery; "duh'" is not a word and there is no Section 6.2 in the document.
4. "Neil read v1's top-of-screen element as a marker of identification as opposed to a feed control, which **he doubted v2 did**, as he was not certain about the meaning..." — the clause "which he doubted v2 did" does not connect grammatically to anything around it.
5. "The answers provided here were **free-text (i.e., unrecognized)**" — "unrecognized" is not a synonym for "free-text" or "unconstrained"; this appears to be a mistranslation/misparaphrase of the original "free-text and unconstrained."
6. "Compared to 'purposive' sampling that is recommended for depth-oriented qualitative research..." — inverts the original meaning; `main2` says the study *followed* purposive-sampling logic, not that it should be "compared to" it.
7. "the folks were hoping that the filtering step would have something to cut" — a sudden register break (casual "the folks") inconsistent with the formal register maintained everywhere else in both `main2` and the rest of `main 4` itself.

## 9. Table content corruption

The interviewee-profile table (Table 2) has its rows structurally scrambled in extraction: role, goals, burnout-trigger, and quote columns no longer line up one-to-one with each participant name in a reliable left-to-right order (compare against `main2`'s Table 2, where every row is a clean 5-column match). This affects the table for all eight participants (Sakshi, Arjun, Meera, Neil, Ashish, Omkar, Rahul, Imen) and should be visually re-checked in Word directly, since text extraction can distort table layout — but the underlying cell content itself also shows the same hyphen-break artifacts documented in Section 5 above (e.g., "person-alised recommenda-tions," "pro-fessional," "or-ganiser," "engi-neer," "chan-nels," "up-dated," "sug-gested," "frus-trates" ×2, "relax- ation," "invest-ment," "up-dates," "algo-rithmic," "over-personalisation" is fine but "al-gorithmic" ×2 recurs).

---

## Summary count

| Category | Count |
|---|---|
| Fabricated/hallucinated content | 7 |
| Broken/reverted citations | 7 |
| Formatting regressions | 3 |
| Rhetorical em/en-dashes | 33 |
| Broken line-wrap hyphenation | 48 |
| Broken proper nouns/encoding | 6 |
| First-person voice leaks | 2 |
| Grammar/coherence breakdowns (sampled, not exhaustive — damage is pervasive) | 7+ |
| **Total individually verified defects** | **113+** |

This is not a document that can be lightly edited back to submission quality — the fabricated quote (Section 1, item 2) and the invented regulatory claim (Section 1, item 1) are integrity risks independent of the mechanical damage, and the mechanical damage (dashes, broken hyphenation, broken proper nouns) is extensive enough that a targeted fix would touch nearly every paragraph.
