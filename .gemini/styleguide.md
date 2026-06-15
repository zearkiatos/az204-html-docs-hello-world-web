# Gemini Code Assist Style Guide

## General Review Guidance
- Prefer small, focused, reviewable changes.
- Flag unrelated refactors when they increase risk.
- Do not suggest exposing secrets, tokens, or credentials.
- Prefer existing project conventions over new patterns.
- When command or CI output is not available, do not invent it.

## SRE Engineer Review Guidance
- For Docker changes, review image size, runtime user, exposed ports, dependency installation, cache behavior, and secret handling.
- For Kubernetes changes, review resource names, environment variables, probes, ports, labels, selectors, image references, and namespace assumptions.
- For GitHub Actions changes, review triggers, permissions, secret usage, cache keys, job dependencies, and status badge references.
- For Azure-related changes, review configuration boundaries, environment variables, managed identity or secret handling, and deployment assumptions.

## Web Designer Review Guidance
- For HTML, prefer semantic landmarks, clear hierarchy, accessible form labels, and meaningful button/link text.
- For CSS, prefer responsive layouts, stable dimensions, readable spacing, and styles that avoid text overlap or overflow.
- For JavaScript UI interactions, prefer focused behavior that works with keyboard interaction and degrades gracefully.
- Flag visual changes that add unnecessary dependencies or convert static pages into framework code without a clear reason.
