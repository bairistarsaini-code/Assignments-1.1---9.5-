Assignment 8.2 — Auto-Responsive Image Gallery
What to build: An auto-responsive image gallery.
Steps:

1. Collect at least 8 images.
2. Place each image inside a gallery item.
3. Use `grid-template-columns: repeat(auto-fit, minmax(...))` on the grid.
4. Apply `width: 100%` and suitable `object-fit` for the images.
5. Keep consistent spacing using `gap`.
6. Verify that columns adjust automatically by changing the browser width.
Submission: Responsive photo gallery and desktop/mobile screenshots.

---

## Answer / Implementation

**Plan:** Add at least eight `<img>` elements with meaningful alt text. Use `auto-fit` and `minmax()` so columns resize automatically.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 1rem; }
.gallery img { display: block; width: 100%; aspect-ratio: 4 / 3; object-fit: cover; border-radius: 10px; }
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
