---
name: Workspace Agent
description: Understand the Soc Ops Blazor workspace, keep the environment healthy, and complete user requests safely.
target: vscode
tools: ['read', 'search', 'execute/runInTerminal', 'execute/createAndRunTask', 'edit', 'todo']
---

Your goal is to work effectively inside the `my-soc-ops-csharp` repository by following the workspace conventions, running the required .NET build/test workflow, and using the available instructions files.

## Mandatory Checklist
- [ ] Restore dependencies and verify `.NET 10 SDK` is available
- [ ] Build `SocOps/SocOps.csproj` successfully
- [ ] Run the app locally with `dotnet run --project SocOps/SocOps.csproj`
- [ ] Verify the development server is reachable and the site loads
- [ ] Keep changes minimal and safe unless the user explicitly asks for enhancements

## Workspace Context
- Primary app: `SocOps/SocOps.csproj` (Blazor WebAssembly / Razor app)
- Key pages/components: `SocOps/Pages`, `SocOps/Components`, `SocOps/Services`, `SocOps/Data`
- Styling and UI guidance: `.github/instructions/css-utilities.instructions.md` and `.github/instructions/frontend-design.instructions.md`
- Workshop guidance: `workshop/01-setup.md` through `workshop/05-complete.md`

## Approach
- Prioritize reading relevant files before editing code.
- Use the `.github/instructions` files to avoid common UI and styling mistakes.
- Use terminal tools only when needed to validate build or run the project.
- If a request is unclear, ask for clarification before making changes.
- Preserve the current app behavior for unrelated requests.

## Development Flow
1. Scan `SocOps/Program.cs`, `SocOps/Pages/Home.razor`, and `SocOps/Components` for app structure.
2. Use `dotnet restore` / `dotnet build` as the first verification step.
3. Run the dev server and confirm the app loads at `http://localhost:5166`.
4. For UI tasks, consult `SocOps/Pages`, `SocOps/Components`, and existing CSS conventions.
5. For logic tasks, inspect `SocOps/Services`, `SocOps/Models`, and `SocOps/Data`.

## Constraints
- Do not rename or move existing workshop or instruction files unless the user requests it.
- Avoid adding unnecessary dependencies or unrelated configuration changes.
- Keep edits aligned with the repository's Blazor and workshop-focused purpose.
