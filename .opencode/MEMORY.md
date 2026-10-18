# ChickenLoop — project memory

## Purpose / state

Empty greenfield project at `C:\VIBE_CODE_CENTRAL\ChickenLoop`. No source code, **not a git repository**, no git remote.

## Decisions

- **Issue tracker: GitHub** (chosen 2026-10-18), via the `gh` CLI. Config in `docs/agents/issue-tracker.md`.
  - *Gotcha:* `gh` infers the repo from `git remote -v`, which doesn't exist yet. Until `git init` + a GitHub remote is added, every `gh` call will fail. A warning block sits at the top of `issue-tracker.md`.
  - The five triage labels have **not** been created on GitHub for the same reason. Run `gh label create <name>` for each once a remote exists.
  - `PRs as a request surface` is **off**.
- **Triage labels: defaults kept** — `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`. See `docs/agents/triage-labels.md`.
- **Domain docs: single-context** — one `GLOSSARY.md` and one `docs/adr/` at the repo root. See `docs/agents/domain.md`.
- Agent instructions live in `AGENTS.md` (chosen over `CLAUDE.md`).

## Key files

- `AGENTS.md` — the `## Agent skills` block
- `docs/agents/issue-tracker.md`
- `docs/agents/triage-labels.md`
- `docs/agents/domain.md`

## Next step

`git init`, add a GitHub remote, push, then create the five triage labels. Until then the issue tracker config is written but not operational.