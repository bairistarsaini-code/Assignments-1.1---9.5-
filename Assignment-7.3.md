Assignment 7.3 — Responsive Product Listing
What to build: A responsive product listing of product cards.
Steps:

1. Create at least 6 product cards.
2. Add an image, name, price, and button to each card.
3. Use `display: flex` and `flex-wrap: wrap` on the container.
4. Add spacing between cards using `gap`.
5. Experiment with `flex-grow`, `flex-shrink`, and `flex-basis`.
6. Cards should wrap to the next line when the screen gets smaller.
Submission: Responsive product listing and screenshots at desktop and mobile widths.

---

## Answer / Implementation

**Plan:** Create six cards with image, product name, price, and button. `flex: 1 1 220px` allows cards to grow, shrink, and wrap.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.products { display: flex; flex-wrap: wrap; gap: 1rem; }
.product { flex: 1 1 220px; min-width: 0; padding: 1rem; border: 1px solid #ddd; border-radius: 12px; }
.product img { width: 100%; height: 180px; object-fit: cover; }
button { cursor: pointer; }
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
