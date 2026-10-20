Assignment 4.2 — Job Application Form
What to build: A job application form using different input types.
Required fields:

1. Full name, email, and phone.
2. Date input for date of birth.
3. URL input for portfolio URL.
4. Radio buttons for gender or preferred shift.
5. Checkboxes for skills.
6. Dropdown for qualification or job role.
7. `<textarea>` for cover letter.
8. Submit button.
Rules:
- Every field must have a label.
- Make appropriate fields required.
- Add an example of a disabled field as well.
- Keep the same name for related options in radio buttons.
Submission: Complete job application form and screenshot.

---

## Answer / Implementation

**Approach:** Job application form. Create the file(s) requested in the task, paste/adapt the example, save, and open the HTML page in a browser. Replace sample personal details and image paths with your own. Check all links and required fields before taking the submission screenshot.

```html
<form><label for="name">Full name</label><input id="name" name="name" required><label for="email">Email</label><input id="email" name="email" type="email" required><label for="role">Role</label><select id="role" name="role"><option>Frontend Developer</option><option>Designer</option></select><label><input type="radio" name="work-type" value="full-time"> Full-time</label><label><input type="radio" name="work-type" value="internship"> Internship</label><label for="resume">Resume</label><input id="resume" type="file" name="resume"><input type="text" value="Application ID assigned by office" disabled><button>Submit application</button></form>
```

**Verification:** Open the page in Chrome, test links or form controls, and capture the completed page. For HTML validation, fix missing closing tags, duplicate IDs, missing `alt` text, and invalid nesting.
