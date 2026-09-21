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
   and open decisions/risks; and
   [`DevTickets/`](.localSpec/DevTickets/README.md) — the planning surface:
   the owner's short tickets, the ranked `openTickets/` holding in-flight
   `*_DevPlanTicket.md` work, and `archive/` for closed ones.
3. [`DevSpecs.md`](.agentSpec/DevSpec/DevSpecs.md) — the underlying,
   project-agnostic philosophy all of the above conforms to. It lives, with
   `DOCSTYLE.md`, [`AgentConduct.md`](.agentSpec/DevSpec/AgentConduct.md) —
   the checklist shape, commit-message rule, and attribution every
   conforming project shares — and the generic `AGENT.md` template, in
   `flipoyo/DevSpec`, which the mounted `flipoyo/.agentSpec` repository
   mounts one level deeper (neither is tracked by this repo — see
   `.gitignore`), the same way `docs/` holds `DocSpecs.md`.
   `.agentSpec/TICKETLIFECYCLE.md` sits in the outer one.
