# Pull Request & Commit Guidelines

## Index

1. [Branching Strategy](#branching-strategy)
2. [Pull Request Titles](#pull-request-titles)
3. [Pull Request Template](#pull-request-template)
4. [Pre-Merge Checklist](#pre-merge-checklist)
5. [Review Process](#review-process)
6. [Merging Rules](#merging-rules)
7. [Commit Message Guidelines](#commit-message-guidelines)

---

## Branching Strategy

| Branch          | Purpose                      |
|-----------------|------------------------------|
| `master`        | Production-ready code        |
| `dev`           | Integration / staging branch |
| `feature/*`     | Feature branches             |
| `fix/*`         | Fix branches                 |
| `hotfix/*`      | Hotfix branches              |
| `refactoring/*` | Refactoring branches         |

- Always branch off from `dev`.
- Use `<commit-type>/<scope>` naming convention (e.g. `feature/select-account` or `feature/sa-1234`).

---

## Pull Request Titles

Use this format for all PR titles:

```
<type>(<scope>): Short, clear PR title
```

**Examples:**
```
fix(auth): prevent crash on expired token
feat(uikit): add RadioGroup component
refactor(core): simplify size format utility
```

- No Jira ticket numbers in titles.
- Focus on clarity, consistency, and scope.

---

## Pull Request Template

```md
### Description

[Jira ticket → SA-XXXX](https://magictoolbox.atlassian.net/browse/SA-XXXX)

Describe the purpose of this PR. What does it do? Why was it needed?

---

### Type of change

> Check all that apply:

- [ ] 🐛 Bugfix  
- [ ] 🔥 Feature  
- [ ] 🎨 Code style (formatting, minor naming changes)  
- [ ] 🧑‍💻 Refactor (no behavior changes)  
- [ ] 📝 Docs update  
- [ ] ✅ Tests  
- [ ] 🔭 Chore / Other  

---

### How to test it

Explain how this can be tested locally (manual or automated). Mention any specific packages or affected areas of the app.

---

### Notes for reviewer

Add any context, decisions, or tricky points that reviewers should know.
```
---

## Pre-Merge Checklist

Before requesting a review:

- [ ] Pull latest from `dev`
- [ ] Test changes manually
- [ ] Lint and type-check
- [ ] Remove debug logs and unused code
- [ ] Test affected local packages (e.g., `@sirv/ui`)
- [ ] Visually and functionally test any shared components (like from @sirv/ui) across all applications where they're used, to ensure nothing breaks
- [ ] Clearly document any updates to shared packages or workspace configurations

---

## Review Process

- Use `[WIP]` in title if still in progress.
- Assign **at least two reviewers** once ready.
- Be responsive to feedback and update PR as needed.
- Don’t self-merge unless explicitly allowed (e.g., for solo-owned modules).

---

## Merging Rules

- Merge only into `dev`.
- Use **Squash and merge** to keep commit history clean.
- Ensure:
  - Review approved
  - No conflicts
  - Final tests passed

If a shared package (e.g., `ui`) is changed:
- Note the impact clearly in PR

---

## Commit Message Guidelines

### Format

```
<type>(<scope>): short description
```

**Example:**
```
fix(auth): handle validation failure
```

### Allowed Types

| Type        | Description                              |
|-------------|------------------------------------------|
| `feat`      | New feature                              |
| `fix`       | Bug fix                                  |
| `refactor`  | Code restructure without behavior change |
| `style`     | Formatting, naming, whitespace, etc.     |
| `test`      | Adding or updating tests                 |
| `docs`      | Documentation only                       |
| `chore`     | Tooling, infra, package updates          |
| `build`     | Build tools and dependency changes       |
| `perf`      | Performance optimizations                |

### Common Scopes

| Scope              | Usage example                     |
|--------------------|-----------------------------------|
| `<module>`         | Module (e.g. `auth`)              |
| `<shared package>` | Shared package (e.g. `ui`)        |
| `api`              | Backend endpoints or logic        |
| `core`             | Utilities and shared logic        |
| `config`           | Tooling, build, or monorepo setup |

### Avoid

- Vague messages (`fix stuff`, `changes`)
- Unscoped or multi-purpose commits
- Leaving debug or test-only commits unsquashed

---
