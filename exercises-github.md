# Hands-on Exercises

## Exercise 2: Update the Remote Repository (15 minutes)

### Goal

Modify your project locally and publish the changes to GitHub.

### Tasks

Open **README.md** and add:

```markdown
## Team Members

Your Name

Institution
```

Then run:

```bash
git status
git add .
git commit -m "Add author information"
git push
```

Refresh your GitHub repository in your web browser.

### Expected Outcome

You should see:

- A new commit on GitHub
- An updated `README.md` containing your author information

---

## Exercise 3: Clone Your Repository (15 minutes)

### Goal

Create a second copy of your repository from GitHub.

### Tasks

1. Create a new directory **outside** your original project.
2. Clone your repository:

```bash
git clone https://github.com/USERNAME/healthcare-analysis.git
```

3. Compare the two folders:

- Original repository
- Cloned repository

### Discussion

Ask participants:

- Do both repositories contain the same files?
- Do they have the same commit history?
- Are the commits identical?

Then verify by running:

```bash
git log --oneline
```

### Expected Outcome

Both repositories should contain **identical commit histories**.

---

# Mini Challenge (10 minutes)

Complete the following **without step-by-step instructions**:

- Create a file named `datasets.md`
- Document three healthcare datasets you are familiar with
- Commit your changes
- Push the commit to GitHub
- Open the repository in your browser and verify the file appears

> **Hint:** If you're unsure what Git expects next, use:

```bash
git status
```

---

# Real Research Scenario

Imagine a genomics research team working on the same project:

- **Alice** writes the data-cleaning script.
- **Brian** develops the analysis pipeline.
- **Carol** prepares the project documentation.

Each researcher works on their own computer, commits changes locally, and pushes them to GitHub.

GitHub becomes the **shared source of truth**, while Git preserves the complete history of every contribution. This workflow enables collaboration, transparency, and reproducibility, making it the standard approach for both research and software development.

---

# Reflection Questions

### Why do we still need Git if we have GitHub?

Git tracks project history locally. GitHub simply hosts Git repositories online for sharing and collaboration.

---

### What happens if you make commits but never push?

The commits exist only on your computer. No one else can see them until they are pushed.

---

### Can someone else see your local commits?

No. Local commits remain private until they are pushed to a remote repository.

---

### What is the difference between `clone` and `pull`?

- `git clone` creates a new local copy of a remote repository.
- `git pull` updates an existing local repository with the latest remote changes.

---

### Why is GitHub valuable for research teams?

GitHub makes it easy to share code, collaborate, review changes, and maintain a complete, transparent project history.

---

# Looking Ahead

Today you learned how to publish your work to GitHub and keep local and remote repositories in sync.

In the next session, you'll learn how multiple people can work on the same project using:

- Branches
- Merge conflicts
- Pull requests

These are the core collaboration tools used in both open-source software and modern research projects.