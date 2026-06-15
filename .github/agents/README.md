# Copilot Agents

This repository defines custom Copilot agents in `.github/agents`.

## Available Agents
- `sre-engineer`: SRE and Azure specialist for Docker, Kubernetes, GitHub Actions, Makefile, and deployment automation.
- `web-designer`: Web designer and frontend layout specialist for semantic HTML, responsive CSS, and focused JavaScript interactions.

## Usage
- In Copilot custom agents, select `sre-engineer` or `web-designer`.
- For reusable prompts, use `.github/prompts/sre-engineer.prompt.md` or `.github/prompts/web-designer.prompt.md`.

## Notes
- Custom agents must be Markdown files ending in `.agent.md`.
- Agent files need YAML frontmatter with at least a `description`.
- `AGENTS.md` files are instructions, not selectable custom agent profiles.
