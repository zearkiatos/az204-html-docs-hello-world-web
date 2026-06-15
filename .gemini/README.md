# Gemini Configuration

This folder configures Gemini-related behavior for this repository.

## Files
- `../GEMINI.md`: Root Gemini CLI context file. It imports the agent mode files in this folder.
- `agents/sre-engineer.md`: SRE Engineer mode for Docker, Kubernetes, GitHub Actions, Azure, and deployment work.
- `agents/web-designer.md`: Web Designer mode for semantic HTML, responsive CSS, JavaScript interactions, and layout work.
- `config.yaml`: Gemini Code Assist for GitHub repository configuration.
- `styleguide.md`: Gemini Code Assist review style guide.

## Gemini CLI
- Run `/memory show` to inspect loaded context.
- Run `/memory reload` after changing `GEMINI.md` or imported context files.
- Run `/skills list` to confirm the shared workspace skills from `.agents/skills`.
- Run `/skills reload` after changing skill files.

## Notes
- Gemini CLI supports `GEMINI.md` context files and `@file.md` imports.
- Gemini CLI also discovers skills from `.agents/skills`, so the existing `sre-engineer` and `web-designer` skills are shared with Codex.
