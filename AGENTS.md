# AGENTS.md

Rules for every AI agent working in this repository. Read this file before you start any issue.

## Project

- This repository holds the company's website.
- Stack, structure and commands are defined in the plan the board approved. Until that plan exists, do not scaffold or pick a stack on your own.
- Once the stack is decided, the Planner updates the "Commands" section below in the first code PR.

## Commands

<!-- Filled in by the first code PR. Example:
- Install: `npm ci`
- Lint: `npm run lint`
- Build: `npm run build`
- Test: `npm test`
-->

## How to work

1. Read the whole issue first: context, acceptance criteria and any plan linked to it.
2. Work only in the git worktree and branch Paperclip created for the issue. Never commit to `main`.
3. One issue = one small PR. If the issue is too big for one PR, say so in a comment instead of doing it all.
4. Use conventional commits: `feat:`, `fix:`, `chore:`, `docs:`, `refactor:`, `test:`.
5. Before opening a PR, run lint and build (and tests, if they exist). All must pass.
6. Push with `git push -u origin HEAD`. Open the PR with `gh pr create --fill --base main` if none exists yet.
7. Report in the Paperclip issue. The first line of your comment is the PR URL. Then list what changed and which checks you ran.
8. Move the issue to `in_review` only when CI is green.

## When something goes wrong

- **CI fails:** fix it. If you can't, mark the issue `blocked` and name the failing check.
- **Merge conflict:** stop. Don't resolve it blindly. Mark the issue `blocked` and explain what conflicts.
- **Unclear request:** ask in a comment on the issue and wait. Don't guess.

## Never

- Merge PRs (no `gh pr merge`, no `--admin`).
- Force-push, use `--no-verify`, or rewrite history on shared branches.
- Deploy anything. Deploys happen only after the board's OK.
- Commit secrets, tokens, `.env` files or client data.
- Add a new dependency without explaining why in the PR description.
- Change `AGENTS.md`, `.github/CODEOWNERS` or branch protection, unless the issue explicitly asks for it.
- Touch files outside this repository's worktree.

## Communication

- Comments to the board (João) in Brazilian Portuguese. Keep them short.
- Code, commit messages and PR titles in English.
