Assignment 8.4 — Dashboard with Grid and Flexbox
What to build: A dashboard with an outer Grid layout and inner Flexbox cards.
Steps:

1. Create a header, sidebar, and main content in the dashboard.
2. Use CSS Grid for the outer page.
3. Add 4 statistic cards in the main area.
4. Align icons, titles, and numbers inside the cards using Flexbox.
5. Add a small table or recent activity section.
6. Check the layout using the DevTools Grid inspector.
Submission: Complete dashboard page and CSS code showing both Grid and Flexbox.

---

## Answer / Implementation

**Plan:** The outer dashboard uses Grid; each statistic card uses Flexbox to align its icon, label, and value. Inspect the grid overlay in DevTools.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.dashboard { display: grid; grid-template-columns: 220px minmax(0, 1fr); gap: 1rem; }
.stats { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 1rem; }
.stat { display: flex; align-items: center; justify-content: space-between; gap: 1rem; padding: 1rem; background: #eef5ff; }
@media (max-width: 700px) { .dashboard, .stats { grid-template-columns: 1fr; } }
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
