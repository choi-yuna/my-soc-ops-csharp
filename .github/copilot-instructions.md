---
description: Workspace-level guidance for the my-soc-ops-csharp Blazor app and lab repo.
---

# Workspace Instructions

## Mandatory development checklistÍ
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

## Design Guide

### Current Theme: Princess Style
The SocOps bingo game features a magical princess-themed design with elegant aesthetics, sparkles, and fairy-tale elements while maintaining professional functionality and accessibility.

### Color Palette
- **Primary:** Pink (#ec4899) - main accent color for buttons and highlights
- **Secondary:** Purple (#9333ea) - for marked states and secondary elements
- **Winning:** Gold (#fbbf24) - for bingo lines and victory states
- **Backgrounds:** Soft pink pastels (#fdf2f8) - light, elegant base colors
- **Text:** High contrast grays for readability

### Typography
- **Titles:** Playfair Display (Google Fonts) - clean, modern serif for elegance
- **Body:** System UI stack - sans-serif for readability
- **Hierarchy:** Consistent sizing with `text-4xl` for main titles, `text-3xl` for headings

### Design Principles
- **Creative & Distinctive:** Avoid generic AI aesthetics; use unique fonts, cohesive themes, and surprising elements
- **Motion & Delight:** CSS animations for page loads, hover effects, and micro-interactions
- **Accessibility:** High contrast ratios, readable fonts, keyboard navigation
- **Consistency:** CSS variables for colors, maintainable utility classes
- **Elegance:** Subtle gradients, ornate borders, sparkles without overwhelming simplicity

### Decorative Elements
- Sparkles (✨) for interactive states
- Crown icons (👑) for winning moments
- Rounded-xl borders and princess shadows
- Smooth transitions and float animations

### Guidelines for Changes
- Reference `frontend-design.instructions.md` for UI/style work
- Use `css-utilities.instructions.md` for CSS conventions
- Maintain princess theme consistency across new features
- Test on multiple screen sizes and ensure accessibility
- Prioritize user delight through thoughtful animations and visual hierarchy

## Agent workflow
- Use `setup.prompt.md` for environment setup and local dev checks
- Use `frontend-design` for UI/style work
- Use `css-utilities.instructions.md` for app CSS conventions
- Keep changes focused in `SocOps/` unless user asks to update docs or workshop content
