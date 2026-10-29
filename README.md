# Skills

Personal agent skills for Antigravity (`npx skills` / `.agents/skills` compatible).

## Included Skills

- **[`antigravity-wrapped`](./antigravity-wrapped/)**: Builds an "Antigravity Wrapped" (a Spotify-Wrapped-style, single-file HTML story) for the current project from its local Antigravity conversation history: stats, models, tokens, tools, skills, a narrated timeline, and an optional two-host audio overview.

## Installation

### Via Skills CLI
```bash
npx skills add estherwasatester/skills@antigravity-wrapped
```

### Manual Copy
Copy any skill folder to:
- `~/.gemini/config/skills/<skill-name>/` (global across all projects)
- `<repo>/.agents/skills/<skill-name>/` (project-scoped)
