Assignment 6.5 — Profile Card / Product Card Mini-Project
What to build: A complete profile card or product card component.
Profile card must include:
- Profile image
- Name and role
- Short description
- Skills
- Contact button
Product card must include:
- Product image
- Product name
- Price
- Short description
- Buy button
Rules:

1. Use box model properties.
2. Add background, border, and `border-radius`.
3. Place a badge or button using positioning.
4. Keep CSS class names meaningful.
5. Test the card on different screen widths.
Submission: Finished card component, HTML/CSS files, and a screenshot.

---

## Answer / Implementation

**Plan:** Include a local image with descriptive alt text, name, role, description, skills, and contact button. Test the card at narrow and wide viewport widths.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
.profile-card { position: relative; box-sizing: border-box; width: min(360px, 100%); margin: 2rem auto; padding: 1.5rem; text-align: center; border: 1px solid #ddd; border-radius: 18px; background: white; box-shadow: 0 8px 24px #0001; }
.profile-card img { width: 100px; height: 100px; border-radius: 50%; object-fit: cover; }
.profile-card .badge { position: absolute; top: 1rem; right: 1rem; }
button { padding: .7rem 1rem; cursor: pointer; }
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
