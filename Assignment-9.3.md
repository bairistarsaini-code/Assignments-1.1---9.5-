Assignment 9.3 — Combine Flexbox and Grid Responsively
What to build: A landing page using both CSS Grid and Flexbox.
Steps:

1. Create a header and navigation bar.
2. Arrange text and images in the hero section.
3. Add 3–6 cards in the features section.
4. Use Grid for the main section layout.
5. Use Flexbox for the navbar, card internal content, or hero alignment.
6. Convert columns into a single-column layout in mobile view.
7. Check spacing and alignment on both desktop and mobile.
Submission: Complete responsive landing page, HTML/CSS files, and screenshots.

---

## Answer / Implementation

**Plan:** Use Grid for the hero/features layout and Flexbox for navigation and card internals. Switch the hero to one column on mobile.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.navbar { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 1rem; }
.hero { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); align-items: center; gap: 2rem; }
.features { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 1rem; }
.feature { display: flex; flex-direction: column; gap: .75rem; padding: 1rem; }
img { max-width: 100%; height: auto; }
@media (max-width: 650px) { .hero { grid-template-columns: 1fr; } }
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
