Assignment 7.4 — Modern Landing Page Header
What to build: A header and hero section for a modern landing page.
Steps:

1. Add a logo, navigation links, and a CTA button in the header.
2. Create a heading, paragraph, and button in the hero section.
3. Add an illustration or image.
4. Arrange the text and image side-by-side using Flexbox.
5. Properly align the hero content.
6. Style the footer or sticky section using earlier CSS concepts.
7. Check the layout at different widths.
Submission: Complete code for the landing page header + hero section.

---

## Answer / Implementation

**Plan:** Place header and hero content in flex containers. Use an image with alt text and stack the hero at smaller widths.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.site-header { display: flex; align-items: center; justify-content: space-between; gap: 1rem; padding: 1rem 5%; }
.hero { display: flex; align-items: center; justify-content: space-between; gap: 2rem; padding: 4rem 5%; }
.hero > * { flex: 1; min-width: 0; }
.hero img { max-width: 100%; height: auto; }
@media (max-width: 700px) { .hero, .site-header { flex-direction: column; } }
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
