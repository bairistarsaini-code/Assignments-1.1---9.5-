Assignment 9.1 — Convert a Desktop Page into a Mobile-First Layout
What to build: Make an existing desktop-only webpage responsive.
Steps:

1. Open the dashboard or photo gallery project from Week 8.
2. Verify the viewport meta tag in the HTML `<head>`.
3. Write CSS for mobile screens first.
4. Improve tablet and desktop layouts using media queries.
5. Add at least 2 breakpoints.
6. Test on different screen sizes using Chrome DevTools' Device Mode.
7. Fix horizontal overflow and overlapping elements.
Submission: Updated HTML/CSS files and screenshots for mobile, tablet, and desktop.

---

## Answer / Implementation

**Plan:** Start with one column for mobile and add breakpoints at 600px and 900px. Use Chrome DevTools Device Mode to test phone, tablet, and desktop.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
/* Mobile first */
.container { display: grid; grid-template-columns: 1fr; gap: 1rem; padding: 1rem; }
img { max-width: 100%; height: auto; }
@media (min-width: 600px) { .container { grid-template-columns: repeat(2, minmax(0, 1fr)); } }
@media (min-width: 900px) { .container { grid-template-columns: repeat(3, minmax(0, 1fr)); max-width: 1200px; margin: auto; } }
```

**Example HTML structure**
```html
<header class="navbar"><strong>My Website</strong><nav><a href="#home">Home</a> <a href="#features">Features</a></nav></header>
<main class="container" id="home">
  <section class="hero"><div><h1>Build Something Great</h1><p>A clean, responsive sample page.</p><a href="#features">Explore features</a></div><img src="images/hero.jpg" alt="Website project preview"></section>
  <section class="features" id="features">
    <article class="feature"><h2>Feature One</h2><p>Useful and clear content.</p></article>
    <article class="feature"><h2>Feature Two</h2><p>Responsive layout.</p></article>
    <article class="feature"><h2>Feature Three</h2><p>Accessible structure.</p></article>
  </section>
</main>
<footer>© 2026 My Website</footer>
```

**Testing and submission:** Save all files, run the page with Live Server, resize the browser, inspect with DevTools, and take the screenshots listed in the assignment. Replace example image paths and sample text with real project content.
