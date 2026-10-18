# MUS 601: conventions

## the two courses

MUS 601, Birth and Death of Tonality, runs in the fall, and MUS 602, Post-Tonality and Beyond, in the spring. Both are graduate research-and-analysis seminars in the M.A. in Music. Students take 601 then 602, and the two run as one year-long sequence: 602 picks up chronologically where 601 ends. Each course's own facts are in its syllabus.

Both seminars teach students to become scholars of a repertoire: formulating research questions, evaluating sources critically, using the bibliographic tools of the field, writing scholarly analysis with correct citation, and connecting analysis to historical and cultural context.

- 601 covers the Renaissance to the Romantic: modal practice moving toward functional harmony, the consolidation of common-practice tonality, and its chromatic saturation and dissolution across the nineteenth century. The vocabulary is figured bass, Roman-numeral and functional analysis, counterpoint, form, modulation and chromatic harmony, and Schenkerian reduction where a passage calls for it. The method is comparative analysis across works and periods. Burnett and Nitzberg's hexachord-system framework is the seminar's analytical framework, with chapters 3 and 4 assigned.
- 602 covers the turn of the century to World War II: Debussy, the Second Viennese School, Stravinsky, Bartók, and their contemporaries. The vocabulary is pitch-class set theory (set classes, interval vectors, Tn and TnI), symmetry and interval cycles, twelve-tone and serial technique, and atonal voice leading, in a theoretical framework that is still contested. My analytical lens (symmetry, interval cycles, form as process) is a through-line of the seminar.

When a tool could serve either course, ask me which repo it's for.

## who owns what

Each body of material has one canonical home. Edit it there; everything else points to it.

- `README.md`: the face of the course, public-facing. Course description, meeting time and place, instructor and office hours, the syllabus link, and a pointer to each folder. Each folder's `README.md` holds that folder's live links and what each page gives, and is public-facing.
- `syllabus.html`: the full course record and the source of truth for every course fact. Schedule, per-unit bibliographies, directed questions, outcomes, the analytical papers (what they are, the method, the standard, sources, the specifications, how they are assessed), assessment and the rubric, policies, term dates, meeting time, modality.
- `outline.md`: a one-page glance, mine. Dates, unit titles, paper due dates. Derived from the syllabus; keep it in step.
- `research/source-work.html`: the source and citation handout. The research tools and how to search them, what each paper asks for in sources, and the Chicago notes-bibliography forms. Shared with 602: author here, copy there, keep identical.
- `meta/research-and-bibliography.md`: the design behind the research work, mine. The tools with their access routes, the per-paper source plan, and the citation forms the handout draws on.
- `meta/editions.md`: the edition behind each seminar score, mine.
- `meta/visual-conventions.md`: the house style. Shared with 602 and with mus312.
- `meta/assessment-scheme.md`: the 0-4 grade-point scheme and the grading mechanics, reusable across courses.
- `units/unit-1.html` to `units/unit-4.html`: the per-unit pages linked from the Canvas modules. Each gives its unit's selected bibliography, weeks, works, and paper prompt with directed questions. Derived from `syllabus.html`; keep in step, and edit the syllabus first.
- `lesson-plans/`: mine. `unit-N-readings.md` is the reading synthesis for that unit: what each assigned reading argues, where the readings meet the unit's repertoire, and the open items. `unit-1-modal-theory-1000-1600.md` is the dated through-line from the eleventh-century apparatus to 1600. `renaissance-baroque-galant.md` is the style comparison from c. 1550 to 1770, by strand. `unit-N-class-notes.md` is the lecture in the order of the handwritten class notes, expanded with the readings; where the class notes and a reading disagree, the reading stands. `unit-N-recap.md` is the lesson plan for that unit's paper meeting: the contextual intro and the system and form charts for the paper's works. Unit 1 files exist; the others are written as the units are built.
- `tools/`: interactive analytical tools and handouts. `tools/modal-species.html` gives the four categories of mode with the species of fourth and fifth and the authentic and plagal ambitus. `tools/gamut-layers.html` lays the hexachordal, tetrachordal, and modal divisions over one pitch field (gamut) as eleventh-century scalar and modal theory. `tools/affinities.html` gives the affinities, the cofinals, and transposition. `tools/systems.html` gives the three-hexachord gamut system, `tools/twelve-modes.html` the twelve modes under both numberings. The five are numbered 1 to 5 in their titles and carry a rail listing all five. `tools/tuning.html` gives seven keyboard tunings from 1482 to 1691 on one circle of fifths, with interval and triad sizes and playback; it is unnumbered and carries no rail. `tools/ritornello.html` gives the concerto ritornello after Dreyfus and Burnett: the segments, the markedness matrix, Dreyfus's ritornello formations on a measure strip and on the hexachord, with R for a complete statement and r for an incomplete one, and the two readings of Brandenburg 2; it is unnumbered and carries no rail.
- `meta/`: planning and conventions, mine and Claude only. Markdown anywhere in the repo, including in `lesson-plans/`, is mine and Claude's, except the READMEs. The repo is public, so all of it is readable at the repo and at the Pages URL.

## source of truth

This file and `meta/visual-conventions.md` govern mus601 and mus602, and mus602's `meta/conventions.md` adds what is specific to that repo. Read them before any work in either repo. They are authoritative over anything earlier in a conversation; where the two disagree, flag it. When a decision changes, update the file that holds it.

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

Feedback on student work follows the "how I want you to communicate" section of my Claude profile preferences. Whether a paper meets the specifications is my call, and the feedback doesn't judge it.

Feedback on each student's paper is one Claude Docs doc, titled "Paper N feedback, First Last." Under the title are the date, my name, and one line naming the paper and its works. The feedback is written in three passes, each its own lowercase section, and printed.

### pass 1: references

The section is headed "references." It covers citation placement, note form, and the bibliography. It leaves out the specifications, what each secondary source is used for, and where an edition was found.

- Overcitation, measured against "the music itself" in `meta/research-and-bibliography.md`: the count and one example from the paper.
- Note form, with note numbers: first notes set as bibliography entries, short forms, title styling, volume and issue, empty or stray notes.
- One of the student's own sources as a model, in three forms: first note, short note, bibliography entry.
- The bibliography, corrected in full and alphabetized. An item only the source can supply is left as a bracketed blank, named in one sentence above the list.

### pass 2: content

The section is headed "content." It replies to the paper's analysis, work by work, in the paper's order.

- Each paragraph takes the student's claim in the student's own terms, gives what the score has, and says what that does to the student's reading.
- Corrections follow the system and cadence charts in the unit's recap in `lesson-plans/`.
- Where the chart has nothing on a passage, or the difference is a bar, nothing is flagged.

### pass 3: comparison

The section is headed "comparison." It replies to the paper's comparison of the works.

- Each comparison claim is tested against the scores and the paper's own analysis: a claim without evidence gets the passages that would supply it, by measure; a claim the corrected readings change gets the corrected comparison; a comparison that measures the works on different terms gets one shared measure from the paper's analysis.
- Where the paper has no closing comparison, the section names, from the paper's own analysis, the terms one could use.
