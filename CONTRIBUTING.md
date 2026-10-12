# Contributing

Follow these steps every time you make a change. Never commit directly to `main`.

## 1. Start from the latest `main`

```bash
git checkout main
git pull
```

## 2. Create a new branch

Name it after yourself and what you're doing:

```bash
git checkout -b your-name/short-description
```

Example: `git checkout -b alex/add-grade-calculator`

## 3. Make your changes and commit

```bash
git add .
git commit -m "Describe what you changed"
```

Commit as often as you like. Small commits with clear messages are easier to review.

## 4. Push your branch

```bash
git push -u origin your-name/short-description
```

## 5. Open a pull request (PR)

1. Go to the repo on GitHub. You'll see a yellow banner for your branch; click **Compare & pull request**.
2. Make sure the base branch is `main`.
3. Write a clear title and a short description: **what** you changed and **why**.
4. Click **Create pull request**.

## 6. Update the docs

Add docs for your change in the `docs/` folder, then commit and push them to the same branch. They'll show up in your PR automatically.

| Folder | When to add something |
|--------|------------------------|
| `docs/prs/` | **Every PR.** Copy your PR description into a new file, e.g. `0002-add-grade-calculator.md` (use your PR number). |
| `docs/adr/` | You made a significant design or technical decision (a new library, a change to how the project is structured). Explain what you decided and why. |
| `docs/design/` | You built something others need to understand: how it works, diagrams, plans. |
| `docs/issues/` | You found a bug or problem that needs a detailed write-up. |
| `docs/review/` | Notes from reviewing someone's code, or team retrospectives. |

Each folder has a `README.md` with more details on what goes there and how to name files.

## 7. Get an approval and merge

- Every PR needs **1 approval** from a teammate before it can be merged.
- Ask a teammate to review it. If they request changes, make them on the same branch and push again.
- Once it's approved, click **Merge pull request** on GitHub.

## 8. Clean up

Switch back to `main` and get the latest changes before starting your next task:

```bash
git checkout main
git pull
```
