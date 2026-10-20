Assignment 4.3 — Student Marks Table
What to build: A student marksheet table.
Steps:

1. Add data for at least 5 students and 3 subjects.
2. Use `<table>`, `<tr>`, `<th>`, and `<td>` for the table.
3. Organize the table into `<thead>`, `<tbody>`, and `<tfoot>`.
4. Give a title to the table using `<caption>`.
5. Show total or average marks in the footer.
6. Use `colspan` or `rowspan` where appropriate.
7. Keep table headers meaningful.
Submission: `marksheet.html` and a screenshot of the complete table.

---

## Answer / Implementation

**Approach:** Student marks table. Create the file(s) requested in the task, paste/adapt the example, save, and open the HTML page in a browser. Replace sample personal details and image paths with your own. Check all links and required fields before taking the submission screenshot.

```html
<table><caption>Student Marksheet</caption><thead><tr><th>Student</th><th>HTML</th><th>CSS</th><th>JavaScript</th><th>Total</th></tr></thead><tbody><tr><td>Asha</td><td>80</td><td>85</td><td>78</td><td>243</td></tr><tr><td>Ravi</td><td>75</td><td>82</td><td>80</td><td>237</td></tr><tr><td>Neha</td><td>90</td><td>88</td><td>92</td><td>270</td></tr><tr><td>Aman</td><td>70</td><td>76</td><td>74</td><td>220</td></tr><tr><td>Sana</td><td>86</td><td>91</td><td>89</td><td>266</td></tr></tbody><tfoot><tr><th colspan="4">Class total</th><td>1236</td></tr></tfoot></table>
```

**Verification:** Open the page in Chrome, test links or form controls, and capture the completed page. For HTML validation, fix missing closing tags, duplicate IDs, missing `alt` text, and invalid nesting.
