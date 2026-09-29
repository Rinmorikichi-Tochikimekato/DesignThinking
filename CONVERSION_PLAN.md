# MindfulFeed Project Report — Conversion Plan (Base Document)

> **Note (updated):** The base document is now `Design Thinking 2/main.tex`, not `Design thinking/main.tex` (Draft 1). Draft 2 was restructured in place: literature-essay duplication removed, artifacts (interview table, empathy map, persona, POV/HMW, SCAMPER, DFP, feedback table) merged into a single pass through the five d.School phases, TikZ wireframes added for v1/v2/v3, formatting skeleton (A4, 2cm margins, Arial, Title Page, Roman/Arabic numbering, real List of Figures/Tables/Abbreviations) applied, and GenAI disclosure rewritten to be specific. Compiles clean (pdflatex+biber+pdflatex+pdflatex), 17 pages total, ~3,365 words core prose. Re-graded — see grading history below.

**Course:** DLMBPDDT02 – Design Thinking (IU International University of Applied Sciences)
**Task:** Task 2 — Stanford d.School approach (Empathize, Define, Ideate, Prototype, Test)
**Product:** MindfulFeed — a pro-social, non-addictive social media app

**Current grade (as graded 2026-09-06):** F (28–35%)
**Target grade:** A

**Core disqualifier being fixed:** *"If it looks like a research essay or a case study analysis, the project report will fail."* The current `main.tex` is a citation-heavy literature synthesis about dark patterns, governance frameworks, and other researchers' studies — it never presents MindfulFeed's own primary evidence in the required artifact form (tables, personas, wireframes, test logs).

---

## Source documents (read once, referenced from here on)

- `Design thinking resources/Description.pdf` — project report requirements & structure, GenAI usage rules
- `Design thinking resources/Guideline for Avoiding Plagiarism (3).pdf` — plagiarism types, Turnitin process, citation checklist
- `Design thinking resources/Guidelines Project Report.pdf` — official structure (Intro/Main Body/Conclusion %), formal formatting table (A4, margins, fonts, page numbering), evaluation weighting table
- `Design thinking resources/Task_Project Report_DLMBPDDT02 (1).pdf` — Task 2 (d.School) background & task text, desirability/feasibility/profitability framing
- `settings.json` — original generation master prompt; contains the exact required content specs for each phase (3 named user profiles: Alex/Elena/Marcus; persona Maya Lin; 5 DFP concepts; 3 prototype versions; feedback table) — **treat this as the canonical content spec for what to build**, not as something to cite

## Evaluation weighting to optimize against

| Criterion | Weight |
|---|---|
| Quality (depth, coherence, reflection, appropriate theory use) | 25% |
| Process (coherence & fidelity to d.School phases) | 25% |
| Transfer (theory → practice) | 15% |
| Creativity (originality in framing/ideation/iteration) | 15% |
| Documentation (academic style, formal criteria, spelling) | 10% |
| Resources (selection/efficient use of DT tools) | 10% |

---

## Phase 0 — Document skeleton (formatting compliance)

- [ ] Geometry → A4, 2cm margins all sides (replace `letterpaper` + 3cm sides)
- [ ] Force Arial via `\usepackage{helvet}` + `\renewcommand{\familydefault}{\sfdefault}` (pdfLaTeX) — or switch to lualatex + `fontspec` if a true Arial font file is available
- [ ] Add proper Title Page: title, "Project Report", course name/code, course of study, date, author name, matriculation number, tutor's name
- [ ] Add Table of Contents, List of Figures, List of Tables, List of Abbreviations — numbered in Roman numerals (I, II, III…)
- [ ] Restart Arabic numbering (1, 2, 3…) at the Introduction, continue through Appendix
- [ ] Verify heading levels stay ≤ 3 (1. / 1.1 / 1.1.1) after restructuring
- [ ] Add an Appendix section at the very end for GenAI disclosure + raw artifact backups

## Phase 1 — Rewrite Introduction (~1.5–2 pages, 10–15%)

- [ ] 1.1 Context & Motivation: trim current burnout/regulatory literature to ~0.75 page, keep only the 4–5 strongest sources
- [ ] 1.2 Product Vision & Scope: standalone paragraph defining MindfulFeed's boundaries (finite batching, algorithm toggles, friction nudges, freemium model)
- [ ] 1.3 Methodology Rationale: comparison table — d.School (selected) vs. IDEO Field Guide (rejected, no distinct Define phase) vs. HPI Micro-Cycle (rejected, redundant for software prototyping)
- [ ] 1.4 Preparatory Work, AI Tools & Timeline: state secondary research done; disclose GenAI use here with a pointer to the Appendix; add an ASCII 8-week timeline diagram across the 5 d.School phases

## Phase 2 — Build Empathize artifacts (replace current §4)

- [ ] User Interview Summary Table — 3 profiles:
  - Alex (Gen-Z student) — infinite scroll & auto-play; sleep procrastination & cognitive fatigue
  - Elena (remote analyst) — outrage algorithms & notification loops; attention fragmentation & workplace stress
  - Marcus (product manager) — pull-to-refresh dark patterns; frustration over lost autonomy
  - Each row: 2–3 illustrative quotes, addictive trigger, emotional impact
- [ ] Empathy Map Matrix (Says / Thinks / Does / Feels) synthesizing the three interviews, as an actual table
- [ ] Keep exactly one short paragraph of literature grounding (burnout + dark-pattern research) as rationale — cut the rest of current §4 prose
- [ ] Disclose in Appendix that interview quotes are AI-simulated qualitative personas (permitted per plagiarism guideline when cited/disclosed)

## Phase 3 — Build Define artifacts (replace current §5)

- [ ] Persona card for Maya Lin (26, UX Researcher/Hybrid Worker): demographics, psychographics, core goals, frustrations — formatted as a labeled block/table
- [ ] Explicit POV statement, single boxed/quoted sentence
- [ ] 3–4 How-Might-We questions as a numbered list, each traceable to a specific empathy-map/interview finding

## Phase 4 — Build Ideate artifacts (replace current §6)

- [ ] SCAMPER pass (7 rows) applied to the current feed model, as a table
- [ ] Desirability-Feasibility-Profitability (DFP) Selection Matrix scoring 5 concepts: Finite Batch Feeds, Intentional Friction, Algorithm Dashboard, Total Ad Prohibition, Hard Time Locks — with justification column and adopted/rejected flag

## Phase 5 — Build Prototype + Test artifacts (replace current §7–8)

- [ ] v1 Low-Fi wireframe (TikZ or placeholder image): 10-post batch feed + "content completion marker"
- [ ] v2 Mid-Fi wireframe: Pro-Social Algorithm Control Dashboard with feed-intent sliders
- [ ] v3 Hi-Fi mockup: full interactive architecture — Preset Modes (Focus/Discovery/Social), Ethical AI Compliance Indicator, subscription loop
- [ ] Feedback & Redesign Summary Table — rows: Feed Scrolling / Algorithm Adjustments / Monetization Realism; columns: v1 finding → v2 change → v3 change (stopping-prompt-too-abrupt → v2; slider-cognitive-overload → preset modes in v3)
- [ ] Trim heavy citation-grounding in these sections to one short rationale note per version, not paragraph-length synthesis

## Phase 6 — Trim & reframe remaining sections

- [ ] §9 System Architecture, §10 Evaluation: keep as reflective analysis (this is where Transfer/Quality scoring happens) but rewrite from prescriptive ("should implement…") to evidentiary past tense ("the project team implemented…", "testing confirmed…")
- [ ] Conclusion: keep structure, rewrite to reference the actual artifacts now in the report instead of abstract findings

## Phase 7 — Appendix & disclosures

- [ ] GenAI Usage Disclosure: where AI was used (simulating interview quotes/personas, drafting wireframe concepts), prompts used, short rationale — mandatory per plagiarism guideline
- [ ] Optionally include raw simulation logs / extra survey data (no page limit in appendix)

## Phase 8 — Final QA pass

- [ ] Page count check: 12–15 pages core text (excluding front matter/appendix) — trim literature-heavy sections aggressively after adding tables/figures to hit this
- [ ] Verify every in-text citation has a bib entry and vice versa
- [ ] Self-check against the 6 weighted criteria table above
- [ ] Re-run `/grade-paper` against the same Task 2 criteria before considering this done

---

## Status
All phases currently unstarted. Update checkboxes in this file as work proceeds across sessions.
