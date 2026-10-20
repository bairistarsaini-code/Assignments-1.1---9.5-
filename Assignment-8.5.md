Assignment 8.5 — CSS Grid Mini-Project
What to build: A complete photo-gallery website or dashboard page.
Required features:
- Header
- Main grid layout
- Multiple cards/images
- Consistent gaps
- Responsive columns
- Footer
Rules:

1. Use CSS Grid for the primary layout.
2. Use `repeat()`, `minmax()`, and `fr` units.
3. Demonstrate named grid areas or explicit grid placement.
4. Prevent overflow in images and text.
5. Test on different screen widths.
Submission: Complete Grid-based project, HTML/CSS files, and a GitHub link.

---

## Answer / Implementation

**Plan:** Include header, responsive image/card grid, and footer. `repeat()`, `minmax()`, and `fr` create flexible columns without fixed widths.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.page { display: grid; grid-template-columns: 1fr; grid-template-areas: 'header' 'main' 'footer'; gap: 1rem; }
header { grid-area: header; } main { grid-area: main; } footer { grid-area: footer; }
.gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(min(100%, 220px), 1fr)); gap: 1rem; }
.gallery img { width: 100%; height: 200px; object-fit: cover; }
.card { min-width: 0; overflow-wrap: anywhere; }
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
