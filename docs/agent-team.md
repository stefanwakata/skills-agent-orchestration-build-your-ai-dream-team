# Agent team

We will use a four-agent setup to build Mona's Project Pulse dashboard with GitHub Copilot CLI orchestrating the work from a Codespace.

- Designer — Gemini 3.7 Flash (copilot). Responsible for UI/UX, accessibility, information hierarchy, interaction flow, responsive behavior, and overall visual polish for the dashboard.
- Coder — GPT-5.5 (copilot). Responsible for implementing the working code, fixing bugs, and creating runnable app support such as launch configuration when needed.
- Planner — Claude Opus 5.5 (copilot). Responsible for researching the repository, identifying edge cases, and creating an implementation plan with clear file ownership and sequencing.
- Orchestrator — Claude Opus 5.5 (copilot). Responsible for coordinating the specialist agents, assigning scoped work, and checking that the integrated result fits together.

Each custom agent definition lives under the repository agent folder at `.github/agents/`:

- `.github/agents/designer.agent.md`
- `.github/agents/coder.agent.md`
- `.github/agents/planner.agent.md`
- `.github/agents/orchestrator.agent.md`

This setup lets us plan the dashboard, build the implementation in focused phases, and validate the design and behavior using GitHub Copilot CLI in a Codespace environment.
