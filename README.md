# Awesome Skills

A curated collection of open-source tools, skills, plugins, MCP servers, workflows, and local AI projects for AI-assisted development.

Focus: better coding agents, cleaner context, fewer wasted tokens, stronger workflows, and useful local tooling.

<img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> marks projects I personally use or especially like.

* [Agent Orchestration](#agent-orchestration)
* [Skills & Subagents](#skills--subagents)
* [Context & Token Management](#context--token-management)
* [MCP Servers & Browser Tools](#mcp-servers--browser-tools)
* [Coding Agents & Utilities](#coding-agents--utilities)
* [Local AI](#local-ai)
* [Plugins & Bundled Ecosystems](#plugins--bundled-ecosystems)
* [Contributing](#contributing)

## Agent Orchestration

These projects provide opinionated agent workflows, orchestration, delegation, planning, hooks, commands, or execution strategies.

They are generally better used **individually rather than stacked together**.

Running multiple orchestration systems at once can cause:

* conflicting system instructions
* duplicated planning and delegation
* competing hooks and lifecycle logic
* duplicated commands or skills
* conflicting task routing
* unnecessary context usage
* harder debugging
* unpredictable agent behavior

Each project can be useful on its own. Pick the orchestration model that fits your workflow instead of combining several frameworks that try to control the same agent lifecycle.

* [OmO](https://github.com/code-yeongyu/oh-my-openagent) — Full agent ecosystem with specialized agents, lifecycle hooks, commands, MCP integrations, delegation, and workflow automation.
* <img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> [OmO Slim](https://github.com/alvinunreal/oh-my-opencode-slim) — Leaner OpenCode multi-agent setup focused on delegation without the full OmO stack.
* [OpenAgentsControl](https://github.com/darrenhinde/OpenAgentsControl) — Plan-first development workflow with controlled execution, testing, review, and validation.
* [Superpowers](https://github.com/obra/superpowers) — Structured software development methodology built from composable agent skills and workflows.
* [YYLO](https://github.com/yylo-dev/yylo) — Orchestration CLI for AI coding agents with Kanban board, task worktrees, merge orchestration, and controller metadata stored as plain Markdown.

## Skills & Subagents

Reusable instructions, behaviors, and specialized agents.

* <img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> [Caveman](https://github.com/JuliusBrussee/caveman) — Keeps coding agents concise and reduces wasted tokens.
* <img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> [Hallmark](https://github.com/Nutlope/hallmark) — Design skill for interfaces that do not look AI-generated.
* <img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> [Ponytail](https://github.com/DietrichGebert/ponytail) — Pushes coding agents toward simpler engineering decisions.
* [i-have-adhd](https://github.com/ayghri/i-have-adhd) — Keeps coding-agent responses focused, scannable, and less likely to bury the useful answer.
* [Agent Skills](https://github.com/vercel-labs/agent-skills) — Reusable skills for AI coding agents.
* [Skills](https://github.com/mattpocock/skills) — Practical coding-agent skills by Matt Pocock.
* [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) — Large collection of specialized Claude Code subagents for development tasks.

## Context & Token Management

Tools focused on keeping agent context useful instead of filling it with unnecessary output.

* [Context7](https://github.com/upstash/context7) — Gives coding agents current library documentation.
* [RTK](https://github.com/rtk-ai/rtk) — Reduces command output before it reaches agent context.
* [Context Mode](https://github.com/mksglu/context-mode) — Sandboxes large tool outputs and reduces unnecessary context-window usage.
* <img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> [Dynamic Context Pruning](https://github.com/Tarquinen/opencode-dynamic-context-pruning) — Dynamically removes low-value OpenCode context to reduce token usage while preserving useful information.

## MCP Servers & Browser Tools

Useful Model Context Protocol servers and agent integrations.

* <img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> [Playwright MCP](https://github.com/microsoft/playwright-mcp) — Playwright MCP server for structured browser automation.
* [Browser MCP](https://github.com/BrowserMCP/mcp) — MCP server that lets AI applications control an existing browser session.
* <img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> [GitHub MCP Server](https://github.com/github/github-mcp-server) — GitHub's official MCP server for repository, issue, pull request, and development workflows.

## Coding Agents & Utilities

Standalone coding agents and supporting development tools.

* <img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> [OpenCode](https://github.com/anomalyco/opencode) — Open-source AI coding agent for terminal and desktop workflows.
* [Codex](https://github.com/openai/codex) — OpenAI coding agent for terminal-based development.
* [Serena](https://github.com/oraios/serena) — Semantic code retrieval and editing toolkit for coding agents.
* [Plannotator](https://github.com/backnotprop/plannotator) — Visual interface for reviewing agent plans and code changes.
* [CCUsage](https://github.com/ccusage/ccusage) — Tracks coding-agent token usage and costs.
* [Codeburn](https://github.com/getagentseal/codeburn) — Local token and cost tracker supporting many AI coding tools and agents.

## Local AI

Open-source tools for running, training, and experimenting with models locally.

* [Ollama](https://github.com/ollama/ollama) — Run and manage open models locally.
* <img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> [llama.cpp](https://github.com/ggml-org/llama.cpp) — Efficient local LLM inference in C and C++.
* [ik_llama.cpp](https://github.com/ikawrakow/ik_llama.cpp) — Performance-focused llama.cpp fork with extensive quantization and inference work.

  * Main upstream repository: [ikawrakow/ik_llama.cpp](https://github.com/ikawrakow/ik_llama.cpp)
  * Ready-to-use executables and release builds: [Thireus/ik_llama.cpp](https://github.com/Thireus/ik_llama.cpp)
* <img src="./assets/star-full.svg" width="12" height="12" alt="Favorite"> [Unsloth](https://github.com/unslothai/unsloth) — Open-source tooling for running, fine-tuning, and training local models.
* [TextGen](https://github.com/oobabooga/textgen) — Open-source desktop app and web UI for local LLMs with text, vision, tool calling, extensions, and compatible APIs.

## Plugins & Bundled Ecosystems

Plugins can be more than small extensions.

A plugin can package multiple pieces of an agent ecosystem together, including:

* MCP servers
* commands
* skills
* subagents
* hooks
* configuration
* workflow logic

For larger ecosystems, this is often preferable to asking users to install and configure every MCP server, command, skill, and hook separately.

Bundling related functionality into a plugin gives the ecosystem one installation path, one update path, compatible versions, predictable configuration, and easier removal.

Individual components still make sense when they are independently useful. Tightly coupled components are usually better shipped together.

## Contributing

Suggestions are welcome.

Open an issue or pull request if you know a useful AI coding skill, tool, workflow, MCP server, plugin, or local AI project that belongs here.

Projects must have a **100% open-source implementation available in a public GitHub repository**.

Not interested in:

* freemium products where important functionality is proprietary
* open-core projects with essential features kept closed
* source-available software that is not genuinely open source
* closed-source tools
* hosted-only services without a complete open-source implementation

Prefer the original upstream repository.

Keep descriptions short, factual, and useful.

Avoid adding several tools that solve exactly the same problem unless they provide meaningfully different approaches.

## License & Acknowledgements

This repository is licensed under the [MIT License](LICENSE).

Projects listed here remain subject to their own licenses.

Thanks to the maintainers and contributors behind every project listed here.

If this collection is useful to you, consider starring this repository and the projects you use.
