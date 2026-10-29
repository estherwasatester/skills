# Antigravity Wrapped (skill)

A Spotify-Wrapped-style recap of every Antigravity conversation in a project: a single, self-contained HTML
story with stats, models, tokens, tools, skills, a narrated timeline and an optional two-host audio overview.
Everything is mined locally from your Antigravity history.

See [`examples/wrapped.html`](examples/wrapped.html) for a finished example (open it in a
browser). The skill uses it both as the visual reference and as the HTML template for new Wrappeds.

## Install
Copy this `antigravity-wrapped/` folder to one of:
- `~/.gemini/config/skills/antigravity-wrapped/`: available in all your projects
- `<repo>/.agents/skills/antigravity-wrapped/`: shared with everyone who clones the repo

## Use
Open Antigravity in the project and ask: **"Make me an Antigravity Wrapped"**.

## Requirements
- Node.js ≥ 22.5 (uses `node:sqlite`)
- Optional: the `gemini-api` CLI, signed in (for AI narration + audio). Without it, the agent writes the story itself.
- Optional: `ffmpeg` (smaller embedded audio)

## Privacy
Only aggregated, redacted stats are sent to Gemini (when available). Quoted prompts are capped at 160 chars, with
secrets, emails and passcodes redacted. Review the HTML before sharing it: it includes your file names and prompts.
