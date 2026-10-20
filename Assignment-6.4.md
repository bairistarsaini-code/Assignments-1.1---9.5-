Assignment 6.4 — Positioning Practice
What to build: A webpage with a floating action button and a sticky navigation bar.
Steps:

1. Create a webpage with multiple scrollable sections.
2. Keep the navigation bar at the top using `position: sticky`.
3. Give a floating contact/help button `position: fixed`.
4. Place a badge inside a card using `position: absolute`.
5. Apply the appropriate `position: relative` to the parent element.
6. Control the order of overlapping elements using `z-index`.
Submission: Working webpage and a screenshot showing the sticky navbar, floating button, and positioned badge.

---

## Answer / Implementation

**Plan:** Use `sticky` for the navbar, `fixed` for the help button, `relative` on the card, and `absolute` on its badge. `z-index` controls stacking order.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.navbar { position: sticky; top: 0; z-index: 10; background: #173b70; color: white; padding: 1rem; }
.card { position: relative; padding: 2rem; }
.badge { position: absolute; top: .5rem; right: .5rem; }
.help { position: fixed; right: 1rem; bottom: 1rem; z-index: 20; }
section { min-height: 70vh; padding: 2rem; }
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
