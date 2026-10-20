Assignment 4.1 — Student Registration Form
What to build: A student registration form.
Required fields:
- Full Name
- Email
- Password
- Phone Number
- Age
- Submit button
Steps:

1. Build the form inside a `<form>` tag.
2. Add a proper `<label>` for each field.
3. Use correct input types, such as text, email, password, and number or a suitable tel.
4. Give each input a unique id and meaningful name.
5. Add `required` on mandatory fields.
6. Complete the form with a submit button.
Submission: `registration.html` and a screenshot of the working form.

---

## Answer / Implementation

**Approach:** Student registration form. Create the file(s) requested in the task, paste/adapt the example, save, and open the HTML page in a browser. Replace sample personal details and image paths with your own. Check all links and required fields before taking the submission screenshot.

```html
<form action="#" method="post"><label for="name">Full name</label><input id="name" name="name" required><label for="email">Email</label><input id="email" name="email" type="email" required><label for="course">Course</label><select id="course" name="course" required><option value="">Choose a course</option><option>MCA</option><option>BCA</option></select><button type="submit">Register</button></form>
```

**Verification:** Open the page in Chrome, test links or form controls, and capture the completed page. For HTML validation, fix missing closing tags, duplicate IDs, missing `alt` text, and invalid nesting.
