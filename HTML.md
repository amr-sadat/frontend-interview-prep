# 🚀 HTML Interview Preparation Guide
> 🟢 Easy | 🟡 Medium | 🔴 Advanced

---

## Table of Contents
- [🟢 Q1 - What is the difference between `<section>`, `<article>`, `<aside>`, and `<div>`?](#q1-what-is-the-difference-between-section-article-aside-and-div)
- [🟢 Q2 - What are semantic HTML elements and why are they important?](#q2-what-are-semantic-html-elements-and-why-are-they-important)
- [🟢 Q3 - What is the purpose of the `meta viewport` tag?](#q3-what-is-the-purpose-of-the-meta-viewport-tag)
- [🟢 Q4 - What is the difference between `async` and `defer` on script tags?](#q4-what-is-the-difference-between-async-and-defer-on-script-tags)
- [🟢 Q5 - What is the difference between `<input type="button">` and `<button>`?](#q5-what-is-the-difference-between-input-typebutton-and-button)

---

### Q1. What is the difference between `<section>`, `<article>`, `<aside>`, and `<div>`?

**Answer:**
- **`<section>`** — A thematic grouping of content, typically with a heading. Used for chapters, tabbed content, or numbered sections.
- **`<article>`** — Self-contained content that could be distributed independently (blog post, news article, comment).
- **`<aside>`** — Content tangentially related to the main content (sidebar, pull quote, advertising).
- **`<div>`** — A generic, non-semantic block container with no inherent meaning. Use it only when no semantic element fits.

> **Key rule:** If removing the element would make the page harder to understand for screen readers, use a semantic element. If it's purely for layout/styling, use `<div>`.

---

### Q2. What are semantic HTML elements and why are they important?

**Answer:**
Semantic HTML elements clearly describe their meaning to both the browser and the developer. Examples: `<header>`, `<nav>`, `<main>`, `<footer>`, `<article>`, `<section>`, `<figure>`, `<time>`.

**Why they matter:**
1. **Accessibility** — Screen readers use semantic elements to build the accessibility tree and help users navigate.
2. **SEO** — Search engines better understand and rank page content.
3. **Maintainability** — Code is self-documenting and easier to read.
4. **Browser defaults** — Some elements carry built-in behaviour (e.g., `<button>` is keyboard-focusable by default).

---

### Q3. What is the purpose of the `meta viewport` tag?

**Answer:**
```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```
Without it, mobile browsers render the page at a typical desktop width (~980px) and then scale it down, making text tiny. The viewport meta tag tells the browser to:
- Set the viewport width to the device's actual screen width (`width=device-width`).
- Use a 1:1 zoom ratio (`initial-scale=1`).

This is required for CSS media queries to work correctly on mobile devices.

---

### Q4. What is the difference between `async` and `defer` on script tags?

**Answer:**

| | `async` | `defer` |
|---|---|---|
| Download | Parallel with HTML parsing | Parallel with HTML parsing |
| Execution | Immediately when downloaded (pauses parsing) | After HTML is fully parsed |
| Order | Not guaranteed | Preserved (DOMContentLoaded order) |
| Use case | Independent scripts (analytics, ads) | Scripts that depend on the DOM |

**Rule of thumb:** Prefer `defer` for application scripts; use `async` only for truly independent third-party scripts.

---

### Q5. What is the difference between `<input type="button">` and `<button>`?

**Answer:**
- **`<input type="button">`** — Self-closing, content set via `value` attribute, cannot contain HTML markup.
- **`<button>`** — Can contain HTML (icons, spans, images), supports `type="submit"`, `type="reset"`, `type="button"`. More flexible and semantic.

Default `type` for `<button>` is **`submit`** when inside a form, which is a common gotcha.

---