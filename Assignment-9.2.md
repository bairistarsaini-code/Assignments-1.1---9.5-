Assignment 9.2 — Responsive Typography & Images
What to build: A webpage where text and images adjust properly across different screen sizes.
Steps:

1. Create an article or portfolio page.
2. Add headings, paragraphs, and images.
3. Use `rem`, `em`, or `clamp()` for font sizes.
4. Apply `max-width: 100%` and `height: auto` to images.
5. Set a suitable `max-width` on the content container.
6. Improve line length and spacing for mobile and desktop.
7. Check that images do not stretch and text does not overflow the screen.
Submission: Responsive webpage and mobile/desktop screenshots.

---

## Answer / Implementation

**Plan:** Use `clamp()` for responsive type, a readable content width, and `max-width: 100%; height: auto` for images.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
body { font-family: Arial, sans-serif; line-height: 1.7; }
article { width: min(100% - 2rem, 70ch); margin-inline: auto; }
h1 { font-size: clamp(2rem, 5vw, 3.5rem); line-height: 1.15; }
p { font-size: clamp(1rem, 1.5vw, 1.125rem); }
img { display: block; max-width: 100%; height: auto; }
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
