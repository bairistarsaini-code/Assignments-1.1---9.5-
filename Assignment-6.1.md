Assignment 6.1 — Box Model Inspection
What to build: A webpage to inspect and modify the box models of different elements.
Steps:

1. Create 3 cards or boxes.
2. Add a heading and a paragraph to each box.
3. Apply different padding, border, and margin to each box.
4. Observe the difference between `box-sizing: content-box` and `box-sizing: border-box`.
5. Inspect the box model diagram in Chrome DevTools.
6. Take a screenshot and label the parts of the box model.
Submission: HTML, CSS, and an annotated screenshot explaining content, padding, border, and margin.

---

## Answer / Implementation

**Plan:** The box model consists of content, padding, border, and margin. `content-box` adds padding and border outside the declared width; `border-box` includes them inside the width.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.box { width: 260px; padding: 20px; border: 4px solid #2457c5; margin: 16px; }
.content-box { box-sizing: content-box; }
.border-box { box-sizing: border-box; }
* { box-sizing: border-box; }
/* content → padding → border → margin */
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
