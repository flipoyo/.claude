# claude

This project's Claude Code interface: `CLAUDE.md`, `AGENT.md`, the
permission-allowlist `settings.json`, and whatever the interface grows next
(skills, agents, commands).

Mount this repository at `.claude/` in a consuming project. This `main`
branch carries the shared baseline — currently just `settings.json`'s
permission allowlist, which every project inherits. Each consuming project
then gets its own branch, named after the project, merging `main` forward
and adding that project's `CLAUDE.md` and `AGENT.md`.

The consuming project tracks `CLAUDE.md` and `AGENT.md` at its own root as
symbolic links into this mount (`CLAUDE.md -> .claude/CLAUDE.md`,
`AGENT.md -> .claude/AGENT.md`), so Claude Code finds them at the exact
path it expects.
