Assignment 1.4 — Git Essentials I
Task: Convert a local project into a Git repository.
What to do:

1. Install Git and verify with `git --version`.
2. Open the terminal in the project folder.
3. Run `git init`.
4. Configure your Git username and email.
5. Create an HTML file.
6. Use `git status`, `git add`, and `git commit`.
7. Make at least 3 meaningful commits.
Submission: Screenshots of the repository folder and the history of three commits.

---

## Answer / Git Commands

From the project folder, run:

```bash
git --version
git init
git status
git add .
git commit -m "Initial project commit"
git log --oneline
```

`git init` creates a local repository, `git add .` stages changes, and `git commit` saves a snapshot. If Git asks for identity, configure it with `git config --global user.name "Your Name"` and `git config --global user.email "you@example.com"`. Take screenshots of `git status` and the commit.
