Assignment 5.4 — CSS Variables & Design Tokens
What to build: A small design system with reusable colors and spacing variables.
Steps:

1. Define CSS variables in `:root`.
2. Set primary color, secondary color, background color, and text color.
3. Define small, medium, and large spacing variables.
4. Create font-size variables.
5. Use variables in buttons, headings, and cards.
6. Change a variable and verify that multiple elements update.
Submission: Design-token stylesheet and a sample webpage using these variables.

---

## Answer / Implementation

**Plan:** CSS custom properties declared in `:root` are reusable throughout the page. Change `--primary` once to update every component that uses it.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
:root { --primary: #2457c5; --secondary: #16a085; --bg: #f5f7fb; --text: #1f2937; --space-sm: .5rem; --space-md: 1rem; --space-lg: 2rem; --font-sm: .9rem; --font-lg: 1.5rem; }
body { background: var(--bg); color: var(--text); font-family: Arial, sans-serif; }
.card { padding: var(--space-lg); margin: var(--space-md); background: white; }
button { background: var(--primary); color: white; padding: var(--space-sm) var(--space-md); }
h1 { font-size: var(--font-lg); }
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
