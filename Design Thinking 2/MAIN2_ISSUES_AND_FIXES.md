# Issues Found and Fixed in `main 2.docx` → `main2.tex`

This document records every defect found in the "humanized" rewrite (`main 2.docx`,
produced to lower the Turnitin AI-detection score from ~74% to a masked "under 20%")
and the fix applied, first directly in the `.docx`, then again during the `.tex`
conversion. The unedited original is preserved at
`main 2 (backup before fixes).docx`. The clean source of truth throughout was
`main.tex` (the original, ungenerated-from-scratch v1 report).

**Bottom line on Turnitin reliability:** both `TurnitinReportBefore.pdf` and
`TurnitinReportAfter.pdf` were submitted under fabricated identities — "Abid Hussain"
and "John Doe" respectively, at a university the author does not attend. Neither the
74% nor the "under 20%" score reflects a submission under the author's real account.
Treat both numbers as unverified until re-run for real.

---

## 1. Fabricated content (invented facts, entities, or citations not in the original)

These are the most serious category: text that asserts something untrue rather than
just being awkwardly worded.

| # | Location | What was fabricated | Fix |
|---|----------|---------------------|-----|
| 1 | Conclusion / Outlook | A nonsense clause referencing "Sue" and "ethicization" | Deleted entirely |
| 2 | Introduction, DFA regulatory sentence | "over the age of 12" — an invented regulatory detail with no basis in the source literature | Deleted |
| 3 | Prototype v3 rationale | Garbled sentence claiming a decision was made because "Calculating it was deemed... hence the book was written" | Restored original meaning: Ashish "selected v3 specifically because it was deemed to be 'easiest to understand'" |
| 4 | Abstract; Methodology Rationale | "d.The" — the framework name "Stanford d.School" corrupted, with "school" duplicated/dropped in the following clause | Fixed both instances to "d.School" and reflowed the surrounding sentence |
| 5 | Define phase, POV Statement | Two overlapping, redundant paragraphs saying the same thing with degraded grammar, Priya's name dropped | Collapsed into one coherent statement, Priya named explicitly |
| 6 | Prototype v2 findings | **"Powertweak"** and a fake version number **"release 0.3.3"** — an invented competing product that does not exist anywhere else in the report | Removed; restored the real citation (Ukgoda, 2024, p. 3) about navigation-depth obstruction |
| 7 | Feasibility paragraph (×2) | **"Zulia"** — a fabricated alternate product name (the actual product is MindfulFeed throughout the rest of the document) | Removed both instances |
| 8 | Real-User Testing Tool appendix | **"artikulated"** — a non-word | Replaced with "human-authored" (the term used correctly elsewhere) |
| 9 | Ideate / SCAMPER Exploration | **"Nominate, Bypass or Substitute, then Reverse"** — invented SCAMPER move names; the actual SCAMPER moves (Substitute, Combine, Adapt, Modify, Put to another use, Eliminate, Reverse) are used correctly everywhere else, including Table 5 in the same section | Corrected to "Substitute through Reverse" |
| 10 | Prototype v3 section | Sentence truncated mid-thought — "...part of the deal of the trade is that participants" — then jumps straight into a figure | Completed using the original meaning (the v2→v3 technical-transparency trade-off) |
| 11 | GenAI Usage Disclosure appendix, item 3 | "pre-designed **in Spanish**" — a nonsense insertion; no Spanish-language content exists anywhere in this English-language project | Removed (caught during the `.tex` conversion, not the earlier docx pass) |

## 2. Grammar and coherence breakage (not fabrications, but broken or garbled English)

| # | Location | Problem | Fix |
|---|----------|---------|-----|
| 12 | User Interview Summary | Duplicate word: "profile profile" | Removed duplicate |
| 13 | Define, Synthesis of Findings | Missing verb: "personalisation taking place" | Inserted "was" |
| 14 | Feasibility paragraph | "Three," should read "Third," in a numbered sequence | Corrected |
| 15 | Introduction | Sentence fragment: "As regulators have begun to pay attention. The EU..." | Merged into one sentence: "Regulators have begun to pay attention: the EU..." |
| 16 | Define, HMW questions | Stray "?" inside "How Might We? questions" used as a compound noun | Removed the erroneous "?" |
| 17 | Throughout (~80+ instances) | Line-wrap hyphenation artifacts baked in as literal text (e.g. "Proto-type", "em-pathy", "under-stand") | Removed the inserted hyphens, rejoining each word |
| 18 | Throughout | Mixed straight (`"`/`'`) and curly (`" " ' '`) quote marks, plus two pre-existing quote-count defects (one spurious extra quote before "cut off mid-thought"; one missing closing quote after "Nothing is sent anywhere automatically") | Normalized to consistent curly quotes in reading order; fixed both root-cause count defects |
| 19 | Introduction | "behaviouraleconomics" — missing space | Fixed to "behavioural economics" |
| 20 | Appendix B, Strategy | Said "Total of 8 questions", contradicting the same appendix's own "sixteen questions" (8 + 8) elsewhere | Corrected to state the 8-then-8 structure consistently (caught during `.tex` conversion) |
| 21 | Various (Introduction, Qualitative Approach, Empathy Map, Synthesis of Findings, Evaluation section) | Assorted garbled/run-on sentences: pronoun mismatch ("he... They're"), circular reasoning ("it works because... not really deceptive"), non-sequitur framing ("Compared to X, phase involved Y"), a coding paragraph reading "against all three trans. Not trans by trans.", a paragraph dangling on the word "Second," before an unrelated new paragraph, a misattributed quote missing its opening quotation mark, wrong pronoun "his POV statement" for Priya (she), typo "Autopreset modes" | Each rewritten for grammatical sense while preserving the paraphrase's own vocabulary where sound (see `.tex` conversion pass below for full text) |

## 3. First-person voice violations (academic register requires third person throughout)

| # | Location | Original text | Fix |
|---|----------|---------------|-----|
| 22 | Evaluation, feasibility paragraph | "to a non-technical user **like me**, is not" | "to a non-technical user is not" |
| 23 | Evaluation, feasibility paragraph | "was **out of my reach** for this project" | "fell outside the scope of this project" |
| 24 | Prototype v2 | "**we** take the feedback of v1 and add..." | "Prototype v2... responded to the v1 feedback by introducing..." |
| 25 | Evaluation | "**we** postulated that **we** were more inclined to avoid hard time locks" | "This real-user evidence also puts pressure on a design bet made back in Define..." |
| 26 | Evaluation | "the walk-throughs that **the authors** performed" | "the wireframe walkthroughs" |
| 27 | Prototype v1 | "the two or three minutes **she told me** was her 'quick check'" | "the two-to-three-minute window Sakshi described as her intended 'quick check'" (caught during `.tex` conversion) |

## 4. Structural issues caught specifically during the `.tex` conversion

| # | Issue | Fix |
|---|-------|-----|
| 28 | Two tables present in the docx (interviewee-profile table, empathy-map table) were initially omitted when first drafting `main2.tex` | Caught by an "undefined reference" compile error; both tables reinserted with the correct data, verified against a clean recompile |

---

## Verification performed on the final `main2.tex` / `main2.pdf`

- Compiles with 0 errors, 0 undefined references (pdflatex → biber → pdflatex ×2)
- 9/9 citations resolve correctly against `references.bib`
- 0 occurrences of any fabrication listed above, confirmed by text-scanning the compiled PDF
- 0 em-dashes; only expected en-dashes from LaTeX's `--` numeric-range typesetting (e.g. "45--60 minutes")
- 0 first-person violations remaining outside direct interview quotes and the legitimate "How-Might-We" term
- Straight-vs-curly quote usage matches `main.tex`'s own established convention exactly
- 102 Overfull/Underfull hbox warnings — identical to `main.tex`'s own count, confirming no typesetting regression
- Page count (~30) is in the same range as `main.pdf` (~31) — both exceed the 14–17 page target in `settings.json`, but this is a pre-existing v1 issue, not introduced by this conversion

## Known pre-existing issue, not fixed (out of scope unless requested)

- `references.bib` entry `4807303` has an author field (`Aadithya P and ...`) missing a
  comma, which makes biblatex render every citation to that source as "P et al."
  instead of the full author name. This bug is present identically in `main.tex`'s own
  compiled PDF, so it was not introduced by the rewrite and was left untouched.
