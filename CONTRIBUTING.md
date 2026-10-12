# Contributing

Follow these steps every time you make a change. Never commit directly to `main`.

The steps below use **GitHub Desktop**. If you prefer the command line, open the "Using the command line" section under each step.

## 1. Start from the latest `main`

In GitHub Desktop, click **Current Branch** and select `main`, then click **Fetch origin** (and **Pull origin** if it appears).

<details>
<summary>Using the command line</summary>

```bash
git checkout main
git pull
```
</details>

## 2. Create a new branch

Click **Current Branch** → **New Branch**. Name it after yourself and what you're doing, then click **Create Branch**.

Example: `alex/add-grade-calculator`

<details>
<summary>Using the command line</summary>

```bash
git checkout -b alex/add-grade-calculator
```
</details>

## 3. Make your changes and commit

Edit your files. In the **Changes** tab, check the files you want, write a short summary of what you changed, and click **Commit to [your branch]**.

Small commits with clear messages are easier to review.

<details>
<summary>Using the command line</summary>

```bash
git add .
git commit -m "Describe what you changed"
```
</details>

## 4. Push your branch

Click **Publish branch** (first time) or **Push origin** (after that).

<details>
<summary>Using the command line</summary>

```bash
git push -u origin alex/add-grade-calculator
```
</details>

## 5. Open a pull request (PR)

1. In GitHub Desktop, click **Create Pull Request**. This opens GitHub in your browser.
2. Make sure the base branch is `main`.
3. Write a clear title and a short description: **what** you changed and **why**.
4. Click **Create pull request**.

## 6. Update the docs

Add docs for your change in the `docs/` folder, then commit and push them to the same branch (steps 3 and 4). They'll show up in your PR automatically.

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

Go back to step 1: switch to `main` and pull the latest changes before starting your next task.
