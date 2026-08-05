# MUS 601: conventions

Canonical conventions for this repo, per the project's source-of-truth rule: read this before drafting material that follows the repo's conventions, and defer to it. It grows as conventions solidify.

## source of truth: who owns what

Each body of material has one canonical home. Edit it there; everything else points to it rather than carrying a second copy.

- `syllabus.html`: the full course record. The complete schedule (weeks, units, per-unit bibliographies, directed questions), learning outcomes, assessment, policies, and course facts (term dates, meeting time, modality). The source of truth for every course fact.
- `outline.md`: a one-page glance, mine. Dates, unit titles, and paper due dates only, no bibliographies and no directed questions. Derived from the syllabus; keep it in step when the schedule changes.
- `research/analytical-papers.html`: the canonical paper handout (what the papers are, the method, what a strong paper does, format, how they are assessed). The syllabus carries a short paragraph and points here.
- `research/source-work.html`: the canonical source handout (the constant requirement, what each paper adds, the five tests of trustworthiness, the annotated entry). Repertoire, source tasks, citation types, and lenses live here and nowhere else.
- `research/chicago-notes-bibliography.html`: the citation guide. Shared with 602: author here, copy there, and keep the two identical.
- `meta/research-and-bibliography.md`: the design behind the research work, mine. Where students start, the exit list, the constant-volume design, tool sequencing, scaffolding level, and the 602 handoff.
- `meta/visual-conventions.md`: the house style. Palette, type, layout, and the quality floor for every page and tool. Shared with 602.
- `meta/assessment-scheme.md`: the 0-4 grade-point scheme and the per-course grading decisions, including 601's rounding rule. Grading mechanics live here, not in the syllabus.
- `meta/`: internal planning and conventions, mine and Claude only. The repo is public, so nothing that belongs only to us goes in a student-facing file.

## format by audience

Student-facing material is HTML on `assets/style.css`, served from GitHub Pages and linked from Canvas. Markdown is instructor-facing: the outline, the conventions, and the course design. Nothing exists in both formats, so a fact lives in one file and one format.

Markdown files state what is the case. They carry no history of superseded decisions and no justification of settled ones.

## settled decisions

- Modality: in person (on-the-ground) only. No online-synchronous option and no Zoom, in any file.
- Grade rounding: round the course average to the nearest grade point, ties broken upward. Stated for students in the syllabus with a worked example; the rule also lives in `meta/assessment-scheme.md`.
- Duplication: the schedule and the paper guidance each live in one file. Do not reintroduce a second full copy of either.
- Source volume: the authoritative edition of each work analyzed, plus two secondary sources, on every paper. The two secondary sources are the fixed quantity; the edition count follows the number of works (three, two, two, one, one). Do not let the number grow across the term.
- Source grading: inside the paper's 0-to-4 score, not a sixth component. Annotations are submitted separately and fall outside the 6-to-8-page count. The assessment table stays at five papers, 20% each.
- Tool sequencing: RILM to Paper 1, JSTOR and WorldCat to Paper 2, Grove and footnote-chasing to Paper 3, ProQuest Dissertations to Paper 4, nothing new at Paper 5. Each tool is introduced in that week's seminar meeting, folded into the lecture. No separate Canvas mini-lessons.
- Paper 5 checkpoint: the source component is the readiness gate into 602, with feedback keyed point by point to the research outcomes.
- Grade scale: the eleven grade-point anchors, one row per grade, with no percentage column. The 0-to-4 score is grade points, so a percentage of points earned is a different and incompatible number. See `meta/assessment-scheme.md`.

## still to settle

- Fall 2026 office hours, and the required-versus-recommended materials confirmation in the syllabus policies.
- The late-work reduction, stated in the syllabus as half credit (50%). On a 0-to-4 scale that reads as a percentage of points, so give the reduction in grade points instead.

## still to author

- `units/`: week-by-week seminar material, as pages.
- `tools/`: the interactive analytical tools.
