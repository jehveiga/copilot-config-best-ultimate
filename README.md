# .NET Copilot Configuration Pack

A curated set of GitHub Copilot customization files for .NET/C# backend development. Drop the `.github/` folder into any .NET repository to get opinionated, context-aware AI assistance out of the box.

## What's Included

### Agents

| Agent | Purpose |
|-------|---------|
| **.NET Self-Learning Architect** | Principal-level .NET architect that designs systems with right-sized architecture (minimalist → Clean Architecture), orchestrates subagents, and maintains a self-learning system with lessons and memories across sessions. |
| **C#/.NET Janitor** | Code cleanup, modernization, and tech debt remediation — applies latest C# features, fixes warnings, optimizes performance, and ensures test coverage. |

### Instructions

| File | Scope | Purpose |
|------|-------|---------|
| `csharp.instructions.md` | `**/*.cs` | Coding style, naming conventions, project structure, and C# 14 best practices. |
| `dotnet-upgrade.instructions.md` | On-demand | Step-by-step guidance for .NET framework version upgrades with progressive tracking. |

### Skills

| Skill | Domain |
|-------|--------|
| `csharp-async` | Async/await patterns, pitfalls, and performance |
| `csharp-docs` | XML documentation comments and API docs |
| `csharp-mstest` | MSTest 3.x/4.x best practices |
| `csharp-xunit` | xUnit testing patterns |
| `dotnet-best-practices` | General .NET/C# quality standards |
| `dotnet-design-pattern-review` | Design pattern review and recommendations |
| `dotnet-upgrade` | Framework upgrade analysis and execution |
| `ef-core` | Entity Framework Core best practices |

## Key Features

- **Architecture Selection Policy** — automatically scales from minimalist single-project structure to full Clean Architecture/DDD/CQRS based on actual project complexity.
- **Self-Learning System** — captures lessons from mistakes and durable memories from decisions, preventing repeated errors across sessions.
- **Post-Implementation Review** — automatically delegates code review to the Janitor agent after every feature delivery.
- **Living Documentation** — maintains a `CLAUDE.md` onboarding document that keeps project context synchronized across sessions.
- **Subagent Orchestration** — supports parallel and sequential delegation modes for complex multi-step tasks.

## Usage

1. Copy the `.github/` folder into the root of your .NET repository.
2. Open the project in VS Code with GitHub Copilot Chat enabled.
3. The agents, instructions, and skills are automatically available in Copilot Chat.

### Invoking Agents

- Use `@.NET Self-Learning Architect` for architecture decisions, feature implementation, and complex delivery.
- Use `@C#/.NET Janitor` for code cleanup, modernization, and quality sweeps.

## Requirements

- VS Code with GitHub Copilot Chat extension
- Copilot Chat agent mode enabled
- Compatible models: Claude Sonnet 4.6, Claude Opus 4.6, GPT-5.3-Codex, Claude Haiku 4.5

## License

MIT — use and adapt freely for your .NET projects.