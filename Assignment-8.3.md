Assignment 8.3 — Magazine Layout Using Grid Areas
What to build: A magazine or news-style webpage.
Steps:

1. Create header, navigation, main article, sidebar, and footer sections.
2. Define a grid container.
3. Set the layout using `grid-template-areas`.
4. Assign a named grid area to each section.
5. Give the main article more space than the sidebar.
6. Test different section sizes and alignments.
Submission: Magazine-style layout and grid-area CSS code.

---

## Answer / Implementation

**Plan:** Give each semantic section a named grid area. The main article gets a wider column than the sidebar; mobile changes to one column.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.magazine { display: grid; gap: 1rem; grid-template-columns: minmax(0, 2fr) minmax(220px, 1fr); grid-template-areas: 'header header' 'nav nav' 'article sidebar' 'footer footer'; }
header { grid-area: header; } nav { grid-area: nav; } article { grid-area: article; } aside { grid-area: sidebar; } footer { grid-area: footer; }
@media (max-width: 650px) { .magazine { grid-template-columns: 1fr; grid-template-areas: 'header' 'nav' 'article' 'sidebar' 'footer'; } }
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
