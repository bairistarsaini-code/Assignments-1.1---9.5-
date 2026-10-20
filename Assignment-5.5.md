Assignment 5.5 — CSS Fundamentals Mini-Project
What to build: Style the multi-page college club website from Week 4.
Steps:

1. Use external CSS.
2. Choose a consistent color palette and typography.
3. Style navigation, headings, paragraphs, and buttons.
4. Make forms and tables readable.
5. Use CSS selectors and variables.
6. Debug styling issues using DevTools.
7. Keep CSS clean and reusable.
Submission: Styled multi-page website, all CSS files, and a 4–5 line explanation of design choices.

---

## Answer / Implementation

**Plan:** Use the same external stylesheet across pages. The shared palette and spacing variables make the club website consistent; test forms and tables on mobile.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
:root { --brand: #174a7e; --accent: #f0a202; --surface: #f5f7fa; }
body { margin: 0; font: 16px/1.6 Arial, sans-serif; background: var(--surface); }
nav { display: flex; flex-wrap: wrap; gap: 1rem; background: var(--brand); padding: 1rem; }
nav a { color: white; }
main { max-width: 1000px; margin: auto; padding: 1rem; }
button { background: var(--accent); border: 0; padding: .75rem 1rem; border-radius: .4rem; }
input, select { max-width: 100%; padding: .6rem; }
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
