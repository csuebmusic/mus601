# visual conventions

The house style for student-facing pages and interactive analytical tools in mus601. mus312 isn't updated to match it.

## palette

The palette is a white ground, black line, and one accent, and the accent marks what's live: links, hover state, active controls, and the element under discussion. Fixed reference marks stay in ink.

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

Domain families extend the palette for the tools that use them.

| variable | value | use |
|---|---|---|
| `--seg-vordersatz` | `#0b6e77` | ritornello segment: Vordersatz |
| `--seg-fortspinnung` | `#427018` | ritornello segment: Fortspinnung |
| `--seg-epilog` | `#b02e5c` | ritornello segment: Epilog |
| `--seg-pianoidee` | `#7c4dab` | ritornello segment: pianoidée |

A segment color sets the segment's label and outline; a 14 to 16 percent `color-mix` of it into `--paper` fills its box. Segment-colored text on a fill meets 4.5:1.

Colors are addressed through these variables. Component CSS and inline SVG use no hex values.

## type

| variable | family | use |
|---|---|---|
| `--font-body` | IBM Plex Sans, 400, 400 italic, 600 | prose, headings |
| `--font-data` | IBM Plex Mono, 400 and 500 | dates, week markers, table labels, eyebrows, and analytical data: pitch-class names, set-class labels, interval vectors, matrix cells |

Both are self-hosted woff2 in `assets/fonts/`, under the SIL Open Font License. Sans Italic sets titles of works and journals. Mono marks data; prose never sets in it.

Music glyphs set in Bravura, a SMuFL font subset to the glyphs in use and self-hosted as `assets/fonts/Bravura-subset.woff2`, under the SIL Open Font License. Its `@font-face` is declared in the page that uses it rather than in the stylesheet. One staff space is a quarter of the em: set `font-size` to four times the staff space in pixels. A clef glyph's reference line is on the baseline, and so is a notehead's vertical center. A page using it credits both families in the footer.

Body sets at 1rem on a 1.55 line height. Prose runs to a 34rem measure and takes `.full` to run the width of the column. Tables, panels, and figures are full width.

Headings are lowercase and set in the body face at 600. An `h2` opens its section under a hairline rule. The stylesheet lowercases them, so a proper noun that must keep its capital takes `<span class="caps">`.

## layout

The layout is one centered column, `.wrap` at 78rem, inside `body` padding. A page opens with a mono eyebrow, an `h1` with `id="top"`, and a `.lede full` paragraph, and closes with a `<footer>` giving the font credit. `.lede` is a semantic hook and takes no rule.

Spacing is `--step`, 0.5rem. Two units between paragraphs, three from a heading to its content, four between blocks, six between sections.

Table row labels are `th` in `tbody`. Numeric cells take `.num`. Table variants: `.papers`, `.rubric`, `.grades`.

The schedule sets units as `.unit` (mono label, then an `h3`) and weeks as `.week` (a `.marker` line in Mono Medium at full ink, then an `h4`). A week with a paper due takes `.week.due`, which marks it in the accent. A break between weeks takes `.recess`. Readings are in `ul.readings`. Citation specimens are in `.cite`, a boxed list of hanging-indent entries under mono labels. Quoted specimens are in `blockquote`, washed in the accent. Small print takes `.note`.

The contents list at the head of a long page is `ul.toc`, two columns above 62rem and one below. Every `h2` takes an id and appears in it.

## pages

Student-facing material is HTML on the shared stylesheet.

Every link that leaves the page opens in a new tab, with `target="_blank"` and `rel="noopener"`. In-page anchors and `mailto:` links take neither.

Each page is self-contained and browser-only: no build step, no framework, no external runtime dependency, no CDN. SVG is written inline so the variables resolve. Scripts, where a tool needs them, are inline in the page.

Pages are linked individually from Canvas. There's no landing page and no inter-page navigation beyond the links inside the prose.

## cache

Pages link the stylesheet as `assets/style.css?v=N`. Bump N in every page whenever `style.css` changes.

## minimum requirements

Every page is responsive to mobile, shows visible keyboard focus on every interactive element, respects `prefers-reduced-motion`, and has a print stylesheet that clears the body padding and sets links in ink. Ink and muted text meet WCAG AA on the paper ground. The accent reaches 3.8:1, which meets AA for large text and for non-text marks; links take an underline, and color is never the only cue.
