Assignment 5.1 — Convert an HTML Page into a Styled Page
What to build: Add CSS to the HTML website from Week 4.
Steps:

1. Create a `style.css` file.
2. Link the external stylesheet in HTML.
3. Set the body background, text color, and font.
4. Style headings, paragraphs, and links.
5. Make navigation links readable and attractive.
6. Inspect styles using Chrome DevTools.
Submission: Styled version of the original HTML page and the CSS file.

---

## Answer / Implementation

**Plan:** Create `style.css`, link it with `<link rel="stylesheet" href="style.css">` inside `<head>`, and inspect rules in Chrome DevTools → Elements → Styles.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
body { margin: 0; font: 16px/1.6 Arial, sans-serif; background: #f4f7fb; color: #222; }
nav { display: flex; gap: 1rem; padding: 1rem; background: #173b70; }
nav a { color: white; text-decoration: none; }
main { max-width: 900px; margin: 2rem auto; padding: 1rem; }
h1, h2 { color: #173b70; }
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
