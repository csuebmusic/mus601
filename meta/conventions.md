# MUS 601: conventions

Read this before drafting anything that follows the repo's conventions, and defer to it.

## who owns what

Each body of material has one canonical home. Edit it there; everything else points to it.

- `syllabus.html`: the full course record and the source of truth for every course fact. Schedule, per-unit bibliographies, directed questions, outcomes, the analytical papers (what they are, the method, format, submission, assessment), assessment, policies, term dates, meeting time, modality.
- `outline.md`: a one-page glance, mine. Dates, unit titles, paper due dates. Derived from the syllabus; keep it in step.
- `research/source-work.html`: the source handout. The deliverables and their dates, the per-paper arc, repertoire, source tasks, citation types, trustworthiness lenses, and the annotated entry live here alone. Citation mechanics do not; they are the Chicago guide's.
- `research/chicago-notes-bibliography.html`: the citation guide. Shared with 602: author here, copy there, keep identical.
- `meta/research-and-bibliography.md`: the design behind the research work, mine.
- `meta/editions.md`: the edition behind each seminar score, mine.
- `meta/visual-conventions.md`: the house style. Shared with 602.
- `meta/assessment-scheme.md`: the 0-4 grade-point scheme and the grading mechanics.
- `meta/`: planning and conventions, mine and Claude only.

## format by audience

Student-facing material is HTML on `assets/style.css`, served from GitHub Pages and linked from Canvas. Markdown is instructor-facing. A fact lives in one file and one format.

Heading levels on a page follow the document outline with no skipped levels: on the syllabus the schedule is `h2`, units and the introductory week are `h3`, and the weeks inside a unit are `h4`.

Markdown files state what is the case. Keep out decision history, rationale for settled questions, and anything that reads as a log.

## the rules

- Modality is in person (on-the-ground), in every file.
- The course grade uses the eleven grade-point anchors, one row per grade, with no percentage column. Each 0-to-4 score is grade points.
- Round the course average to the nearest grade point, ties upward.
- Every paper takes the authoritative edition of each work analyzed plus two secondary sources. Hold that constant across the term; the edition count follows the number of works (three, two, two, one, one).
- A late paper is reduced by 2% of the paper's value per day late (0.08 grade points), any part of a day counting as a day, floored at half the paper's value, a score of 2.0. This is the standard late policy and it is what Canvas's late-policy setting applies, so the syllabus states the percentage alongside its grade-point equivalent.
- Papers 1 through 4 are handed in on paper at the start of the meeting they are due, annotations stapled behind. Paper 5 goes through Canvas, due Saturday, December 12, by the end of the day.
- Source work is scored inside the paper's 0 to 4. Annotations are submitted separately, outside the 6-to-8-page count. Assessment stays at five papers, 20% each.
- The source-finding log for Paper 2 is handed in on paper at the start of the week 8 meeting, October 6. The source swap for Paper 3 happens in the week 11 meeting, October 27, with students bringing their two picks. Neither is separately weighted.
- Every deliverable and its date appears in the syllabus schedule, in the week it falls, and in the `source-work.html` deliverables table. Nowhere else.
- `source-work.html` carries the deliverables and the per-paper arc as tables, with prose only where a table cannot hold it.
- Tools come in as RILM, then JSTOR and WorldCat, then Grove and footnote-chasing, then ProQuest, with nothing new at Paper 5. Each is introduced in that week's meeting, folded into the lecture.
- Paper 5's source component is the readiness gate into 602, with feedback keyed to the research outcomes.
- Unit 4's single meeting before Paper 5, and week 13's double duty, are as intended.
- In the Chicago guide, the note and the bibliography example inside one citation form use the same source, so the pair shows the difference in punctuation and name order.
- Student-facing pages state what is the case. Keep out sentences that justify a design decision, announce what the next sentence will do, or explain why an ordering or requirement is as it is. The schedule names works and dates; it does not argue for them.
- Every reading and score is required and carries equal weight, and all of them are provided through Canvas or library reserve. Students purchase nothing.
- The week entries name the works studied in each meeting. Editions are not listed on the syllabus; they live in `meta/editions.md`.
- The syllabus bibliography follows the Chicago style the seminar teaches: abbreviated page ranges, no initial "The" in journal titles, spaced initials, place of publication, season where the issue gives one. Christensen chapters stay nested under the volume; everything else is a full entry.

## open

- Week-by-week seminar material, as pages, in a directory added when the first unit lands.
- The interactive analytical tools, in a directory added when the first tool ships.
