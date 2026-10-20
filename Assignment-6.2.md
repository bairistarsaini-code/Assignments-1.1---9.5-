Assignment 6.2 — Backgrounds, Borders & Display
What to build: 3 different card designs on a webpage.
Steps:

1. Create 3 cards, such as Basic, Standard, and Premium.
2. Add a title, description, and button to each card.
3. Keep background colors and borders distinct.
4. Create rounded corners using `border-radius`.
5. Demonstrate `display: block`, `inline`, and `inline-block` with practical examples.
6. Set width, height, and `max-width`.
Submission: 3 differently styled cards and the CSS file.

---

## Answer / Implementation

**Plan:** Use three cards with distinct classes and demonstrate block, inline, and inline-block on sample labels. `max-width: 100%` prevents cards from exceeding narrow screens.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.cards { display: flex; flex-wrap: wrap; gap: 1rem; }
.card { width: 240px; max-width: 100%; padding: 1.2rem; border: 2px solid #2457c5; border-radius: 14px; background: #eef5ff; }
.block { display: block; }
.inline { display: inline; }
.inline-block { display: inline-block; width: 120px; }
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
