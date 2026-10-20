Assignment 2.4 — HTML Validation & Debugging
Task: Debug a intentionally buggy HTML file.
What to do:

1. Take a sample HTML file containing missing closing tags, incorrect nesting, and missing attributes.
2. Identify the errors.
3. Inspect using the Elements panel in browser DevTools.
4. Check the markup using an HTML validation tool.
5. Fix all errors and properly indent the code.
Submission: Before-and-after code and a screenshot of the fixed webpage.

---

## Answer / Implementation

**Approach:** Validated HTML. Create the file(s) requested in the task, paste/adapt the example, save, and open the HTML page in a browser. Replace sample personal details and image paths with your own. Check all links and required fields before taking the submission screenshot.

```html
<!doctype html>
<html lang="en">
<head><meta charset="UTF-8"><title>Validated Page</title></head>
<body><h1>Correct Heading</h1><p>Every opened element is properly closed.</p><a href="https://example.com">Example link</a></body>
</html>
```

**Verification:** Open the page in Chrome, test links or form controls, and capture the completed page. For HTML validation, fix missing closing tags, duplicate IDs, missing `alt` text, and invalid nesting.
