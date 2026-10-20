Assignment 1.2 — Development Environment Setup
Task: Set up the web development environment on your computer.
What to do:

1. Install Visual Studio Code.
2. Install the LTS version of Node.js.
3. Install the Live Server and Prettier extensions in VS Code.
4. Create a folder named: web-development-practice.
5. Create index.html, style.css, and script.js files inside the folder.
6. Run the HTML file in the browser using Live Server.
7. Verify the installation by running `node -v` and `npm -v` commands in the terminal.
Submission: Screenshots of VS Code, Node.js version, and the running HTML page in the browser.

---

## Answer / Setup Steps

1. Install Visual Studio Code and the current Node.js LTS release from their official websites.
2. In VS Code Extensions, install **Live Server** and **Prettier – Code formatter**.
3. Create `web-development-practice` and add `index.html`, `style.css`, and `script.js`.
4. Open `index.html`, right-click and choose **Open with Live Server**.
5. In VS Code → Terminal → New Terminal, run:

```bash
node -v
npm -v
```

Both commands should print version numbers. Save screenshots of the project files, version output, and running browser page.

**index.html**
```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Web Development Practice</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <main class="card">
    <h1>Welcome to Web Development</h1>
    <p>My development environment is ready.</p>
    <button id="hello">Click me</button>
    <p id="message"></p>
  </main>
  <script src="script.js"></script>
</body>
</html>
```

**style.css**
```css
body { font-family: Arial, sans-serif; background: #eef2ff; }
.card { max-width: 600px; margin: 15vh auto; padding: 2rem; text-align: center; background: white; border-radius: 12px; }
button { padding: .7rem 1rem; cursor: pointer; }
```

**script.js**
```js
document.querySelector("#hello").addEventListener("click", () => {
  document.querySelector("#message").textContent = "JavaScript is working!";
});
```
