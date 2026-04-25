---
description: Workspace-level guidance for the my-soc-ops-csharp Blazor app and lab repo.
---

# Workspace Instructions

## Mandatory development checklist
- [ ] lint: run formatting/linting if configured (for example, `dotnet format`)
- [ ] build: `dotnet build SocOps/SocOps.csproj`
- [ ] test: run repository tests if present, e.g. `dotnet test`

## What this repo is
- Blazor WebAssembly social bingo game in `SocOps/`
- Workshop lab content in `workshop/` and docs in `docs/`
- `.solutions/` holds sample solution content; avoid editing unless requested

## Run and build
- `cd SocOps`
- `dotnet build SocOps.csproj`
- `dotnet run --project SocOps/SocOps.csproj`
- VS Code tasks: `.vscode/tasks.json` includes `dotnet: build` and `dotnet: run`

## Key areas
- `SocOps/Program.cs` — startup and services
- `SocOps/App.razor` — routing shell
- `SocOps/Pages/` — pages and routes
- `SocOps/Components/` — reusable UI pieces
- `SocOps/Services/` — game state and logic
- `SocOps/wwwroot/css/app.css` — utility CSS

## Agent workflow
- Use `setup.prompt.md` for environment setup and local dev checks
- Use `frontend-design` for UI/style work
- Use `css-utilities.instructions.md` for app CSS conventions
- Keep changes focused in `SocOps/` unless user asks to update docs or workshop content
