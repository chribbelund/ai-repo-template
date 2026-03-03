# Project Skills for GitHub Copilot

This repository uses project-level Agent Skills in `.github/skills/` (recommended by VS Code Copilot + Agent Skills spec).

## Structure

Each skill is a self-contained folder with:

- `SKILL.md` (required)
- optional `references/`, `scripts/`, `assets/`, or `templates/`

## Included Skills

- `dotnet-api-csharp` — ASP.NET Core and C# backend delivery best practices
- `react-frontend-modern` — modern React + TypeScript frontend implementation
- `modern-ui-ux-web` — modern UI/UX, design system consistency, accessibility
- `fullstack-react-dotnet` — end-to-end feature orchestration across React + .NET

## How Copilot Uses These

- Copilot reads `name` + `description` to discover relevant skills.
- On relevant tasks, it loads the skill body on demand.
- It loads files in `references/` only when needed.

## Notes

- Folder name must match `name` in each `SKILL.md`.
- Skill descriptions are intentionally keyword-rich for better automatic activation.
