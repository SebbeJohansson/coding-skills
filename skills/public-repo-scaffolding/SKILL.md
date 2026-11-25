---
name: public-repo-scaffolding
description: Start a new public GitHub repo from Sebastian's scaffolding template. Use when creating a new public repository, publishing a project, or setting up AGENTS.md, SECURITY.md, LICENSE, README, Go module or npm package publishing for a public repo.
---

# Public repo scaffolding

Template repo: https://github.com/SebbeJohansson/public-repo-template

It is a GitHub template repo. It holds the basics every public repo needs.

## What the template contains

| File | Purpose |
| ---- | ------- |
| `AGENTS.md` | Rules for agents: no secrets or internal references, what may be committed, issues, PRs, releases |
| `SECURITY.md` | How to report vulnerabilities, supported versions |
| `LICENSE` | MIT by default |
| `README.md` | Base README: what it is, install, usage, configuration, contributing, license |
| `docs/go-packages.md` | Go module path, tags, `go.mod` hygiene, module proxy |
| `docs/npm-packages.md` | `package.json` fields, scoped names, `files`, provenance, publishing |
| `docs/licenses.md` | When to pick a license other than MIT |

## Steps

1. Create the repo from the template, on the personal account:
   `gh repo create SebbeJohansson/<name> --template SebbeJohansson/public-repo-template --public --clone`
2. Fill in `README.md`: replace the placeholders, delete install lines that do not apply.
3. Check `LICENSE`. Keep MIT, or follow `docs/licenses.md` to choose another. Confirm you own the code: work written for an employer may not be yours to publish.
4. Check `SECURITY.md`: the contact address and the supported versions.
5. Keep only the package guide that applies (`docs/go-packages.md` or `docs/npm-packages.md`). Delete the other and its link in `AGENTS.md`.
6. Run the pre-publish checklist at the bottom of `AGENTS.md`. Nothing internal may remain.
7. Commit with the git identity for personal projects (not an employer email).

## Rules

- The template is the source of truth. Improve it there, not in copies.
- Never put secrets or internal names (company, tickets, hostnames) in a public repo, including its history.
- Do not publish a package, or push a tag, without the maintainer's approval.
