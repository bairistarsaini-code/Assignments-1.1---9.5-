Assignment 1.1 — How a Website Works
Task: Explain in a single paragraph how a website opens on the screen after typing a URL.
What to do:

1. Understand the basic roles of browser, client, server, and database.
2. Write the meanings of HTTP and HTTPS.
3. Explain the request-response cycle.
4. Write the differences between a static and a dynamic website.
5. Open Chrome DevTools and inspect requests in the Network tab of any website.
Submission: An explanatory paragraph and a screenshot of the Network tab.

---

## Answer

A website opens when a user enters a URL in a browser. The browser (client) sends an HTTP or HTTPS request to a web server. HTTP means Hypertext Transfer Protocol; HTTPS means Hypertext Transfer Protocol Secure and encrypts data in transit. The server processes the request and may communicate with a database, then sends a response containing HTML, CSS, JavaScript, images, or data. The browser interprets these resources and displays the page; this is the request-response cycle. A static website usually serves fixed files, while a dynamic website can produce different content based on user input, application logic, or database records.

**Network inspection:** Open Chrome → press F12 → Network → reload the page. Inspect the `document` request, status code, type, and timing. Capture a screenshot of the Network tab for submission.
