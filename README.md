# company-site

The company's institutional website.

This repository currently holds documentation only: no application code, no
build step and no dependencies yet.

## Status

- Scope: the public website of the company.
- Code: none yet.
- Stack: not decided.

## Stack

The framework, build tooling, hosting and deployment target will be defined by
the plan approved by the board. Until that plan exists:

- Do not pick a stack.
- Do not scaffold a project.
- Do not add dependencies.

The `Commands` section of [AGENTS.md](./AGENTS.md) is the single place where the
install, lint, build and test commands will be recorded. It is filled in by the
first code pull request, after the stack comes from the plan.

## How agents work here

Work is organized around one issue at a time: each issue gets its own git
worktree and branch, the change lands as a single small pull request against
`main`, and it is reviewed before anything else happens. Agents do not merge
pull requests and do not deploy anything — both wait for the board.

## Where decisions live

- [AGENTS.md](./AGENTS.md) — the source of truth for how work is done in this
  repository: branches, commits, pull requests, checks, review, and what agents
  must never do.
- The board-approved plan — scope, stack, structure and deployment for the
  website. It is linked from the issue that introduces each decision.

## Before you start

Read [AGENTS.md](./AGENTS.md) in full, then follow the process described there.
This README only points to it; if the two ever disagree, `AGENTS.md` wins.
