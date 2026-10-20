Assignment 6.3 — Overflow & Layout Fixing
What to build: A scrollable content box and a fixed-size container.
Steps:

1. Create a container with a fixed height.
2. Add enough text inside it so that the content overflows the container.
3. Test `overflow: visible`, `hidden`, `auto`, and `scroll`.
4. Use `overflow: auto` in a second container.
5. Identify and fix an overflow issue in a sample page.
Submission: An example of each overflow value and a screenshot of the fixed layout.

---

## Answer / Implementation

**Plan:** `visible` lets content spill out, `hidden` clips it, `auto` adds scrolling only when needed, and `scroll` provides scrollbars. Prefer `auto` for long content boxes.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.overflow-box { height: 120px; width: 260px; border: 2px solid #2457c5; margin: 1rem; }
.visible { overflow: visible; } .hidden { overflow: hidden; }
.auto { overflow: auto; } .scroll { overflow: scroll; }
.container { max-width: 100%; overflow-wrap: anywhere; }
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
