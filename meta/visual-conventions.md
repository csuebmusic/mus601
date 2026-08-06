# visual conventions

The house style for student-facing pages and interactive analytical tools across mus601 and mus602. Each repo carries its own copy of `assets/style.css` and its own fonts, so it stands alone. The two copies stay identical: edit here, copy across.

## the look

White-ish, minimalist, analytical. A near-white ground, high-contrast ink, one functional accent used for selection, emphasis, and links. Hairlines rather than boxes. Nothing rounded, nothing shadowed, no gradients.

## color

Addressed through named variables. No hardcoded hex in component CSS or in inline SVG.

| variable | value | use |
|---|---|---|
| `--bg` | `#fafaf8` | page ground |
| `--bg-alt` | `#f0f0ec` | panels, citation examples, quiet fills |
| `--ink` | `#17181b` | body text, rules that carry structure |
| `--ink-soft` | `#5d6067` | labels, secondary text, list markers |
| `--accent` | `#1d5c56` | links, selection, emphasis, paper-due markers |
| `--accent-soft` | `#dcebe8` | selected fills, link underlines at rest |
| `--rule` | `#dcdcd5` | hairlines between sections |

Domain families for the tools, so a matrix or a pitch-class row is themed from the same place:

| variable | value | use |
|---|---|---|
| `--pitch-bg`, `--pitch-ink` | `#f0f0ec`, `#17181b` | pitch-class chip at rest |
| `--pitch-bg-sel`, `--pitch-ink-sel` | `#1d5c56`, `#fafaf8` | pitch-class chip selected |
| `--interval-bg`, `--interval-ink` | `#e6ebef`, `#2b3a45` | interval labels and vectors |
| `--cell-bg`, `--cell-bg-sel`, `--cell-rule` | `#fafaf8`, `#dcebe8`, `#dcdcd5` | matrix cells |

## type

IBM Plex Sans for prose, IBM Plex Mono for analytical data that carries meaning: pitch-class names, set-class labels, interval vectors, matrix cells, week markers, table headers, and small labels. Mono marks data rather than decorating; prose never sets in it.

Five faces, self-hosted in `assets/fonts/` as woff2 so pages render with no network call: Sans Regular, Sans Italic, Sans SemiBold, Mono Regular, Mono Medium. Reach them through `--sans` and `--mono` rather than by family name. Titles of works and journals set in Sans Italic, which is why that face ships.

Body sets at 1.62 line height on a measure of about 34rem. Headings are lowercase and semibold, separated by a hairline rather than by size alone. Numbers in tables use `font-variant-numeric: tabular-nums`.

## pages

Student-facing material is HTML on the shared stylesheet. Markdown in this repo is for the instructor.

Each page is self-contained and browser-only: no build step, no framework, no external runtime dependency, no CDN. SVG is written inline so the variables resolve. Scripts, where a tool needs them, are inline in the page.

The layout is one column on a left-hand gutter, with the gutter carrying week markers on the schedule and collapsing to zero below 46rem. A page opens with a masthead (mono eyebrow, title, italic standfirst) and closes with a mono back link to the index.

## cache

Pages link the stylesheet with a version query, `assets/style.css?v=N`. Bump N in every page whenever `style.css` changes, or browsers keep serving the old sheet and the change looks like it never landed.

## the quality floor

Responsive to mobile, visible keyboard focus on every interactive element, `prefers-reduced-motion` respected, and a print stylesheet that drops navigation and page furniture. Contrast meets WCAG AA at every text size in the palette above.
