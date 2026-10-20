Assignment 7.5 — Flexbox Mini-Project
What to build: A complete responsive landing page.
Required sections:
- Navigation bar
- Hero section
- 3 feature cards
- Call-to-action section
- Footer
Rules:

1. Use Flexbox in the navbar and hero layout.
2. Arrange feature cards in a responsive row.
3. Use `gap`, `justify-content`, `align-items`, and `flex-wrap`.
4. Keep colors, typography, and spacing consistent.
5. Content should not overflow on smaller screens.
Submission: Complete landing page, HTML/CSS files, and a GitHub repository link.

---

## Answer / Implementation

**Plan:** Add navbar, hero, three feature cards, CTA, and footer. Reuse spacing and colors and verify mobile layout.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.navbar, .hero, .features { display: flex; align-items: center; justify-content: space-between; gap: 1rem; }
.features { flex-wrap: wrap; }
.feature { flex: 1 1 220px; padding: 1.5rem; border-radius: 12px; background: #f1f5f9; }
.hero { padding: 4rem 5%; }
@media (max-width: 650px) { .navbar, .hero { flex-direction: column; text-align: center; } }
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
