Assignment 8.1 — Dashboard-Style Grid Layout
What to build: A basic dashboard using CSS Grid.
Steps:

1. Create the dashboard header.
2. Create a sidebar and main content area.
3. Add 3 or 4 statistic cards in the main content.
4. Use `display: grid` for the outer layout.
5. Set `grid-template-columns` and `grid-template-rows`.
6. Use gaps between cards.
7. Inspect the grid layout in the browser.
Submission: Dashboard webpage and CSS file.

---

## Answer / Implementation

**Plan:** Use Grid for sidebar and content, then a nested responsive grid for statistic cards. The media query collapses the sidebar layout on mobile.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.dashboard { display: grid; grid-template-columns: 220px minmax(0, 1fr); grid-template-rows: auto 1fr; min-height: 100vh; }
.header { grid-column: 1 / -1; padding: 1rem; background: #173b70; color: white; }
.sidebar { padding: 1rem; background: #eef2f7; }
.stats { display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 1rem; padding: 1rem; }
.stat { padding: 1.5rem; background: white; border: 1px solid #ddd; border-radius: 10px; }
@media (max-width: 650px) { .dashboard { grid-template-columns: 1fr; } }
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
