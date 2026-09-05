# AGENT

*Created: 2026-08-31*

This file exists only to state the reading order for an agent onboarding to
this project, per `DevSpecs.md`'s Documentation convention — it carries no
rules of its own.

1. [`CLAUDE.md`](CLAUDE.md) — commands, before-committing checklist, the
   architecture boundary summary.
2. `.localSpec/` for this project's own deeper references:
   [`AGENT.md`](.localSpec/AGENT.md) — the parallel-agent orchestration
   roster; [`AdditionalSpecs.md`](.localSpec/AdditionalSpecs.md) —
   architecture and project-specific technical rules (its Ring-model
   subsection points to [`docs/DevGuide/`](docs/DevGuide/README.md) for
   the full dependency graph and Tier↔Ring reconciliation);
   [`audit.md`](.localSpec/audit.md) — audit findings, legacy references,
   and open decisions/risks. `AgentSpec/` (and its `archive/`) holds any
   active `*_DevPlanTicket.md` — in-flight work.
3. [`DevSpecs.md`](.agentSpec/DevSpecs.md) — the underlying,
   project-agnostic philosophy all of the above conforms to. It lives, with
   `DOCSTYLE.md` and `TICKETLIFECYCLE.md`, in a mounted `flipoyo/.agentSpec`
   repository (not tracked by this repo — see `.gitignore`), the same way
   `docs/` holds `DocSpecs.md`.
