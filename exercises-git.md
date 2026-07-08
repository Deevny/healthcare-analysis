# Hands-on Exercises

## Exercise 1: Create Your First Git Repository (15 minutes)

### Goal
Create a new Git repository and make your first commit.

### Tasks

1. Create a project folder named:

```text
healthcare-analysis
```

2. Inside the folder, create two files:

```text
README.md
notes.txt
```

3. Initialize the directory as a Git repository.

4. Stage both files.

5. Create your first commit.

6. View the commit history.

### Expected Outcome

Running:

```bash
git log --oneline
```

should display **one commit**.

---

## Exercise 2: Update the Repository (15 minutes)

### Goal
Modify an existing file and record the changes.

### Tasks

Open **README.md** and add:


# Healthcare Analysis

This repository contains scripts used during the Git workshop.
```

Then:

1. Check the repository status.

```bash
git status
```

2. Stage the modified file.

3. Commit the change.

```bash
git commit -m "Add project description"
```

4. View the commit history.

```bash
git log --oneline
```

### Expected Outcome

The repository should now contain **two commits**.

---

## Exercise 3: Tracking Changes (10 minutes)

### Goal
Understand the difference between modified and staged files.

### Tasks

Edit **notes.txt** and add:

```text
Dataset:
clinical_patients.csv

Analysis:
Exploratory data analysis
```

Run:

```bash
git status
```

### Discussion

Before staging, answer the following:

- What changed?
- Is the file staged?
- What needs to happen before Git saves this version?

Then:

```bash
git add notes.txt
git commit -m "Add project notes"
```

---

# Mini Challenge (10 minutes)

Complete the following **without step-by-step instructions**:

- Create a file named `todo.txt`
- Add three tasks related to a healthcare data analysis project
- Stage the file
- Commit it using a meaningful commit message
- Display the commit history using:

```bash
git log --oneline
```

> **Instructor:** Walk around the room and provide guidance only when participants become stuck.

---

# Reflection

Discuss the following questions:

1. Why is `git status` one of the most useful Git commands?
2. What is the difference between `git add` and `git commit`?
3. What information does Git store with every commit?
4. Why are meaningful commit messages important?
5. How can Git improve reproducibility in healthcare research?

---

# Key Takeaways

By the end of today's session, you should understand that:

- Git is a **local version control system** that records the complete history of a project.
- A **repository** is simply a project managed by Git.
- The basic Git workflow is:

```text
Modify files
      ↓
git status
      ↓
git add
      ↓
git commit
```

- Commits should represent **one logical change**.
- Commit messages should clearly describe **what changed and why**.

### Looking Ahead

In the next session, you'll build on this local repository by:

- Publishing it to GitHub
- Collaborating with others
- Using Markdown to create professional project documentation