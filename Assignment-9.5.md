Assignment 9.5 — Responsive Landing Page: Finish & Review
What to build: Make the landing page from Assignment 9.4 complete, responsive, and portfolio-ready.
Steps:

1. Implement tablet and mobile breakpoints.
2. Adjust the navbar and content for small screens.
3. Make images and typography responsive.
4. Test the functionality of buttons and links.
5. Check different viewport sizes in Chrome DevTools.
6. Fix horizontal scrolling, overlapping, broken images, and spacing issues.
7. Keep HTML/CSS clean and properly formatted.
8. Push final changes to GitHub.
Submission: Final responsive landing page, desktop/tablet/mobile screenshots, and updated GitHub repository link.

---

## Answer / Implementation

**Plan:** Test all links and buttons, inspect phone/tablet/desktop widths, fix overflow and broken images, format the files, and push final changes to GitHub.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
/* Final responsive review */
* { box-sizing: border-box; }
html { scroll-behavior: smooth; }
body { margin: 0; overflow-wrap: anywhere; }
.container { width: min(1100px, 92%); margin-inline: auto; }
img { display: block; max-width: 100%; height: auto; }
.navbar { display: flex; flex-wrap: wrap; align-items: center; justify-content: space-between; gap: 1rem; }
.hero { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 2rem; align-items: center; }
.features { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 1rem; }
button, a { touch-action: manipulation; }
@media (max-width: 800px) { .hero { grid-template-columns: 1fr; } .features { grid-template-columns: repeat(2, minmax(0, 1fr)); } }
@media (max-width: 520px) { .navbar { flex-direction: column; align-items: flex-start; } .features { grid-template-columns: 1fr; } }
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
