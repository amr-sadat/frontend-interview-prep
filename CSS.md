# 🚀 CSS Interview Preparation Guide

> 🟢 Easy | 🟡 Medium | 🔴 Advanced

---

## Table of Contents

- [🟢 Q1 - What is the difference between em, rem, px, %, vw, and vh?](#-q1-what-is-the-difference-between-em-rem-px--vw-and-vh)
- [🟢 Q2 - Explain the CSS box model and `box-sizing: border-box`.](#-q2-explain-the-css-box-model-and-box-sizing-border-box)
- [🟢 Q3 - How does CSS specificity work?](#-q3-how-does-css-specificity-work)
- [🟢 Q4 - What is the difference between `position: relative`, `absolute`, `fixed`, and `sticky`?](#-q4-what-is-the-difference-between-position-relative-absolute-fixed-and-sticky)
- [🟢 Q5 - What is the difference between Flexbox and CSS Grid?](#-q5-what-is-the-difference-between-flexbox-and-css-grid)
- [🟢 Q6 - What is the difference between `display: none` and `visibility: hidden`?](#-q6-what-is-the-difference-between-display-none-and-visibility-hidden)
- [🟢 Q7 - What is the CSS cascade, and how does it differ from specificity?](#-q7-what-is-the-css-cascade-and-how-does-it-differ-from-specificity)
- [🟢 Q8 - What is the difference between inline, inline-block, and block display values?](#-q8-what-is-the-difference-between-inline-inline-block-and-block-display-values)
- [🟢 Q9 - What are pseudo-classes vs pseudo-elements? (`:hover` vs `::before`)](#-q9-what-are-pseudo-classes-vs-pseudo-elements-hover-vs-before)
- [🟢 Q10 - What is margin collapsing and how does it work?](#-q10-what-is-margin-collapsing-and-how-does-it-work)
- [🟢 Q11 - What are CSS combinators (`>`, `+`, `~`, descendant space)?](#-q11-what-are-css-combinators)
- [🟢 Q12 - What is a CSS reset / normalize.css, and why use one?](#-q12-what-is-a-css-reset--normalizecss-and-why-use-one)

- [🟡 Q13 - What is a stacking context and why does `z-index` sometimes "not work"?](#-q13-what-is-a-stacking-context-and-why-does-z-index-sometimes-not-work)
- [🟡 Q14 - What are CSS custom properties and how do they work?](#-q14-what-are-css-custom-properties-and-how-do-they-work)
- [🟡 Q15 - What is the BEM methodology?](#-q15-what-is-the-bem-methodology)
- [🟡 Q16 - How does Angular's view encapsulation work?](#-q16-how-does-angulars-view-encapsulation-work)
- [🟡 Q17 - What is the difference between CSS animations and JS animations?](#-q17-what-is-the-difference-between-css-animations-and-js-animations)
- [🟡 Q18 - How do media queries work, and what's mobile-first vs desktop-first CSS?](#-q18-how-do-media-queries-work-and-whats-mobile-first-vs-desktop-first-css)
- [🟡 Q19 - What are CSS Grid's `fr` unit, `minmax()`, and auto-fit vs auto-fill?](#-q19-what-are-css-grids-fr-unit-minmax-and-auto-fit-vs-auto-fill)
- [🟡 Q20 - What is `clamp()`, `min()`, and `max()` used for in responsive design?](#-q20-what-is-clamp-min-and-max-used-for-in-responsive-design)
- [🟡 Q21 - What's the difference between CSS transitions and CSS animations (`@keyframes`)?](#-q21-whats-the-difference-between-css-transitions-and-css-animations-keyframes)
- [🟡 Q22 - What is float and clearfix, and why is it rarely used for layout now?](#-q22-what-is-float-and-clearfix-and-why-is-it-rarely-used-for-layout-now)
- [🟡 Q23 - What are CSS logical properties (`margin-inline`, `padding-block`) vs physical ones?](#-q23-what-are-css-logical-properties-margin-inline-padding-block-vs-physical-ones)
- [🟡 Q24 - What is `aspect-ratio` and what problem does it solve?](#-q24-what-is-aspect-ratio-and-what-problem-does-it-solve)
- [🟡 Q25 - What's the difference between `overflow: hidden`, `scroll`, and `auto`?](#-q25-whats-the-difference-between-overflow-hidden-scroll-and-auto)
- [🟡 Q26 - What are CSS methodologies like BEM, OOCSS, SMACSS, and utility-first (Tailwind)? How do they compare?](#-q26-what-are-css-methodologies-like-bem-oocss-smacss-and-utility-first-tailwind-how-do-they-compare)
- [🟡 Q27 - What is `will-change` and when should (and shouldn't) you use it?](#-q27-what-is-will-change-and-when-should-and-shouldnt-you-use-it)
- [🟡 Q28 - What is `clip-path` and how does it differ from mask?](#-q28-what-is-clip-path-and-how-does-it-differ-from-mask)

- [🔴 Q29 - Explain the rendering pipeline: Layout, Paint, Composite.](#-q29-explain-the-rendering-pipeline-layout-paint-composite)
- [🔴 Q30 - What is CSS containment and how does it improve performance?](#-q30-what-is-css-containment-and-how-does-it-improve-performance)
- [🔴 Q31 - What is CSS Houdini?](#-q31-what-is-css-houdini)
- [🔴 Q32 - How do you build a design token system in Angular?](#-q32-how-do-you-build-a-design-token-system-in-angular)
- [🔴 Q33 - What are `:is()`, `:where()`, and `:has()`?](#-q33-what-are-is-where-and-has)
- [🔴 Q34 - What are CSS cascade layers (`@layer`), and what problem do they solve?](#-q34-what-are-css-cascade-layers-layer-and-what-problem-do-they-solve)
- [🔴 Q35 - What is native CSS nesting, and how does it differ from Sass nesting?](#-q35-what-is-native-css-nesting-and-how-does-it-differ-from-sass-nesting)
- [🔴 Q36 - What is CSS subgrid, and how does it differ from regular Grid?](#-q36-what-is-css-subgrid-and-how-does-it-differ-from-regular-grid)
- [🔴 Q37 - What are container queries (`@container`), and how do they differ from media queries?](#-q37-what-are-container-queries-container-and-how-do-they-differ-from-media-queries)
- [🔴 Q38 - What are the new viewport units svh/lvh/dvh, and why were they introduced (mobile browser UI issue)?](#-q38-what-are-the-new-viewport-units-svhlvhdvh-and-why-were-they-introduced-mobile-browser-ui-issue)
- [🔴 Q39 - What is scroll-snap, and how do you build a snapping carousel with pure CSS?](#-q39-what-is-scroll-snap-and-how-do-you-build-a-snapping-carousel-with-pure-css)
- [🔴 Q40 - What are `prefers-color-scheme` and `prefers-reduced-motion`, and how do you design for them?](#-q40-what-are-prefers-color-scheme-and-prefers-reduced-motion-and-how-do-you-design-for-them)
- [🔴 Q41 - What is the difference between `:focus`, `:focus-visible`, and `:focus-within`?](#-q41-what-is-the-difference-between-focus-focus-visible-and-focus-within)
- [🔴 Q42 - How does CSS specificity interact with `!important` and cascade layers together?](#-q42-how-does-css-specificity-interact-with-important-and-cascade-layers-together)
- [🔴 Q43 - What are CSS color functions like `oklch()`/`lab()`, and why are they replacing `rgb()`/`hsl()`?](#-q43-what-are-css-color-functions-like-oklchlab-and-why-are-they-replacing-rgbhsl)
- [🔴 Q44 - What is critical CSS, and how do you extract/inline it for performance?](#-q44-what-is-critical-css-and-how-do-you-extractinline-it-for-performance)
- [🔴 Q45 - What is the difference between CSS Modules, CSS-in-JS, and Shadow DOM scoping?](#-q45-what-is-the-difference-between-css-modules-css-in-js-and-shadow-dom-scoping)

---

### 🟢 Q1. What is the difference between em, rem, px, %, vw, and vh?

**Answer:**
These are the core CSS units for sizing. Each resolves against a different reference.

| Unit | Relative to | Use case |
|---|---|---|
| `px` | Fixed — 1px is a CSS pixel (a device-independent unit) | Borders, one-off exact sizes. Does **not** scale with user font-size/zoom accessibility settings |
| `em` | The computed `font-size` of the **current element** (compounds — see gotcha below) | Padding/margins sized relative to an element's own text size |
| `rem` | The `font-size` of the root element (`<html>`) | Default for text and spacing — scales with user preferences, no compounding |
| `%` | `font-size`: parent's `font-size`. `width`/`height`: parent's **content box** dimension | Flowing, parent-relative layouts |
| `vw` | 1% of viewport width | Full-width hero sections, fluid type |
| `vh` | 1% of viewport height | Full-height layouts, viewport-aligned elements |

**Gotcha 1 — `em` compounding:** `em` is relative to the computed font-size of the *current* element, not just its parent — and it compounds. If `.parent { font-size: 1.2em }` and `.child { font-size: 1.2em }` sits inside it, the child computes off the parent's already-scaled size, not the root. Nest `em` a few levels deep and sizes spiral unpredictably. This is the #1 reason `rem` is preferred for font sizing — it always resolves against `<html>`'s font-size, no matter how deep the nesting.

**Gotcha 2 — `<html>`'s em is the baseline:** `rem` is defined as relative to the root's font-size, so if that root font-size is itself set in `em` or `%`, it still resolves from the browser's default base size (usually 16px).

**Gotcha 3 — `%` behaves like `em` for font-size**: `%` for `font-size` is parent-relative (same as `em`), but `%` for `width`/`height` is relative to the parent's *content box dimension* — a different axis of "parent-relative" than font sizing.

**Gotcha 4 — `vmin`/`vmax`:** missing from the common unit list is `vmin`/`vmax` — whichever of `vw`/`vh` is smaller/larger respectively. Useful for elements that need to scale consistently regardless of orientation:

```css
.responsive-square { width: 50vmin; height: 50vmin; }
```

**Practical note on accessibility:** `rem` respects user browser zoom and font-size preferences (a common accessibility setting) while `px` does not scale with those — another reason to default to `rem` for text and spacing.

---

### 🟢 Q2. Explain the CSS box model and `box-sizing: border-box`.

**Answer:**
Every element is a rectangular box made of four concentric layers, outside to inside:

- **Margin** — transparent space pushing the box away from neighbors. Never counted into `width`/`height` by any box-sizing value.
- **Border** — the visible edge, drawn around the padding/content.
- **Padding** — space between the border and the content, inside the box.
- **Content** — the actual inner content (text, images, child elements).

**`box-sizing` changes which of these `width`/`height` include:**

| | `content-box` (default) | `border-box` |
|---|---|---|
| `width: 200px` | Content is 200px; padding + border **add on top** | Content shrinks so total (content + padding + border) = 200px |
| Net effect with `padding: 20px` | Box renders **240px+** wide | Box stays **exactly 200px** |

```css
/* content-box: 200 + 20 + 20 = 240px total */
.box { box-sizing: content-box; width: 200px; padding: 20px; }

/* border-box: still 200px total; content is 160px */
.box { box-sizing: border-box; width: 200px; padding: 20px; }
```

**Critical caveat — margin is never included in either value.** `border-box` only folds padding and border into the declared width/height; margin always adds outside the box regardless of the setting. This trips people up — "why is my 200px `border-box` element still pushing neighbors around" is almost always margin.

**Why `border-box` is the sane default:** with `content-box` (the actual CSS default), adding `padding: 20px` to a `width: 200px` box silently grows it to 240px+, breaking layouts that assumed fixed widths. The universal reset is close to industry-standard practice (used in Bootstrap, Tailwind's preflight, etc.):

```css
*, *::before, *::after { box-sizing: border-box; }
```

---

### 🟢 Q3. How does CSS specificity work?

**Answer:**
When multiple rules target the same element, the browser picks which declaration wins using specificity — a measure of how *specific* a selector is. Specificity is a 4-tuple counted from four tiers:

| Column | Counts | Examples |
|---|---|---|
| a | Inline `style` attribute | `style="color: red"` |
| b | ID selectors | `#nav` |
| c | Classes, attributes, pseudo-classes | `.item`, `[type="text"]`, `:hover`, `:first-child` |
| d | Elements, pseudo-elements | `div`, `::before`, `::after` |

**Comparison is column by column, not summed into one number.** A single ID selector `(0,1,0,0)` beats *any* number of classes: `(0,0,50,0)` still loses to `(0,1,0,0)`. Start from column `a` and move right; the first column where one value is higher wins. This is why ID selectors in CSS are generally discouraged for styling — they're nearly impossible to override without another ID or `!important`.

```css
/* (0,1,1,0) wins over (0,0,3,0) — the ID column decides first */
#nav .item:hover { color: red; }
.foo .bar .baz     { color: blue; }
```

**Pseudo-class vs pseudo-element gotcha:** `:hover` is a pseudo-class — it counts in the `c` column along with classes and attributes. `::before`/`::after` are pseudo-elements — they count in `d`, with actual elements. Easy to conflate since both use colon-ish syntax, but only pseudo-elements (`::`) join the element/tag tier.

**The cascade tiebreakers:**
- **Source order** is the tiebreaker only when specificity is *exactly* equal — the later rule in the cascade wins.
- `!important` genuinely breaks the normal cascade and should be treated as a last resort / escape hatch, not a specificity shortcut. Two `!important` rules revert to normal specificity comparison between themselves.

---

### 🟢 Q4. What is the difference between `position: relative`, `absolute`, `fixed`, and `sticky`?

**Answer:**
Four positioning modes, each relative to a different reference:

| Value | Reference | Flow behavior |
|---|---|---|
| `static` (default) | Normal document flow | Can't be offset — `top/right/bottom/left` do nothing |
| `relative` | **Its own** normal position in the flow | Still occupies its original space; offsets shift it visually without pushing siblings |
| `absolute` | Nearest **positioned ancestor** (anything other than `static`) | Removed from document flow; offsets anchor to that ancestor's padding box |
| `fixed` | The **viewport** (or nearest ancestor with `transform`/`filter`/`will-change` — see gotcha) | Removed from flow; stays put while the page scrolls |
| `sticky` | Its scrollport (nearest scrolling ancestor) | Acts `relative` until scroll crosses a threshold, then "sticks" |

**Gotcha 1 — `absolute` containing block:** "nearest positioned ancestor" specifically means the nearest ancestor with `position` set to anything other than `static` (the default). A common pattern is wrapping an absolutely-positioned element in a `position: relative` parent **with no offset values** — just to establish that containing context:

```css
.card { position: relative; }          /* just establishes context */
.card__badge { position: absolute; top: 8px; right: 8px; }
```

**Gotcha 2 — `fixed` can be trapped:** `transform`, `filter`, and `will-change` on an ancestor also create a containing block for `position: fixed` descendants (not just `absolute`) — a frequently-missed gotcha when a "fixed" element unexpectedly scrolls with its parent.

**Gotcha 3 — `sticky` requirements:** it needs (1) a threshold value (`top`, `bottom`, etc.), and (2) **no ancestor with `overflow: hidden/scroll/auto` between it and its scrolling container** — if any ancestor clips overflow, sticky silently stops working. This is one of the most common "why isn't sticky working" bugs.

```css
.header { position: sticky; top: 0; } /* works only if no middle ancestor clips overflow */
```

---

### 🟢 Q5. What is the difference between Flexbox and CSS Grid?

**Answer:**
Both are modern layout systems, but they think in different dimensions — the #1 way to decide between them:

| | Flexbox | Grid |
|---|---|---|
| Dimension | **1D** — lays out along one axis at a time (row **or** column) | **2D** — defines rows *and* columns up front |
| Mental model | Content-driven: items flow in, sizing themselves by content unless told otherwise | Layout-driven: you define the structure first, then place content into it |
| Strength | Components and content with unknown size — nav bars, button groups, toolbars | Page/app-level layouts where you know the target structure — dashboards, whole-page templates |
| Wrap | Items wrap within one axis; wrapped lines don't align across axes | Full grid cell alignment, tracks, and region-naming |

**The differentiator worth stating out loud:** Flexbox is naturally *content-sized* — items grow/shrink based on their content unless told otherwise — good for components where you don't know content size ahead of time. Grid lets you define the structure first (explicit rows/columns) and place content into it — better when you have a target layout in mind regardless of content. Also, Grid can do most of what Flexbox does (single row/column grids exist), but Flexbox **cannot** do true 2D alignment across both axes simultaneously — that's Grid's defining advantage.

```css
/* Flexbox — flow an unknown set of items along one axis */
.toolbar { display: flex; gap: 8px; align-items: center; }

/* Grid — declare the structure, fit content into it */
.dashboard {
  display: grid;
  grid-template-columns: 240px 1fr 1fr;
  grid-template-rows: auto 1fr;
  grid-template-areas:
    "sidebar main main"
    "sidebar footer footer";
}
```

---

### 🟢 Q6. What is the difference between `display: none` and `visibility: hidden`?

**Answer:**
Both hide an element visually, but behave very differently structurally:

| | `display: none` | `visibility: hidden` |
|---|---|---|
| Occupies space | No — removed from layout entirely | Yes — space is preserved |
| Reflow triggered | Yes — layout recalculates without it | Yes (less impact, no layout shift) |
| Children can override | No — children inherit; can't be shown individually | Yes — a child can set `visibility: visible` to reappear even if parent is hidden |
| Screen readers | Not announced, not in accessibility tree | Not announced, not in accessibility tree |
| Transitions/animations | Cannot animate (element isn't rendered) | Can be combined with opacity transitions for fade effects |
| Focusable | No | No (but still technically in tab order in some browsers — use with caution) |

```css
.a { display: none; }       /* gone — no space reserved */
.b { visibility: hidden; }  /* invisible — space still reserved */
```

Use `display: none` when you want an element to genuinely not exist in the layout (e.g., inactive tab panels). Use `visibility: hidden` when you need to preserve layout position (e.g., hiding one element in a row without the rest reflowing) or plan to reveal a nested child independently.

---

### 🟢 Q7. What is the CSS cascade, and how does it differ from specificity?

**Answer:**
The cascade is the overall algorithm the browser uses to resolve which declaration wins when multiple rules target the same property on the same element. Specificity is just one input into that algorithm — the cascade is the bigger picture.

The full cascade order (highest priority first, as of modern CSS):

1. **Origin and importance** — user `!important` > author `!important` > author normal styles > user normal styles > browser default styles (with some nuance around user-agent `!important`).
2. **Cascade layers (`@layer`)** — layers declared later win over earlier ones; all layered styles beat unlayered styles unless `!important` flips this (see Q34, Q42).
3. **Specificity** — ID vs class vs element (see Q3).
4. **Order of appearance** — last declared rule wins when everything above ties.

So specificity is one step in a larger, ordered decision process — origin and layers are actually evaluated *before* specificity, meaning a low-specificity rule in a later layer can beat a high-specificity rule in an earlier layer. This is a common point of confusion: people assume specificity is the final word, but layers now sit above it in priority.

---

### 🟢 Q8. What is the difference between inline, inline-block, and block display values?

**Answer:**

| | `inline` | `inline-block` | `block` |
|---|---|---|---|
| New line | No | No | Yes |
| Width/height respected | No (ignored) | Yes | Yes |
| Vertical margin/padding | Visually applied but doesn't push surrounding inline content away | Fully respected | Fully respected |
| Horizontal margin/padding | Fully respected | Fully respected | Fully respected |
| Can contain block elements | No | Yes | Yes |

```css
.inline { display: inline; }             /* e.g. <span>, <a> default */
.inline-block { display: inline-block; } /* e.g. <img>, <button> default */
.block { display: block; }               /* e.g. <div>, <p> default */
```

`inline-block` is the useful middle ground: it flows inline with text (doesn't force a new line) but still respects width, height, and full padding/margin — this is why it's a common choice for things like nav items or badges laid out horizontally that still need explicit sizing.

---

### 🟢 Q9. What are pseudo-classes vs pseudo-elements? (`:hover` vs `::before`)

**Answer:**
**Pseudo-classes** (single colon `:`) select elements based on *state or position* — they target real elements that already exist in the DOM, just in a particular condition:

```css
a:hover { color: red; }        /* state */
li:first-child { }             /* position */
input:focus { }                /* state */
p:nth-child(odd) { }           /* position */
```

**Pseudo-elements** (double colon `::`, though single colon still works for legacy ones like `:before`) target a *sub-part of an element* that isn't a real DOM node — the browser generates it:

```css
p::first-line { font-weight: bold; }
.tooltip::before { content: "→"; }
input::placeholder { color: gray; }
```

Key distinction: pseudo-classes describe *when/how* a real element applies (its state); pseudo-elements describe a fictional sub-element the browser conjures for styling purposes (part of an element, or generated content that isn't in the DOM/accessibility tree by default). This also affects specificity — pseudo-classes count with classes `(0,0,1,0)`, pseudo-elements count with element selectors `(0,0,0,1)`.

---

### 🟢 Q10. What is margin collapsing and how does it work?

**Answer:**
When two block-level elements' vertical margins meet, they don't add together — the larger of the two margins wins, and the smaller is absorbed. This only happens with vertical margins (top/bottom), never horizontal.

Three scenarios where it happens:

**1. Adjacent siblings** — bottom margin of one, top margin of the next:
```css
.a { margin-bottom: 30px; }
.b { margin-top: 20px; }
/* actual gap between them = 30px, not 50px */
```

**2. Parent and first/last child** — if there's no border, padding, or content separating a parent's top from its first child's top margin, they collapse into one:
```css
.parent { margin-top: 0; }
.parent .first-child { margin-top: 40px; }
/* parent effectively gets pushed down 40px too — margin "escapes" the parent */
```

**3. Empty elements** — an element with no height, border, or padding: its own top and bottom margins collapse into each other.

**How to prevent it (when unwanted):** add `padding` or `border` to the parent (even 1px), use `overflow: hidden` on the parent (creates a new Block Formatting Context), use flexbox/grid (collapsing doesn't happen inside flex/grid containers), or use `display: flow-root` on the parent (the modern, purpose-built fix):

```css
.parent { display: flow-root; } /* stops margin collapsing without side effects */
```

---

### 🟢 Q11. What are CSS combinators?

**Answer:**
Combinators define the relationship between selectors — how one part of a selector relates structurally to another:

| Combinator | Syntax | Meaning |
|---|---|---|
| Descendant | `A B` | B is anywhere inside A (any depth) |
| Child | `A > B` | B is a direct child of A |
| Adjacent sibling | `A + B` | B is immediately after A, same parent |
| General sibling | `A ~ B` | B is anywhere after A, same parent (not necessarily adjacent) |

```css
.nav li { }         /* any <li> inside .nav, any depth */
.nav > li { }        /* only direct <li> children of .nav */
h2 + p { }           /* the <p> immediately following an <h2> */
h2 ~ p { }           /* all <p> siblings after an <h2>, not just the first */
```

Practical use: `+` is very common for spacing patterns (e.g., "add margin-top to every element except the first" via `* + * { margin-top: 1rem; }`), and `>` is used to avoid accidentally styling deeply nested elements you didn't intend to target.

---

### 🟢 Q12. What is a CSS reset / normalize.css, and why use one?

**Answer:**
Every browser ships default (user-agent) stylesheets with inconsistent baseline styling — different default margins on `<h1>`, different `<ul>` padding, different form control appearances, etc. A reset or normalize stylesheet neutralizes these inconsistencies before your own CSS applies.

**Reset** (e.g., Eric Meyer's classic reset, or the aggressive `* { margin: 0; padding: 0; }` approach): strips almost all default styling to zero, giving you a completely blank slate you build up from scratch.

**Normalize.css:** takes the opposite philosophy — preserves useful defaults (like heading size differences) but fixes cross-browser inconsistencies and bugs (e.g., `<sub>`/`<sup>` line-height issues, inconsistent `<button>` styling across browsers).

Modern practice trends toward a lightweight, custom "modern CSS reset" (popularized by Josh Comeau, Andy Bell) that targets specific known pain points rather than wiping everything:

```css
*, *::before, *::after { box-sizing: border-box; }
* { margin: 0; }
html { -webkit-text-size-adjust: 100%; }
img, picture, video, canvas { display: block; max-width: 100%; }
input, button, textarea, select { font: inherit; }
```

Why bother: without this, the same markup can look meaningfully different across Chrome/Firefox/Safari before you've written a single line of your own CSS — resets establish a consistent, predictable starting point.

---

### 🟡 Q13. What is a stacking context and why does `z-index` sometimes "not work"?

**Answer:**
`z-index` decides the paint order of overlapping elements **within the same stacking context**. A stacking context is an isolated grouping — elements inside it are painted as one unit relative to the outside world, so their internal `z-index` values can't compete against elements in other contexts.

**What creates a stacking context** (beyond the obvious `position` + `z-index`):
- The root element (`<html>`)
- `position: relative/absolute` with a `z-index` other than `auto`
- **`position: fixed` or `sticky` — always**, even with `z-index: auto` (commonly missed)
- Opacity less than 1, `transform`, `filter`, `will-change`, `backdrop-filter`, `clip-path`, `mix-blend-mode`, `contain`
- **Flex/Grid items with `z-index` set (not `auto`)** — a common surprise when flex children with `z-index` don't layer as expected relative to non-flex-item siblings
- `isolation: isolate`

**Why `z-index` "doesn't work":** usually because the two competing elements belong to *different* stacking contexts, and the decision is being made higher up the tree — comparing the ancestors' `z-index`, not the descendants'. If an ancestor has a low `z-index` (or is inside a depth-3 context), nothing its children do with `z-index` escapes that group.

```css
.parent { position: relative; z-index: 1; }      /* context A */
.child  { position: absolute; z-index: 999; }    /* trapped inside A */

.sibling { position: absolute; z-index: 2; }     /* wins, because A as a whole loses */
```

**Debugging tip:** Chrome DevTools' "Layers" panel (under More Tools) visualizes stacking contexts directly — much faster than reasoning through the rules by hand.

---

### 🟡 Q14. What are CSS custom properties and how do they work?

**Answer:**
Custom properties (`--name: value`) are user-defined CSS variables that participate fully in the **cascade and inheritance** like any real CSS property — which is their biggest advantage over preprocessor variables.

```css
:root {
  --color-primary: #0066ff;
  --spacing-md: 1rem;
}

.button { color: var(--color-primary); }
```

**Key points:**
- Defined with `--` prefix, read with `var(--name)`.
- Values only resolve where used — a media query can override `--spacing-md` at a breakpoint, and *everything* using `var(--spacing-md)` updates automatically, no preprocessor recompilation needed.
- Strange but standard character range for names: letters, numbers, `-`, `_` (underscores, since CSS4). Hyphens are fine except leading `--`.

**Fallback values guard against silently-broken layouts:**

```css
.button { color: var(--text-color, black); } /* uses black if --text-color is unset */
```

This matters because unlike Sass variables, an *undefined* custom property doesn't throw a build error — it silently computes to nothing (the initial value, or inherited), which can cause layout to "disappear" without an obvious cause. Fallback values protect against that.

**Animating caveat:** plain custom properties can't be smoothly animated between two values because the browser doesn't know their type. Registering a type in advance — via the CSS Houdini Properties & Values API (see Q31) — is what unlocks interpolation.

---

### 🟡 Q15. What is the BEM methodology?

**Answer:**
BEM (Block, Element, Modifier) is a naming convention that makes CSS class names self-describing and collision-proof. Each selector name reveals its role in the design, not its position in a stylesheet.

- **Block** — a standalone entity: `block`
  - `.card`, `.nav`, `.button`
- **Element** — a part of a block, denoted with two underscores: `block__element`
  - `.card__title`, `.card__image`
- **Modifier** — a state or variant, denoted with two hyphens: `block--modifier` or `block__element--modifier`
  - `.button--primary`, `.card__title--featured`

```html
<div class="card card--featured">
  <h2 class="card__title">Hello</h2>
  <p class="card__body">...</p>
  <button class="card__button card__button--primary">Action</button>
</div>
```

**Why it works:**
- **Specificity stays flat** — every rule is a single class, so overrides are trivial and predictable
- **No deep descendant selectors** like `.card .title p` — the full relationship is in the name
- **Reusable and self-documenting** — the markup alone reads as a design spec

**Common point of confusion — elements don't nest with DOM nesting:** `.card__title` is flat, *not* `.card__body__title`, even if title is nested inside body inside card in the actual markup. The naming reflects the block relationship, not literal DOM depth. This trips up people applying BEM for the first time who instinctively want to mirror HTML structure in the class names.

```html
<!-- Correct BEM: flat names, even when DOM is nested -->
<div class="card">
  <div class="card__body">
    <h2 class="card__title">Flat, not card__body__title</h2>
  </div>
</div>
```

**Trade-offs:** verbose class names bloat HTML; it's a naming discipline (no enforcement) — consistency is on the team. Fine with CSS Modules, a stricter alternative.

---

### 🟡 Q16. How does Angular's view encapsulation work?

**Answer:**
View encapsulation controls whether a component's CSS can leak out to the rest of the app, by scoping styles to the component's own template. It's configured on each component:

```ts
@Component({
  selector: 'app-card',
  encapsulation: ViewEncapsulation.Emulated, // default
  styles: [`:host { display: block; }`]
})
export class CardComponent {}
```

| Strategy | Behavior |
|---|---|
| `Emulated` (default) | Styles are rewritten with attribute selectors (`[_ngcontent-abc123]`) so they only match this component's own DOM. Real Shadow DOM is *not* used — it's a lightweight approximation |
| `ShadowDom` | Uses the native Shadow DOM — true style isolation, both directions. Styles can't get out, page styles can't get in (except inherited properties like `font-family`) |
| `None` | Styles are injected globally — no scoping at all |

**Escaping the component boundary — `::ng-deep` and its deprecation:** `::ng-deep` punches through encapsulation to style child components (e.g., customizing a third-party library's internals). But it's **deprecated**, and browsers are actively removing native `::deep`/`>>>` combinator support — Angular's own docs recommend avoiding it. The modern approach for intentionally leaking styles into child components is scoping via `:host` and `:host-context()`, or simply lifting shared styles into global stylesheets rather than punching through encapsulation.

```css
/* :host — styles the component's own root element */
:host { display: block; }

/* :host-context — style based on an ancestor's class (e.g. a theme) */
:host-context(.dark-theme) { color: white; }

/* Avoid: deprecated and being removed from browsers */
::ng-deep .child { color: red; }
```

**Angular vs Web Components:** Angular components compile to standard JS/DOM but are *not* Web Components by default — the real Shadow DOM encapsulation is opt-in via `ViewEncapsulation.ShadowDom`, or by wrapping with `@angular/elements`.

---

### 🟡 Q17. What is the difference between CSS animations and JS animations?

**Answer:**

| | CSS Animations / Transitions | JS Animations (e.g. `requestAnimationFrame`, GSAP) |
|---|---|---|
| Performance | Can run entirely on the **compositor thread** for `transform`/`opacity` — smooth even when the main thread is busy | Runs on the **main thread** (unless using WAAPI/plugins offloading to compositor) — can jank under heavy JS load |
| Control | Declarative, limited — no easy pause/resume/seek/reverse mid-flight | Full imperative control — pause, resume, reverse, seek, trigger physics, respond to dynamic state |
| Complexity | Best for simple state transitions (`:hover`, class toggles) | Needed for complex sequencing, physics (springs, inertia), scroll-linked/bézier-spline motion |
| Web Animations API (WAAPI) | — | Native, no library — JS-level control **plus** compositor-thread execution for `transform`/`opacity`, closing much of the performance gap with pure CSS |

**The middle ground many answers miss — the Web Animations API:**

```js
element.animate(
  [{ transform: 'translateX(0)' }, { transform: 'translateX(100px)' }],
  { duration: 300, easing: 'ease-out', fill: 'forwards' }
);
```

`element.animate()` gives JS-level control (play/pause/reverse/seek) while still being able to run on the compositor thread for `transform`/`opacity` animations — closing much of the performance gap with pure CSS.

**A good default hierarchy:**
1. **CSS** for simple state transitions (`:hover`, visibility, toggling classes)
2. **Web Animations API** for JS-controlled but performant animation
3. **GSAP/library** when you need complex sequencing, physics, or broad cross-browser easing support beyond what natives offer

**Performance rule of thumb:** animate only `transform` and `opacity` if you care about smoothness — those skip layout/paint. Animating `top`/`left`/`width`/`height` forces re-layout every frame, which is the classic jank source regardless of CSS vs JS.

---

### 🟡 Q18. How do media queries work, and what's mobile-first vs desktop-first CSS?

**Answer:**
Media queries apply CSS conditionally based on characteristics of the viewport/device — most commonly width, but also orientation, resolution, and (increasingly) user preferences (`prefers-color-scheme`, `prefers-reduced-motion`).

```css
@media (min-width: 768px) {
  .container { flex-direction: row; }
}
```

**Mobile-first:** base styles target the smallest screen, then `min-width` queries progressively add complexity/layout changes for larger screens:

```css
.container { display: block; }             /* mobile default */
@media (min-width: 768px) {
  .container { display: flex; }            /* enhance for tablet+ */
}
```

**Desktop-first:** base styles target the largest screen, then `max-width` queries strip down/simplify for smaller screens:

```css
.container { display: flex; }              /* desktop default */
@media (max-width: 767px) {
  .container { display: block; }           /* simplify for mobile */
}
```

**Why mobile-first is generally preferred:** it forces you to prioritize essential content/layout first (better discipline), tends to produce leaner CSS (mobile devices don't have to override desktop styles they'll never fully need), and aligns with the reality that mobile traffic dominates for most sites. It also plays better with progressive enhancement as a general philosophy.

---

### 🟡 Q19. What are CSS Grid's `fr` unit, `minmax()`, and auto-fit vs auto-fill?

**Answer:**
**`fr` (fraction unit):** distributes remaining space proportionally after fixed-size tracks are accounted for:

```css
.grid { grid-template-columns: 200px 1fr 2fr; }
/* first column fixed 200px; remaining space split 1:2 between the other two */
```

**`minmax(min, max)`:** defines a track's size range — grows up to `max`, shrinks down to `min`, never smaller/larger:

```css
grid-template-columns: repeat(3, minmax(200px, 1fr));
/* each column at least 200px, but grows to fill available space equally */
```

**auto-fit vs auto-fill:** both used with `repeat()` to create a responsive number of columns without media queries — the difference only shows when there's leftover space:

```css
grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
```
- **auto-fill:** keeps creating empty tracks to fill the row, even if there's no content for them — items don't stretch to fill leftover space, they stay their intrinsic/minmax size, empty tracks just sit there invisible.
- **auto-fit:** collapses empty tracks to zero width, then stretches existing items to consume the freed space.

This combo (`repeat(auto-fit, minmax(200px, 1fr))`) is the single most common "responsive card grid, no media queries" pattern in modern CSS.

---

### 🟡 Q20. What is `clamp()`, `min()`, and `max()` used for in responsive design?

**Answer:**
These are CSS math functions that let you define fluid, responsive values without media queries.

**`clamp(min, preferred, max)`:** locks a value between a minimum and maximum, using a "preferred" value (often viewport-relative) in between:

```css
font-size: clamp(1rem, 2vw + 0.5rem, 2.5rem);
/* never smaller than 1rem, never larger than 2.5rem, scales fluidly between */
```

**`min()`:** picks the smallest of a list of values — useful for "never exceed X, but shrink if needed":

```css
width: min(90%, 600px); /* fluid up to 600px, then caps */
```

**`max()`:** picks the largest — useful for "never go below X":

```css
padding: max(16px, 2vw); /* never less than 16px, grows with viewport */
```

**Why this matters:** before these functions, fluid typography/spacing required multiple media query breakpoints with hard jumps between sizes. `clamp()` gives smooth, continuous scaling with a single line, and reduces the total CSS needed for responsive design significantly.

---

### 🟡 Q21. What's the difference between CSS transitions and CSS animations (`@keyframes`)?

**Answer:**

| | Transitions | Animations (`@keyframes`) |
|---|---|---|
| Trigger | State change (hover, class toggle, JS-set property) | Runs automatically on element load, or via trigger |
| Number of states | Two (start → end) | Multiple (any number of keyframe steps) |
| Looping | No — runs once per trigger | Yes — `animation-iteration-count: infinite` |
| Direction control | No | Yes — `animation-direction: alternate`, etc. |
| Requires a trigger event | Yes (something must change the property) | No — can run automatically on page load |

```css
/* Transition: needs a state change to fire */
.button { transition: background 0.3s ease; }
.button:hover { background: blue; }

/* Animation: runs independently, multiple steps, can loop */
@keyframes pulse {
  0% { transform: scale(1); }
  50% { transform: scale(1.1); }
  100% { transform: scale(1); }
}
.badge { animation: pulse 2s infinite ease-in-out; }
```

**Rule of thumb:** use transitions for simple two-state changes tied to user interaction (hover, focus, class toggle). Use animations for anything looping, multi-step, or that needs to run without a trigger (loading spinners, entrance animations, attention-getters).

---

### 🟡 Q22. What is float and clearfix, and why is it rarely used for layout now?

**Answer:**
**`float`** was originally designed for wrapping text around images (`float: left` on an `<img>`) — it pulls an element out of normal flow, shifts it to one side, and lets inline content wrap around it.

It got repurposed as a layout hack in the pre-Flexbox/Grid era (roughly 2005–2015) to build multi-column layouts, since there was no proper tool for that yet.

**The core problem:** a floated element is removed from the normal document flow, so its parent container collapses to zero height if all its children are floated (the parent doesn't "see" the floated content as taking up space).

**Clearfix** was the workaround — forcing the parent to recognize the floated content's height:

```css
.clearfix::after {
  content: "";
  display: table;
  clear: both;
}
```

**Why it's rarely used now:** Flexbox and Grid were purpose-built for layout, handle alignment/distribution natively, don't collapse parent height, and don't require hacky pseudo-element workarounds. `float` today is mostly back to its original intended use — wrapping text around an image within an article — not full-page layout.

---

### 🟡 Q23. What are CSS logical properties (`margin-inline`, `padding-block`) vs physical ones?

**Answer:**
**Physical properties** are tied to fixed screen directions: `margin-left`, `padding-top`, `border-right`, `width`.

**Logical properties** are relative to the *writing mode and text direction* of the content, not fixed screen edges: `margin-inline-start`, `padding-block-end`, `inset-inline`.

```css
/* Physical — assumes left-to-right, top-to-bottom */
.card { margin-left: 16px; padding-top: 8px; }

/* Logical — adapts automatically to writing mode/direction */
.card { margin-inline-start: 16px; padding-block-start: 8px; }
```

**Why this matters:** in a left-to-right language (English), `margin-inline-start` behaves exactly like `margin-left`. But in a right-to-left language (Arabic, Hebrew), it automatically flips to behave like `margin-right` — no manual RTL override stylesheet needed. Similarly, block/inline axes adapt for vertical writing modes (some CJK typesetting).

**Key terms:** *inline axis* = the direction text flows within a line (horizontal in English). *block axis* = the direction blocks stack (vertical in English). For sites that need to support multiple languages/directions, logical properties eliminate an entire category of manual RTL-specific overrides.

---

### 🟡 Q24. What is `aspect-ratio` and what problem does it solve?

**Answer:**
`aspect-ratio` lets you declare a fixed width-to-height ratio for an element, so the browser calculates one dimension automatically from the other:

```css
.video-wrapper { aspect-ratio: 16 / 9; }
img { aspect-ratio: 1 / 1; object-fit: cover; }
```

**The problem it solves:** before this property (added ~2021), maintaining aspect ratio for responsive elements (especially video embeds) required a hacky "padding-top percentage trick":

```css
/* Old hack */
.video-wrapper {
  position: relative;
  padding-top: 56.25%; /* 9/16 = 0.5625, forces 16:9 */
}
.video-wrapper iframe {
  position: absolute; top: 0; left: 0; width: 100%; height: 100%;
}
```

`aspect-ratio` replaces this entirely with one clean line, and works for any element (not just ones you can absolutely-position children into). It's also essential for preventing Cumulative Layout Shift — reserving image space before the image loads:

```css
img { width: 100%; aspect-ratio: 16 / 9; object-fit: cover; }
```

---

### 🟡 Q25. What's the difference between `overflow: hidden`, `scroll`, and `auto`?

**Answer:**
Controls what happens when content exceeds an element's box:

- **`hidden`** — excess content is clipped and simply invisible — no scrollbar, no way to access it (unless scrolled programmatically via JS)
- **`scroll`** — always shows scrollbars (both axes by default), even if content fits — can create unnecessary scrollbars on content that doesn't actually overflow
- **`auto`** — shows scrollbars only if content actually overflows — the most commonly desired behavior, adaptive

```css
.clip { overflow: hidden; }   /* content cut off, no access */
.always-scroll { overflow: scroll; }  /* scrollbar always visible */
.smart { overflow: auto; }    /* scrollbar appears only when needed */
```

You can also set each axis independently: `overflow-x: hidden; overflow-y: auto;` (common for preventing horizontal scroll while allowing vertical). Note: setting `overflow` to anything other than `visible` also creates a new Block Formatting Context, which has side effects — it stops margin collapsing (see Q10) and contains floats, which is sometimes used intentionally as a layout trick.

---

### 🟡 Q26. What are CSS methodologies like BEM, OOCSS, SMACSS, and utility-first (Tailwind)? How do they compare?

**Answer:**
**BEM (Block, Element, Modifier)** — see Q15. A naming convention preventing specificity conflicts via flat, single-class selectors.

**OOCSS (Object-Oriented CSS)** — separates *structure* from *skin*: define reusable structural patterns (e.g., a generic "media object" layout: image + text side by side) separately from visual theming (colors, borders), so the same structural class can be reused with different skins:

```css
.media { display: flex; gap: 12px; }        /* structure */
.media--card { background: white; border-radius: 8px; }  /* skin */
```

**SMACSS (Scalable and Modular Architecture for CSS)** — categorizes styles into five types: Base (element defaults), Layout (major page regions), Module (reusable components), State (JS-toggled states like `.is-active`), Theme (visual variations). More about organizing your stylesheet than a naming convention specifically.

**Utility-first (Tailwind CSS being the dominant example)** — instead of writing semantic component classes, you compose styling directly in markup using small, single-purpose utility classes:

```html
<div class="flex items-center gap-3 p-4 bg-white rounded-lg shadow">
```

**Comparison:**

| | Approach | Strength | Trade-off |
|---|---|---|---|
| BEM / OOCSS / SMACSS | Semantic component classes in a separate CSS file | Markup and CSS cleanly separated; meaningful names for design systems | Naming discipline required; more CSS to maintain |
| Utility-first (Tailwind) | Single-purpose utilities composed in markup | No naming decisions, no dead CSS, design constraints baked into a scale | Verbose/cluttered HTML |

Modern teams increasingly favor utility-first (Tailwind) for app-development speed, while BEM-style approaches remain common in component libraries, marketing sites, or CMS-driven theming.

---

### 🟡 Q27. What is `will-change` and when should (and shouldn't) you use it?

**Answer:**
`will-change` is a hint to the browser that a property is about to change, letting the browser pre-optimize by promoting the element to its own compositor layer ahead of time — avoiding the small delay/jank that can occur when a layer is created just-in-time as an animation starts:

```css
.modal { will-change: transform, opacity; }
```

**When to use it:** on elements you know will be animated soon and where you've observed actual jank — e.g., right before triggering a complex transform-based animation (a modal opening, a drawer sliding in).

**When NOT to use it** — this is the more important half:
- **Don't** apply it broadly/permanently to many elements "just in case" — each `will-change` layer consumes GPU memory, and too many layers can hurt performance more than help it
- **Don't** leave it on indefinitely — best practice is to add it via JS shortly before the animation starts and remove it after the animation completes, rather than hardcoding it in a stylesheet forever
- **Don't** use it as a blanket performance fix — it's a targeted hint for specific, known-jank scenarios, not a general "make things faster" toggle

```js
el.addEventListener('mouseenter', () => el.style.willChange = 'transform');
el.addEventListener('animationend', () => el.style.willChange = 'auto');
```

---

### 🟡 Q28. What is `clip-path` and how does it differ from mask?

**Answer:**
**`clip-path`** defines a geometric region — everything outside that region is hidden, everything inside is fully visible (binary — no partial transparency):

```css
.avatar { clip-path: circle(50%); }
.badge { clip-path: polygon(50% 0%, 100% 50%, 50% 100%, 0% 50%); }
```

**`mask`** uses an image (gradient, SVG, PNG with alpha) as a transparency map — it supports partial/graduated transparency, not just hard on/off boundaries:

```css
.fade-edge {
  mask-image: linear-gradient(to bottom, black 80%, transparent 100%);
}
```

**Key difference:** `clip-path` is for hard-edged geometric shapes (circles, polygons, custom SVG paths) — good for cropping into simple shapes. `mask` is for soft, graduated, or complex transparency effects (fade-outs, texture-based reveals, using an image's luminance/alpha as the mask source) — much more flexible but also more expensive to render.

Both are hardware-accelerated on transform/opacity-adjacent rendering paths in modern browsers, but `clip-path` is generally cheaper since it doesn't require sampling a separate image.

---

### 🔴 Q29. Explain the rendering pipeline: Layout, Paint, Composite.

**Answer:**
After the browser builds the DOM + CSSOM and merges them into the render tree, three consecutive stages turn it into pixels — and crucially, a style/DOM change only re-runs the **minimum** affected stages:

1. **Layout (a.k.a. Reflow)** — Computes exact position and box-model geometry for every render-tree node, relative to the viewport: `width`, `height`, `top`, `left`, text-wrapping, etc. Automatically triggered by DOM changes, viewport resizes, and font/first-paint.
2. **Paint** — Rasterizes pixels (text, color, borders, shadows) into layers on the main thread. Painting happens once per layer, then layers are cached.
3. **Composite** — Done on the compositor (GPU) thread: layers are assembled/transformed/opacity-adjusted and merged into the final frame.

**What each property change costs:**

| You change... | Stages re-run |
|---|---|
| `transform`, `opacity` | **Composite only** — the cheap ones; this is why they're the gold standard for animation |
| `color`, `background-color`, `box-shadow` | Paint + Composite (layout unaffected) |
| `width`, `height`, `margin`, `font-size`, `top/left` | Layout + Paint + Composite (the expensive ones) |

**The critical addition — layout thrashing:** reading a layout-dependent property (`offsetWidth`, `getBoundingClientRect()`) immediately after writing a style change forces a synchronous, **forced reflow** — the browser can't wait for its normal batching, it must recalculate layout right then to give you an accurate read.

```js
// Bad — forces reflow on every iteration (layout thrashing)
elements.forEach(el => {
  el.style.width = '100px';        // write
  console.log(el.offsetWidth);     // read → forces synchronous layout
});

// Good — batch reads, then batch writes
const widths = elements.map(el => el.offsetWidth);  // all reads first
elements.forEach((el, i) => el.style.width = widths[i] + 10 + 'px'); // then writes
```

This read/write interleaving is one of the most common real-world causes of janky scrolling/animation in JS-heavy pages.

**Performance levers that follow directly:**
- `content-visibility: auto` skips layout/paint for offscreen content (see Q30)
- Batch DOM reads and writes; use `requestAnimationFrame` to align writes
- Use compositor-friendly animations (`transform`/`opacity`) and `will-change` sparingly to promote hot elements to their own layers

---

### 🔴 Q30. What is CSS containment and how does it improve performance?

**Answer:**
CSS containment (`contain`) tells the browser that an element's subtree is isolated from the rest of the page, letting the browser **skip layout and paint work** for parts it can prove are unaffected by changes elsewhere — and vice versa.

```css
/* Strict: layout, paint, size, style containment all on */
.leaf-component { contain: strict; }
```

**The `contain` values:**
- `layout` — the element's descendants can't affect layout outside the element (nor vice versa)
- `paint` — descendants can't paint outside the element's bounds (clipped)
- `size` — the element is sized *without* needing to lay out its children first
- `style` — counters/font-features don't leak across the boundary
- `strict` — everything (`layout paint size`)
- `content` — `layout paint` (not `size`), safe when the element's size is content-dependent

**Close relative: `content-visibility: auto`.** Where `contain` isolates a subtree, `content-visibility: auto` builds on it by **skipping rendering work (layout, paint) for offscreen content entirely** — only rendering it once it's about to enter the viewport (similar spirit to `loading="lazy"`, but for arbitrary content, not just images):

```css
.section { content-visibility: auto; contain-intrinsic-size: 0 500px; }
```

`contain-intrinsic-size` reserves an estimated size so the page doesn't jump around as content is skipped/rendered — this pairing is the modern go-to for very long pages (huge comment threads, long articles) where rendering everything upfront is wasteful. Use generous estimates either real values (e.g., `auto 500px`) for accurate scrollbar/CLS behavior.

**Trade-off to mention:** with `content-visibility: auto`, the browser must repaint the region when it scrolls into view — so it helps long, discrete, content-heavy pages, not pages with always-visible animations or small DOMs.

---

### 🔴 Q31. What is CSS Houdini?

**Answer:**
CSS Houdini is a collection of browser APIs that expose parts of the CSS engine to JavaScript — letting developers *hook into how CSS works* instead of working around it: custom paint routines (`paint(worklet)`), customized layout algorithms, and registered, animatable custom properties.

**The main APIs:**

| API | What it does | Support reality |
|---|---|---|
| Paint Worklet (`CSS.paintWorklet`) | Define custom drawable values for `background-image`, etc. via small paint programs | Chromium-only in practice |
| Layout Worklet | Implement custom layout algorithms (like creating your own `display` value) | Chromium/experimental only |
| Animation Worklet | High-performance procedural animation on the compositor thread (scroll-linked, physics-driven) | Chromium/experimental only |
| Properties & Values API (`CSS.registerProperty` / `@property`) | Register a custom property's type, initial value, and inheritance — enabling animation | **Best cross-browser support; practically usable today** |

**The honest caveat:** most Houdini APIs (Paint, Layout, Animation Worklets) are Chromium-only in practice — Firefox and Safari have limited or no support for most of them as of the last couple of years. That makes almost all of Houdini research/experimental territory today, *except* the Properties & Values API.

**The genuinely useful piece — typed custom properties:**

```css
@property --progress {
  syntax: '<number>';
  inherits: false;
  initial-value: 0;
}
```

Registration gives the browser the *type* and *interpolation behavior* it needs — which is exactly what enables smooth animation of custom properties (e.g., animating a gradient angle or a numeric counter), which plain custom properties can't do since the browser doesn't know their type without registration:

```css
.counter { --progress: 0; transition: --progress 1s; }
.counter:hover { --progress: 100; }  /* animates now that the type is registered */
```

That's the realistic answer on Houdini: production-viable today for typed custom properties; the worklets are future-facing because of Chromium-only support.

---

### 🔴 Q32. How do you build a design token system in Angular?

**Answer:**
A design token system extracts design decisions (colors, spacing, type scale, radii, shadows) into named, reusable variables — one source of truth that themes, components, and apps consume instead of hard-coded values. In an Angular project it typically looks like this:

**1. Token tiers:**
- **Primitive/raw tokens** — the raw palette and scale, e.g. `--color-blue-500: #0b6cff`
- **Semantic tokens** — the *intent*-mapped layer, e.g. `--color-primary: var(--color-blue-500)`. The component layer consumes semantic tokens only, so a theme is purely a remap of semantic → primitive.

**2. Token definition lives outside components.** Store token values in CSS custom properties on `:root` and have components reference `var(--token)` (see Q14) — so a theme change is just overriding the `:root` variables, and every component updates at runtime with zero recompilation. Use `@property` registration (see Q31) for tokens you want to animate.

**3. The tooling most commonly used:** Style Dictionary (Amazon's open-source tool) is the standard concrete tool for generating tokens from a single source of truth — it takes token definitions in JSON/YAML and outputs them to CSS custom properties, SCSS variables, iOS/Android formats, TypeScript, etc. This matters if the design system spans web *and* native.

```json
{
  "color": {
    "primary": { "value": "#0b6cff" }
  }
}
```
```css
/* Generated output */
:root { --color-primary: #0b6cff; }
```
```ts
// Also emitted for Angular TS consumption
export const tokens = { colorPrimary: '#0b6cff' };
```

**Tip — keep tokens consumed via CSS custom properties (runtime-switchable), not only TS constants:** TS constants force a rebuild per theme; CSS custom properties allow instant theme switching.

**4. SSR/theme-flash gotcha (Angular Universal):** setting the theme attribute needs to happen **before first paint** to avoid a flash of the wrong theme — typically via an inline script in `index.html` reading a cookie/localStorage value synchronously, since Angular's own bootstrap happens too late to prevent the flash.

```html
<!-- index.html: runs before Angular renders, prevents theme flash -->
<script>
  var theme = localStorage.getItem('theme') || 'light';
  document.documentElement.setAttribute('data-theme', theme);
</script>
```

**Angular-specific wiring:** apply the theme attribute via `HostBinding` on the root `AppComponent` (`@HostBinding('attr.data-theme')`), or set it in an `APP_INITIALIZER` — but remember the index.html script is what kills the flash; Angular-side wiring keeps it in sync for subsequent runs.

---

### 🔴 Q33. What are `:is()`, `:where()`, and `:has()`?

**Answer:**
Three modern functional pseudo-classes (all supported in current browsers) that change how you write and reason about selectors:

**`:is()` — "any of these", with specificity of the most specific argument.** Groups selectors while still respecting specificity — reduce duplication without changing cascade behavior:

```css
/* Instead of: header p, main p, footer p { ... } */
:is(header, main, footer) p { margin: 0; }
```

`:is()` takes the specificity of its **most specific** argument selector. Note `:is()` internally type-constrains the default tag in a way `:where()` doesn't, so keep the worst-case argument specificity in mind.

**`:where()` — same grouping, but always zero specificity.** Best for "universal defaults" that must be trivially overridable — resets/normalizations you never want fighting component styles:

```css
/* Zero specificity — any component rule (even a single class) beats this */
:where(header, main, footer) p { color: gray; }
```

**`:has()` — the parent selector (finally!).** Lets you style **an ancestor or sibling based on its descendants**, closing a gap that used to require JS class-toggling:

```css
.card:has(.featured) { border-color: gold; }
/* Style a label when its input is focused, with no JS and no extra classes */
label:has(+ input:focus) { color: var(--color-primary); }
```

`:has()` is relative — you can also do `:has(> .child)` for direct children, `:has(+ .sibling)`, and combine with `:is()`. It's been one of the most significant CSS additions in years: previously *no pure-CSS parent selector existed*, so patterns like "style X based on what's inside/next to X" were impossible in CSS alone.

---

### 🔴 Q34. What are CSS cascade layers (`@layer`), and what problem do they solve?

**Answer:**
`@layer` lets you explicitly group CSS rules into named layers, with layer order determining priority — independent of selector specificity. Layers declared later win over layers declared earlier, regardless of how specific the selectors inside them are.

```css
@layer reset, base, components, utilities;

@layer reset {
  * { margin: 0; padding: 0; }
}

@layer components {
  .button { background: blue; padding: 8px 16px; }
}

@layer utilities {
  .bg-red { background: red; }
}

/* No !important needed — utilities layer beats components layer */
```

Because `utilities` is declared last, `.bg-red` in that layer beats `.button` in components, even if `.button` had higher specificity — layer order overrides specificity entirely between layers.

**The problem it solves:** the classic CSS pain point of "my utility class isn't overriding the component style because the component selector is more specific" — historically solved with `!important` wars or artificially inflating selector specificity. Layers let you declare intent explicitly ("utilities should always win over components") without fighting specificity math or reaching for `!important`.

**Third-party CSS** (e.g., a component library) can also be wrapped in its own layer, guaranteeing your own styles can override it predictably without needing to out-specificity it.

---

### 🔴 Q35. What is native CSS nesting, and how does it differ from Sass nesting?

**Answer:**
Native CSS nesting (finalized ~2023, now broadly supported) lets you nest selectors inside a parent rule directly in plain CSS, no preprocessor required:

```css
.card {
  padding: 16px;

  & .title {
    font-size: 1.25rem;
  }

  &:hover {
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  }
}
```

**Differences from Sass nesting:**
- The `&` is required for compound selectors in most cases in native CSS (`&.active`, `&:hover`) — Sass allows more implicit nesting patterns without needing `&` as often
- Native nesting is live in the browser — no build step, but also no Sass-specific features like `@extend`, mixins, functions, or loops
- Native nesting has stricter rules around what can be nested where (e.g., nesting a bare element selector like `p { }` directly requires explicit `&` context in some cases to avoid ambiguity with descendant combinators)
- Native nesting generates actual CSSOM rules the browser understands directly, versus Sass which compiles down to flat CSS at build time — meaning native nesting can theoretically be changed dynamically via JS (`CSSStyleSheet` manipulation) in ways compiled Sass output cannot

For most common patterns, native nesting now covers what people used Sass nesting for — but Sass remains relevant for its other features (variables with real math/logic, mixins, loops) that native CSS custom properties/nesting still don't fully replace.

---

### 🔴 Q36. What is CSS subgrid, and how does it differ from regular Grid?

**Answer:**
**Regular nested Grid:** when you put a grid inside a grid item, the inner grid defines its own independent tracks — it has no awareness of the outer grid's column/row sizing, so aligning nested grid items with the outer grid's columns requires manual, often duplicated, sizing.

**Subgrid** lets a nested grid *inherit* the track definitions of its parent grid instead of defining its own — so nested content aligns perfectly with the outer grid's columns/rows automatically:

```css
.outer {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
}

.card {
  grid-column: span 2;
  display: grid;
  grid-template-columns: subgrid; /* inherits the outer grid's column tracks */
}
```

**Why it matters:** the classic use case is a row of cards where each card has an image, title, and description — without subgrid, if one card's title wraps to two lines, the description below it doesn't align with the description in the next card (each card's internal grid is independent). With subgrid, all cards' internal rows can align to a shared set of row tracks across the whole row, so titles/descriptions line up perfectly regardless of individual content length — something that previously required JS to measure and sync heights manually.

---

### 🔴 Q37. What are container queries (`@container`), and how do they differ from media queries?

**Answer:**
**Media queries** respond to the viewport's dimensions — global, page-level context.

**Container queries** respond to a specific *container element's* own size — component-level context, independent of the viewport:

```css
.card-wrapper {
  container-type: inline-size;
  container-name: card;
}

@container card (min-width: 400px) {
  .card { flex-direction: row; }
}
```

**Why this matters:** media queries can't tell you how much space a component actually has — a sidebar widget might be narrow even on a huge desktop screen, or wide even on a small mobile screen if it spans full width in a different layout. Media queries only know the viewport, not the component's actual rendered context.

Container queries make components genuinely context-aware and reusable — the same `.card` component can respond correctly whether it's placed in a narrow sidebar or a wide main content area, without needing to know or care what the viewport size is. This is a major shift toward truly modular, drop-anywhere component design, which was previously only achievable with JS-based ResizeObserver hacks.

---

### 🔴 Q38. What are the new viewport units svh/lvh/dvh, and why were they introduced (mobile browser UI issue)?

**Answer:**
These are viewport-height units that address a long-standing mobile browser problem: `100vh` doesn't behave predictably on mobile because browser chrome (address bar, bottom toolbar) shows and hides dynamically as the user scrolls, and `vh` traditionally measures the largest possible viewport — causing content to be cut off behind browser UI, or layouts to jump when the UI toggles.

| Unit | Meaning |
|---|---|
| `svh` (small viewport height) | 1% of the viewport height when browser UI is fully expanded (smallest available space) — guarantees content fits even in the most cramped state |
| `lvh` (large viewport height) | 1% of the viewport height when browser UI is fully collapsed (largest available space) — closer to old `100vh` behavior |
| `dvh` (dynamic viewport height) | Actively tracks the real-time viewport height as browser UI shows/hides — most accurate, but can cause layout shifts as it recalculates live during scroll |

```css
.hero { height: 100svh; }  /* guaranteed to fit without being cut off */
.full-bleed { height: 100dvh; }  /* tracks live browser UI state */
```

**Practical guidance:** use `svh` for critical full-screen content you never want clipped (e.g., a hero section's call-to-action button must always be visible); use `dvh` when you want the layout to genuinely fill whatever space is currently available and don't mind it adjusting as the user scrolls.

---

### 🔴 Q39. What is scroll-snap, and how do you build a snapping carousel with pure CSS?

**Answer:**
`scroll-snap` lets you build carousel/slider-style snapping behavior using native scroll, no JavaScript required:

```css
.carousel {
  display: flex;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  gap: 16px;
}

.carousel__item {
  flex: 0 0 80%;
  scroll-snap-align: center;
}
```

**Key properties:**
- **`scroll-snap-type`** on the scroll container: axis (`x`, `y`, `both`) + strictness (`mandatory` — always snaps to nearest point after scroll ends; `proximity` — snaps only if close enough)
- **`scroll-snap-align`** on each child: where it snaps to within the container (`start`, `center`, `end`)
- **`scroll-padding`** on the container: offsets the snap points (useful if you have a sticky header overlapping the scroll area)
- **`scroll-margin`** on children: per-item offset adjustments to the snap point

**Why this matters:** before scroll-snap, carousels required JS libraries (Swiper, Slick) to calculate positions and animate scrolling manually. Native scroll-snap gets you smooth, touch-friendly, momentum-respecting snapping for free, with full native scrolling behavior (including keyboard/trackpad/touch support) — JS is only needed now for extras like custom pagination dots or autoplay.

---

### 🔴 Q40. What are `prefers-color-scheme` and `prefers-reduced-motion`, and how do you design for them?

**Answer:**
Both are media features that detect user-level OS/browser accessibility or preference settings, letting you respect the user's choices without requiring them to configure anything on your site specifically.

**`prefers-color-scheme`** — detects whether the user has set their OS to light or dark mode:

```css
:root { --bg: white; --text: black; }

@media (prefers-color-scheme: dark) {
  :root { --bg: #121212; --text: #eee; }
}

body { background: var(--bg); color: var(--text); }
```

**`prefers-reduced-motion`** — detects whether the user has requested reduced motion (an accessibility setting for users with vestibular disorders, motion sensitivity, or who simply find animation distracting):

```css
.card { transition: transform 0.3s; }

@media (prefers-reduced-motion: reduce) {
  .card { transition: none; }
  /* or better: reduce intensity rather than eliminate entirely */
}
```

**Design approach:** treat both as defaults to respect, not edge cases to bolt on later — design the dark theme alongside the light theme from the start (via custom properties, as shown), and audit all animations/transitions to ensure a reduced-motion path exists (either disabling entirely or using a much smaller/faster, less disorienting version). Combining `prefers-reduced-motion` with media queries is considered a baseline accessibility requirement in modern web standards (part of WCAG 2.1's success criteria on animation from interactions).

---

### 🔴 Q41. What is the difference between `:focus`, `:focus-visible`, and `:focus-within`?

**Answer:**
- **`:focus`** — matches an element while it has focus, regardless of *how* it got focus (mouse click, tap, or keyboard Tab). This means clicking a button with a mouse also triggers `:focus` styling — which many designers find visually noisy for mouse users who don't need the indicator.
- **`:focus-visible`** — matches an element only when the browser determines the focus indicator should be visible — generally, keyboard navigation (Tab), not mouse clicks. This is the modern fix for the classic "ugly focus ring on every button click" complaint, while still preserving the focus ring for keyboard users who genuinely need it.
- **`:focus-within`** — matches a *parent* element if any descendant currently has focus — useful for highlighting an entire form group or card when one of its inputs is focused, without needing JS to track and toggle a class.

```css
button:focus { outline: none; }               /* remove for all focus types — bad for a11y alone */
button:focus-visible { outline: 2px solid blue; } /* only show for keyboard nav — good */

.form-group:focus-within { border-color: blue; }
```

**Practical rule:** never do `outline: none` alone — it removes the focus indication entirely (an accessibility violation). Always pair removal with a `:focus-visible` replacement so keyboard users retain a clear indicator while mouse users get a cleaner interaction.

---

### 🔴 Q42. How does CSS specificity interact with `!important` and cascade layers together?

**Answer:**
The full modern cascade priority order, from highest to lowest:

1. `!important` in a **user** stylesheet (browser extension/accessibility override) — extremely rare in practice
2. `!important` declared in an **earlier** cascade layer — counterintuitively, `!important` *reverses* layer order: an `!important` in an earlier layer beats an `!important` in a later layer
3. `!important` in unlayered author CSS
4. **Normal** (non-`!important`) declarations in the **last** declared layer
5. Normal declarations working **backward** through earlier layers
6. **Unlayered normal CSS** — sits below all layered normal CSS in priority (a common surprise: *any* layer, even an early one, beats unlayered CSS for normal declarations, regardless of specificity)
7. Browser default (user-agent) styles

**The critical, frequently-misunderstood point:** `!important` flips the layer priority order for that specific declaration. If you have `@layer reset, components;` and both declare the same property with `!important`, the reset layer's `!important` wins — because layers are processed in reverse for `!important` declarations specifically. This is intentional (letting a "reset" or "base" layer's important overrides act as a hard floor that later layers can't casually override), but it's a very easy trap to fall into if you assume `!important` behaves identically regardless of layer position.

**Practical guidance:** avoid mixing `!important` and layers unless you specifically understand and intend this reversal — for most codebases, minimizing `!important` altogether and relying on layer order + reasonable specificity is far more predictable and maintainable.

---

### 🔴 Q43. What are CSS color functions like `oklch()`/`lab()`, and why are they replacing `rgb()`/`hsl()`?

**Answer:**
`oklch()` and `lab()` are newer color spaces designed to be *perceptually uniform* — meaning equal numeric changes produce equal perceived changes in color, which `rgb()` and `hsl()` don't reliably do:

```css
.button { background: oklch(60% 0.15 250); } /* lightness, chroma, hue */
```

**Problems with `hsl()`:** two colors with the same "lightness" value in `hsl()` can look very different in actual perceived brightness depending on hue — e.g., `hsl(60, 100%, 50%)` (yellow) looks much brighter to the human eye than `hsl(240, 100%, 50%)` (blue) at the same declared lightness. This makes building consistent color scales (e.g., a systematic light-to-dark ramp for a design system) unreliable with `hsl()`.

**`oklch()` fixes this:** its lightness (`L`) value corresponds to actual perceived brightness consistently across all hues — so generating a color scale by just changing the `L` value produces visually even steps, which `hsl()` can't guarantee.

**Wider gamut:** `oklch()`/`lab()` can represent colors outside the traditional sRGB gamut (used by `rgb()`/`hsl()`), accessing more vivid colors available on modern wide-gamut displays (P3 displays, common on newer phones/monitors).

**Practical impact:** color scale generation for design systems, better gradient interpolation (gradients in `oklch()` avoid the "muddy gray" midpoint problem common in `rgb()` gradients between distant hues), and future-proofing for wide-gamut displays. Browser support is now solid in all major browsers, making this a genuinely production-viable upgrade for teams building design systems today.

---

### 🔴 Q44. What is critical CSS, and how do you extract/inline it for performance?

**Answer:**
**Critical CSS** is the minimal subset of CSS needed to render the *above-the-fold* content — what the user sees before scrolling — extracted and inlined directly in the `<head>` so the page can paint immediately without waiting for an external stylesheet to download.

**Why it matters:** external `<link rel="stylesheet">` is render-blocking — the browser won't paint *anything* until the full CSS file downloads and parses, even if 90% of that CSS is for content far below the fold. Critical CSS breaks this bottleneck for the initial paint.

**Typical implementation pattern:**

```html
<head>
  <style>
    /* Inlined critical CSS — just enough for above-the-fold content */
    body { margin: 0; font-family: sans-serif; }
    .header { display: flex; padding: 16px; }
    .hero { height: 60vh; background: #f5f5f5; }
  </style>
  <link rel="preload" href="main.css" as="style" onload="this.rel='stylesheet'">
  <noscript><link rel="stylesheet" href="main.css"></noscript>
</head>
```

The `rel="preload"` + `onload` swap trick loads the full stylesheet non-render-blocking, then activates it once loaded — avoiding a Flash of Unstyled Content while not blocking initial paint.

**Extraction tools:** `critical` (npm package), Critters (used internally by some Next.js/Angular build tooling), or manual extraction for simpler sites. These tools typically render the page in a headless browser, determine what's actually visible in the initial viewport, and extract only those matching CSS rules.

**Trade-off:** adds build complexity (needs to be regenerated whenever above-the-fold markup/styles change) and duplicates a small amount of CSS (inlined + in the main file) — generally worth it for content-heavy, performance-sensitive pages (marketing sites, blogs) but often unnecessary for CSS already small/fast enough or heavily cached across page views (SPA-style apps where the visitor already has the CSS cached from a previous page).

---

### 🔴 Q45. What is the difference between CSS Modules, CSS-in-JS, and Shadow DOM scoping?

**Answer:**
All three solve the same core problem — CSS scoping/isolation, avoiding global class name collisions in component-based apps — but via very different mechanisms.

**CSS Modules — a build-time tool.** You write normal `.css` files, but the build process (webpack, Vite, etc.) automatically generates unique class names (hashes) per file and provides a JS mapping object to reference them:

```css
/* button.module.css */
.button { background: blue; }
```
```js
import styles from './button.module.css';
<button className={styles.button}> // → "button_a3f8x"
```

No runtime cost — it's plain CSS output, scoping happens entirely at build time via renamed classes.

**CSS-in-JS (styled-components, Emotion)** — styles are written inside JavaScript, often as tagged template literals, and generated/injected into the page at runtime (though some modern tools like vanilla-extract or Panda CSS shift this back to build-time / zero-runtime for performance):

```js
const Button = styled.button`
  background: blue;
  &:hover { background: darkblue; }
`;
```

Advantage: dynamic styles based on props/state are trivial (`background: ${props => props.primary ? 'blue' : 'gray'}`). Downside: runtime style injection has a real performance cost (style recalculation on every render in older implementations), though this has improved significantly with newer zero-runtime approaches.

**Shadow DOM scoping (native browser feature, used by Web Components and Angular's `ViewEncapsulation.ShadowDom`)** — creates a genuinely isolated DOM subtree with its own style boundary — styles inside a shadow root cannot leak out, and outside styles cannot leak in (with a few deliberate exceptions like CSS custom properties, which do pierce shadow boundaries by design):

```js
class MyButton extends HTMLElement {
  connectedCallback() {
    this.attachShadow({ mode: 'open' });
    this.shadowRoot.innerHTML = `<style>button{background:blue;}</style><button><slot></slot></button>`;
  }
}
```

**Comparison:** CSS Modules and CSS-in-JS both achieve scoping via naming/class generation — styles still ultimately live in the same global stylesheet/DOM, just with unique enough names to avoid collision. Shadow DOM achieves true browser-level isolation — genuinely separate style computation, not just naming tricks — which is more robust but also harder to theme from outside (requires CSS custom properties or `::part()` to intentionally expose styling hooks) and has broader implications for how the component interacts with global styles, focus, and events.