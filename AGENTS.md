# withings-callback

A static GitHub Pages page used as the OAuth callback URL for James's personal Withings developer app. Withings rejects `localhost` and IP callbacks, so this page just displays the `code` from the redirect so it can be pasted into a local script (the code expires in 30 seconds). It loads no external resources and sends nothing anywhere.

Served at https://jamescropcho.github.io/withings-callback/ from `index.html` on `main`.

## Git hooks

`.githooks/pre-commit` refuses a commit in which `CLAUDE.md`, `GEMINI.md` or
`README.md` is no longer a symlink to `AGENTS.md`. Claude Code turns the hooks
on at the start of every session through a SessionStart hook in
`.claude/settings.json`. Any other agent, or a person in a new clone, must run
`git config core.hooksPath .githooks` once, or commits skip the check silently.

## Project memory

This repo has no memory of its own. Its notes live with the project that uses it, in `~/projects/weight-trend/.claude/memory/`: read that folder's `MEMORY.md` first, then `withings-fat-loss-tracking-research-2026.md` and `setup-history-2026-11.md`.
