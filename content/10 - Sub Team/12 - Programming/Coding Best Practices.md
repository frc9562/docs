---
title: Coding Best Practices
aliases:
created: 2026/01/15
modified: 2026-01-15T19:36:18-05:00
tags:
  - programming
draft: false
---
# Coding Best Practices

## Naming Conventions
- Variables and functions: `camelCase`
- Files classes and types: `PascalCase`
- Constants: `UPPER_SNAKE_CASE`
- Folders: `kebab-case`

# Git Workflow

### Branch Naming
- Use short, descriptive branch names.
- Format:
  - `FirstInitialLastInitial-BranchTopic`
- Before a competition we will create a new branch off of `main` and use that during the competition, the naming convention is as follows:
  - `Comp-20XXCompetitionName`
- After the competition we will review the `Competition` branch and make a new branch based off of it. This review branch will be used to see what we will keep and merge back to `main`, the naming convention is as follows:
  - `Review-20XXCompetitionName`
- The review branch will **ONLY** be merged to `main` through a `pull request`.

**Examples:**
- `YA-ArmSubsystem`
- `Comp-2026Humber`
- `Review-2026Humber`

### Branch Merging
- Branches will be merged using `Squash and Merge` or `Rebase` only, do not use a `Merge Commit`.
- You should only be merging other branches together or merging *FROM* `main` to another branch.
- **NEVER MERGE TO MAIN MANUALLY**. Merges to main shall *ONLY* be done through `pull requests`.
---

### Pull Requests
- All changes to `main` must go through a pull request.
- Keep pull requests formatted according to the `Pull request template`.
- Inside the description clearly describe:
  - What was changed
  - Why it was changed
- Ensure code builds and tests pass before requesting review.
- You must assign the Programming Mentor (Yusuf) and another senior member of the Programming sub-team as a reviewer.
- When the pull request is approved you must merge using `Squash and Merge` or `Rebase`.

---

### Commits


Do your best to follow this commit message format: [Semantic Commit Messages](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716) by Josh Buchea

Within the description of the commit message be concise with what you are changing and adding, summarizing the topic efficiently.

#### Example:

```
feat: add hat wobble
^--^  ^------------^
|     |
|     +-> Summary in present tense.
|
+-------> Type: chore, docs, feat, fix, refactor, style, or test.
```

#### List of types and purposes

- `feat`: (new feature for the user, not a new feature for build script)
- `fix`: (bug fix for the user, not a fix to a build script)
- `refactor`: (refactoring production code, eg. renaming a variable)
- `docs`: (changes to the documentation; no production code change)
- `style`: (formatting, missing semi colons, etc; no production code change)
- `test`: (adding missing tests, refactoring tests; no production code change)
- `chore`: (updating grunt tasks etc; no production code change)
- `ci`: (updating ci to change deployment, etc; no production code change)
