# ChickenLoop — project memory

## Purpose / state

Greenfield project at `C:\VIBE_CODE_CENTRAL\ChickenLoop`, public GitHub repo `Chickenman67/ChickenLoop` (created 2026-10-18, branch `master`, local auth via `gh` as Chickenman67). No source code yet.

## Decisions

- **Issue tracker: GitHub** (chosen 2026-10-18), via the `gh` CLI. Config in `docs/agents/issue-tracker.md`.
  - The five triage labels are **created** on the remote. `wontfix` was pre-seeded by GitHub and was edited to our wording.
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

`GLOSSARY.md` and `docs/adr/` don't exist yet; `/domain-modeling` creates them lazily. Next real work is deciding what ChickenLoop actually is.