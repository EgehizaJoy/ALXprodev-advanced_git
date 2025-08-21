Login Feature Coming soon
# add login changes
# Project Name

This project uses **Git-Flow** to manage development, features, releases, and hotfixes in a consistent and scalable way.

---

## Git-Flow Overview

Git-Flow is a branching model for Git, proposed by Vincent Driessen, that helps developers:

- Organize code by clearly separating development stages
- Collaborate effectively in teams
- Maintain code stability before production
- Manage releases and hotfixes efficiently

---

## Branch Structure

| Branch | Purpose |
|--------|---------|
| `main` (or `master`) | Production-ready code |
| `develop` | Ongoing development |
| `feature/*` | New features in progress |
| `release/*` | Preparation for production releases |
| `hotfix/*` | Critical bug fixes on main |

---

## Best Practices

- **Start with `develop`** – Branch new features from `develop`, not `main`.
- **Feature Isolation** – Keep each feature in its own branch to reduce conflicts.
- **Merge via Pull Requests** – Ensure code review for all merges.
- **Keep `main` clean** – Only production-ready code goes here.
- **Tag Releases** – Use Git tags to mark official release points.
- **Use `hotfix/*` for urgent bugs** – Fix critical issues directly on `main` and merge back into `develop`.
- **Document your workflow** – Keep Git-Flow documentation in your README or wiki.

---

## Git-Flow Commands

```bash
# Initialize Git-Flow
git flow init

# Feature branches
git flow feature start <name>
git flow feature finish <name>

# Release branches
git flow release start <x.x.x>
git flow release finish <x.x.x>

# Hotfix branches
git flow hotfix start <x.x.x>
git flow hotfix finish <x.x.x>
