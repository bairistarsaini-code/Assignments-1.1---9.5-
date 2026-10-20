Assignment 5.2 — CSS Selectors Practice
What to build: A webpage using different CSS selectors properly.
Steps:

1. Create at least 5 HTML elements.
2. Style headings or paragraphs using an element selector.
3. Style multiple cards or sections using a class selector.
4. Style a specific section using an ID selector.
5. Use the universal selector `*` appropriately.
6. Use a grouping selector.
7. Create two conflicting CSS rules and observe the result of cascade and specificity.
Submission: HTML file, CSS file, and a short explanation of the selectors used.

---

## Answer / Implementation

**Plan:** The universal selector targets all elements, element selectors target tags, class selectors can be reused, IDs should be unique, and grouping applies shared declarations. When specificity ties, the later rule wins.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
* { box-sizing: border-box; }
body { font-family: Arial, sans-serif; }
h1 { color: navy; }                 /* element selector */
.card { padding: 1rem; border: 1px solid #bbb; } /* class selector */
#featured { background: #eef5ff; }  /* ID selector */
h1, h2, p { line-height: 1.5; }     /* grouping selector */
p { color: #444; }
.card p { color: #12643b; }         /* more specific rule wins */
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
