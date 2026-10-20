Assignment 9.4 — Responsive Landing Page: Build
What to build: Create an initial version of a landing page based on a given reference design.
Steps:

1. Identify colors, typography, images, and layout in the reference design.
2. Create `index.html`, `style.css`, and an `images` folder in the project folder.
3. Create semantic sections in HTML.
4. Build the structure for the navbar, hero section, buttons, and feature cards.
5. Implement the desktop layout in CSS.
6. Use Grid and Flexbox appropriately.
7. Complete base styling and spacing.
8. Push the code to GitHub.
Submission: Initial desktop version of the landing page, HTML/CSS files, and GitHub link.

---

## Answer / Implementation

**Plan:** Build the initial desktop landing page with semantic sections, navigation, hero, CTA, feature cards, and images. Keep assets in an `images` folder and push the project to GitHub.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.container { width: min(1100px, 92%); margin-inline: auto; }
header { display: flex; align-items: center; justify-content: space-between; gap: 1rem; padding: 1.25rem 0; }
.hero { display: grid; grid-template-columns: 1.1fr .9fr; align-items: center; gap: 2rem; padding: 4rem 0; }
.hero img { width: 100%; height: auto; }
.features { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 1rem; }
@media (max-width: 700px) { header, .hero { display: flex; flex-direction: column; align-items: flex-start; } .features { grid-template-columns: 1fr; } }
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
