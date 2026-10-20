Assignment 5.3 — Typography Showcase Page
What to build: A typography showcase webpage.
Steps:

1. Select 2 complementary font families from Google Fonts.
2. Set different fonts for heading and body text.
3. Use different font sizes and weights.
4. Apply `text-align`, `text-decoration`, and `font-style`.
5. Adjust `letter-spacing` and `line-height`.
6. Create 3 sections: Heading Styles, Paragraph Styles, and Text Emphasis.
Submission: Styled typography webpage and CSS file.

---

## Answer / Implementation

**Plan:** Use the heading font for headings and the body font for readable paragraphs. The `clamp()` value keeps heading size responsive.

Create the HTML structure with semantic elements (`header`, `nav`, `main`, `section`, `article`, `footer`) and add the following rules to `style.css`. Add matching class names to your HTML. For screenshot-based submissions, open the page in Chrome and capture the requested viewport(s).

**style.css**
```css
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;700&family=Playfair+Display:wght@700&display=swap');
body { font-family: 'DM Sans', sans-serif; line-height: 1.7; }
h1, h2 { font-family: 'Playfair Display', serif; }
h1 { font-size: clamp(2rem, 5vw, 3.5rem); text-align: center; }
.emphasis { font-style: italic; text-decoration: underline; letter-spacing: .04em; }
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
