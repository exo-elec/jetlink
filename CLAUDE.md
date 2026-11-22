# CLAUDE.md

## Review and sub-agents

- **Scrutinize (`/scrutinize`).** Skill at `.claude/skills/scrutinize/SKILL.md`. Use it for every review, audit, sanity check or second opinion on a plan, PR, diff or design, and run it on your own non-trivial changes before reporting them done.
- **Antigravity sub-agent (`antigravity`).** Sends a self-contained task to the Google Antigravity CLI (`agy`, Gemini models on the owner's paid plan). Use it when the owner asks for Antigravity, agy or Gemini, for an independent non-Claude second opinion during `/scrutinize` on large or risky changes, or to offload a well-specified side task in parallel. Default model is `gemini-4-neon-high`; use `gemini-4-carbon-high` for the hardest design work. Verify its output yourself before relying on it. If `agy` is not installed or signed in on this machine, skip it.
