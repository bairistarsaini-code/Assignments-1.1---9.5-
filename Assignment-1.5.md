Assignment 1.5 — GitHub Essentials II
Task: Upload a local project to GitHub.
What to do:

1. Create a GitHub account or use an existing one.
2. Create a new public repository.
3. Connect the local repository to the remote repository.
4. Upload files using `git push`.
5. Add a new file and push the second commit.
6. Verify the commit history on GitHub.
Submission: The link to the public GitHub repository.

---

## Answer / Upload to GitHub

1. Create a new empty repository on GitHub (do not add a README if the local project already has one).
2. In the project terminal, use the repository URL shown by GitHub:

```bash
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

Replace the example URL with your own repository URL. If `origin` already exists, check it with `git remote -v` and update it with `git remote set-url origin YOUR-REPOSITORY-URL`. Verify the files appear on GitHub and submit the repository link. Never share a password or access token in the assignment.
