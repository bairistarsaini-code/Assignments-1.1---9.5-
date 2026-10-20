Assignment 2.3 — Div, Attributes & Clean Structure
Task: Convert the previous introduction page into clean and structured HTML.
What to do:

1. Divide the page into Header, About, Education, Skills, and Contact sections.
2. Use `div` for containers.
3. Give elements unique `id` and reusable `class` attributes.
4. Add a `data-*` custom attribute to any element.
5. Update a text element and add new content.
6. Organize the HTML code with proper indentation and meaningful names.
Submission: The updated HTML file and a screenshot showing the page structure.

---

## Answer / Implementation

**Approach:** Structured HTML. Create the file(s) requested in the task, paste/adapt the example, save, and open the HTML page in a browser. Replace sample personal details and image paths with your own. Check all links and required fields before taking the submission screenshot.

```html
<main class="profile" id="profile">
  <section aria-labelledby="about-title"><h1 id="about-title">About Me</h1><p>I am learning web development.</p></section>
  <section><h2>Skills</h2><ul><li>HTML</li><li>CSS</li></ul></section>
</main>
```

**Verification:** Open the page in Chrome, test links or form controls, and capture the completed page. For HTML validation, fix missing closing tags, duplicate IDs, missing `alt` text, and invalid nesting.
