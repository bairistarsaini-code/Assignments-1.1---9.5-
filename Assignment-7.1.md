Assignment 7.1 — Responsive Navigation Bar
What to build: A horizontal navigation bar using Flexbox.
Steps:

1. Create a header containing a logo and navigation links.
2. Apply `display: flex` to the container.
3. Set spacing between items using `justify-content`.
4. Align vertically using `align-items`.
5. Style the navigation links and button.
6. Inspect the layout by changing the browser width.
Submission: Working navigation bar and CSS code.

---

## Answer / Implementation

**Plan:** Use a flex container for logo and links. At mobile width, stack the items using a media query and verify no links overflow.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.navbar { display: flex; justify-content: space-between; align-items: center; gap: 1rem; padding: 1rem; }
.nav-links { display: flex; flex-wrap: wrap; gap: 1rem; }
@media (max-width: 600px) { .navbar { flex-direction: column; } }
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
