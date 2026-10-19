# MUS 601: conventions

## the course

MUS 601, Birth and Death of Tonality, is a graduate research-and-analysis seminar in the M.A. in Music, taught in the fall. The course's facts are in `syllabus.html`.

The seminar teaches students to become scholars of a repertoire: formulating research questions, evaluating sources critically, using the bibliographic tools of the field, writing scholarly analysis with correct citation, and connecting analysis to historical and cultural context.

It covers the Renaissance to the Romantic: the change from modal practice to functional harmony, the consolidation of common-practice tonality, and its chromatic saturation and dissolution across the nineteenth century. The vocabulary is figured bass, Roman-numeral and functional analysis, counterpoint, form, modulation and chromatic harmony, and Schenkerian reduction where a passage calls for it. The method is comparative analysis across works and periods. The seminar's analytical framework is Burnett and Nitzberg's hexachord-system theory, with chapters 3 and 4 assigned.

## who owns what

Each body of material has one canonical home. Edit it there; everything else points to it.

- `README.md`: the course overview, public-facing. Course description, meeting time and place, instructor and office hours, the syllabus link, and a pointer to each folder. Each folder's `README.md` holds that folder's live links and what each page gives, and is public-facing.
- `syllabus.html`: the full course record and the source of truth for every course fact. Schedule, per-unit bibliographies, directed questions, outcomes, the analytical papers (what they are, the method, the standard, sources, the specifications, how they're assessed), assessment and the rubric, policies, term dates, meeting time, modality.
- `outline.md`: a one-page glance, mine. Dates, unit titles, paper due dates. Derived from the syllabus; update it whenever the syllabus changes.
- `research/source-work.html`: the source and citation handout. The research tools and how to search them, what each paper asks for in sources, and the Chicago notes-bibliography forms.
- `meta/research-and-bibliography.md`: the design behind the research work, mine. The tools with their access routes, the per-paper source plan, and the citation forms the handout uses.
- `meta/editions.md`: the edition behind each seminar score, mine.
- `meta/visual-conventions.md`: the house style.
- `meta/assessment-scheme.md`: the 0-4 grade-point scheme and the grading mechanics, reusable across courses.
- `units/unit-1.html` to `units/unit-4.html`: the per-unit pages linked from the Canvas modules. Each gives its unit's selected bibliography, weeks, works, and paper prompt with directed questions. Derived from `syllabus.html`; edit the syllabus first, then update the unit page to match.
- `lesson-plans/`: mine. `unit-N-readings.md` is the reading synthesis for that unit: what each assigned reading argues, where the readings meet the unit's repertoire, and the open items. `unit-1-modal-theory-1000-1600.md` is the dated through-line from the eleventh-century apparatus to 1600. `renaissance-baroque-galant.md` is the style comparison from c. 1550 to 1770, by strand. `unit-N-class-notes.md` is the lecture in the order of the handwritten class notes, expanded with the readings; where the class notes and a reading disagree, the reading governs. `unit-N-recap.md` is the lesson plan for that unit's paper meeting: the contextual intro and the system and form charts for the paper's works. Each is written as its unit is built.
- `tools/`: interactive analytical tools and handouts. `tools/README.md` names each tool and what it gives.
- `meta/`: planning and conventions, mine and Claude's. Markdown anywhere in the repo, including in `lesson-plans/`, is mine and Claude's, except the READMEs. The repo is public, so all of it is readable at the repo and at the Pages URL.

## source of truth

This file and `meta/visual-conventions.md` govern this repo. Read them before any work in it. They're authoritative over anything earlier in a conversation; where the two disagree, flag it. When a decision changes, update the file that holds it.

## git workflow

- Commit directly to `main`, authored as Ines Thiebaut, ines.thiebaut@csueastbay.edu.
- One logical change per commit. The message names what changed and stops.
- Push after each commit. Where the cloud workspace can't push, commit in the local clone, and I push.
- Reorganizations, mass renames, and deletions are proposed in chat and wait for my confirmation.
- Repo files aren't attached in chat. I pull locally.

## deployment

GitHub Pages builds through `.github/workflows/pages.yml`, with `.nojekyll` at the repo root. The legacy Jekyll builder fails silently and stays off.

## sources

- Texts uploaded to the Claude project are authoritative and are searched first for conceptual and pedagogical questions.
- Where no uploaded source covers a topic, the gap is flagged, with an offer to draft a handout or find scholarship, in place of an answer from general knowledge.
- Bibliographic details are checked against the source itself.

## style

Style, register, and feedback for everything in this repo follow the "how I want you to communicate" section of my Claude profile preferences.

## paper feedback

Whether a paper meets the specifications is my call, and the feedback doesn't judge it.

Feedback on each student's paper is one Claude Docs doc, titled "Paper N feedback, First Last." Under the title are the date, my name, and one line naming the paper and its works. The feedback is written in three passes, each its own lowercase section, and printed.

### pass 1: references

The section is headed "references." It covers citation placement, note form, and the bibliography. It leaves out the specifications, what each secondary source is used for, and where an edition was found.

- Overcitation, measured against "the music itself" in `meta/research-and-bibliography.md`: the count and one example from the paper.
- Note form, with note numbers: first notes set as bibliography entries, short forms, title styling, volume and issue, empty or stray notes.
- One of the student's own sources as a model, in three forms: first note, short note, bibliography entry.
- The bibliography, corrected in full and alphabetized. An item only the source can supply is left as a bracketed blank, named in one sentence above the list.

### pass 2: content

The section is headed "content." It replies to the paper's analysis, work by work, in the paper's order.

- Each paragraph states the student's claim in the student's own terms, gives what the score has, and says how that changes the student's reading.
- Corrections follow the system and cadence charts in the unit's recap in `lesson-plans/`.
- Where the chart has nothing on a passage, or the difference is a bar, nothing is flagged.

### pass 3: comparison

The section is headed "comparison." It replies to the paper's comparison of the works.

- Each comparison claim is tested against the scores and the paper's own analysis: a claim without evidence gets the passages that would supply it, by measure; a claim the corrected readings change gets the corrected comparison; a comparison that measures the works on different terms gets one shared measure from the paper's analysis.
- Where the paper has no closing comparison, the section names, from the paper's own analysis, the terms one could use.
