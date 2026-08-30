# visual conventions

The house style for student-facing pages and interactive analytical tools in mus601. It began as a copy of the mus312 stylesheet and has since diverged; mus312 is not kept in step with it. mus602 takes a copy of `assets/style.css` and the fonts when that course is built, and the two are kept in step from then on. Each repo stands alone.

## palette

White ground, black line, one accent. The accent marks what is live: links, hover state, active controls, and the element under discussion. Fixed reference marks stay in ink.

| variable | value | use |
|---|---|---|
| `--paper` | `#ffffff` | background |
| `--ink` | `#101010` | text, primary strokes |
| `--rule` | `#cfcfcf` | secondary strokes, dividers |
| `--muted` | `#6a6a6a` | labels, captions, secondary text |
| `--accent` | `#e2560d` | links, highlight, active state, paper-due markers |
| `--accent-wash` | `rgba(226, 86, 13, 0.10)` | fills under the accent |
| `--accent-edge` | `rgba(226, 86, 13, 0.38)` | outlines on washed fills |
| `--accent-2` | `#1f5fa8` | a second strand, where two things move at once and must be told apart |

Colors are addressed through these variables. Component CSS and inline SVG use no hex values.

## type

| variable | family | use |
|---|---|---|
| `--font-body` | IBM Plex Sans, 400, 400 italic, 600 | prose, headings |
| `--font-data` | IBM Plex Mono, 400 and 500 | dates, week markers, table labels, eyebrows, and analytical data: pitch-class names, set-class labels, interval vectors, matrix cells |

Both are self-hosted woff2 in `assets/fonts/`, under the SIL Open Font License. Sans Italic carries titles of works and journals. Mono marks data; prose never sets in it.

Body sets at 1rem on a 1.55 line height. Prose runs to a 34rem measure and takes `.full` to run the width of the column. Tables, panels, and figures are full width.

Headings are lowercase and set in the body face at 600. An `h2` opens its section under a hairline rule. The stylesheet lowercases them, so a proper noun that must keep its capital takes `<span class="caps">`.

## layout

One centered column, `.wrap` at 78rem, inside `body` padding. A page opens with a mono eyebrow, an `h1` carrying `id="top"`, and a `.lede full` paragraph, and closes with a `<footer>` carrying the font credit. `.lede` is a semantic hook and carries no rule; `.full` does the work.

Spacing is `--step`, 0.5rem. Two units between paragraphs, three from a heading to its content, four between blocks, six between sections.

Tables carry their row labels as `th` in `tbody`. Numeric cells take `.num`. Table variants: `.papers`, `.rubric`, `.grades`.

The schedule sets units as `.unit` (mono label, then an `h3`) and weeks as `.week` (a `.marker` line in Mono Medium at full ink, then an `h4`). A week carrying a paper due takes `.week.due`, which marks it in the accent. A break between weeks takes `.recess`. Readings sit in `ul.readings`. Citation specimens sit in `.cite`, a boxed list of hanging-indent entries under mono labels. Quoted specimens sit in `blockquote`, washed in the accent. Small print takes `.note`.

The contents list at the head of a long page is `ul.toc`, two columns above 62rem and one below. Every `h2` takes an id and appears in it.

## pages

Student-facing material is HTML on the shared stylesheet. Markdown in this repo is for the instructor.

Every link that leaves the page opens in a new tab, with `target="_blank"` and `rel="noopener"`. In-page anchors and `mailto:` links take neither.

Each page is self-contained and browser-only: no build step, no framework, no external runtime dependency, no CDN. SVG is written inline so the variables resolve. Scripts, where a tool needs them, are inline in the page.

Pages are linked individually from Canvas. There is no landing page and no inter-page navigation beyond the links inside the prose.

Interactive tools live in `tools/`.

## cache

Pages link the stylesheet as `assets/style.css?v=N`. Bump N in every page whenever `style.css` changes.

## the quality floor

Responsive to mobile, visible keyboard focus on every interactive element, `prefers-reduced-motion` respected, and a print stylesheet that clears the body padding and sets links in ink. Ink and muted text meet WCAG AA on the paper ground. The accent reaches 3.8:1, which meets AA for large text and for non-text marks; links carry an underline so color is never the only cue.
