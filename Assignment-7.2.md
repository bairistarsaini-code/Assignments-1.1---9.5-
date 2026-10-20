Assignment 7.2 — Pricing Cards & Centered Login Form
What to build: A page with 3 aligned pricing cards and a centered login form.
Steps:

1. Create Basic, Pro, and Premium pricing cards.
2. Add price, features list, and a button to each card.
3. Use Flexbox on the parent container.
4. Align the cards using `justify-content` and `align-items`.
5. Center the login form horizontally and vertically.
6. Demonstrate the practical use of `flex-direction` and alignment properties.
Submission: Webpage with pricing cards and a centered login form.

---

## Answer / Implementation

**Plan:** Build three plan cards and a login form. Flexbox wraps pricing cards; the login form uses a column layout and centers controls.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.pricing { display: flex; justify-content: center; align-items: stretch; flex-wrap: wrap; gap: 1rem; }
.plan { flex: 1 1 220px; max-width: 300px; padding: 1.5rem; border: 1px solid #ddd; border-radius: 12px; }
.login { min-height: 60vh; display: flex; flex-direction: column; justify-content: center; align-items: center; gap: .8rem; }
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
