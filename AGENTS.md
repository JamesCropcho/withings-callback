# withings-callback

A static GitHub Pages page used as the OAuth callback URL for James's personal Withings developer app. Withings rejects `localhost` and IP callbacks, so this page just displays the `code` from the redirect so it can be pasted into a local script (the code expires in 30 seconds). It loads no external resources and sends nothing anywhere.

Served at https://jamescropcho.github.io/withings-callback/ from `index.html` on `main`.

## Project memory

Claude Code loads memory automatically. Other agents: this repo has no memory of its own; the related notes live in `~/projects/.claude/memory/` (see `withings-fat-loss-tracking-research-2026.md`).
