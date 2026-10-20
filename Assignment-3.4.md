Assignment 3.4 — Semantic HTML & Accessibility
What to build: Convert an existing div-based webpage into semantic HTML.
Steps:

1. Structure the page using `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, and `<footer>` where appropriate.
2. Keep navigation links inside `<nav>`.
3. Keep the main content inside `<main>`.
4. Use the correct heading hierarchy.
5. Add meaningful alt text for images.
6. Check that links and page sections are understandable.
Submission: The updated semantic HTML page and before/after screenshots.

---

## Answer / Implementation

**Approach:** Semantic and accessible structure. Create the file(s) requested in the task, paste/adapt the example, save, and open the HTML page in a browser. Replace sample personal details and image paths with your own. Check all links and required fields before taking the submission screenshot.

```html
<header><h1>College Club</h1></header><nav aria-label="Main navigation"><a href="index.html">Home</a></nav><main><article><h2>Latest News</h2><p>Club activities and announcements.</p></article><aside><h2>Upcoming</h2><p>Workshop this Friday.</p></aside></main><footer><p>&copy; 2026 College Club</p></footer>
```

**Verification:** Open the page in Chrome, test links or form controls, and capture the completed page. For HTML validation, fix missing closing tags, duplicate IDs, missing `alt` text, and invalid nesting.
