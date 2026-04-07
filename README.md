<p align="center">
  <br>
  <img width="80" src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg" alt="Awesome">
  <br>
</p>

<h1 align="center">Awesome AI Assistant Extensions</h1>

<p align="center">A curated list of awesome extensions, plugins, skills, and MCP servers for AI assistants.</p>

<p align="center">
  <a href="http://makeapullrequest.com"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome"></a>
  <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" alt="License"></a>
  <a href="https://hol.org/registry/extensions"><img src="https://img.shields.io/badge/Browse-Registry-green" alt="Browse Registry"></a>
</p>

<p align="center">
  This list covers extensions for <strong>OpenAI Codex</strong>, <strong>Claude Code</strong>, <strong>Google Gemini CLI</strong>, and cross-platform <strong>MCP servers</strong> that work across multiple AI assistants.
</p>

<br>

## Contents

- [Start Here](#start-here)
- [OpenAI Codex Plugins](#openai-codex-plugins)
- [Claude Code Extensions](#claude-code-extensions)
- [Google Gemini CLI Extensions](#google-gemini-cli-extensions)
- [MCP Servers (Cross-Platform)](#mcp-servers-cross-platform)
- [Cross-AI Tools](#cross-ai-tools)
- [Development Resources](#development-resources)
- [Related Projects](#related-projects)

---

## Start Here

This list covers the emerging ecosystem of AI assistant extensions. Each platform has its own extension format:

| Platform | Format | Repository |
|----------|--------|------------|
| OpenAI Codex | `.codex-plugin/plugin.json` + skills | [awesome-codex-plugins](https://github.com/hashgraph-online/awesome-codex-plugins) |
| Claude Code | Skills (`SKILL.md` + tools) | [anthropics/skills](https://github.com/anthropics/skills) |
| Gemini CLI | Extensions (`.gemini/`) | [Piebald-AI/awesome-gemini-cli-extensions](https://github.com/Piebald-AI/awesome-gemini-cli-extensions) |
| Cross-AI | MCP servers (`mcp.json`) | [punkye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) |

### Quick Validation

Before publishing extensions, validate them:

```bash
# Codex plugins
pipx run codex-plugin-scanner lint .

# MCP servers
npx @modelcontextprotocol/server-validator
```

---

## OpenAI Codex Plugins

OpenAI Codex plugins package skills, MCP servers, and app integrations into shareable, installable bundles. See the dedicated list: [awesome-codex-plugins](https://github.com/hashgraph-online/awesome-codex-plugins)

<details>
<summary>Curated by OpenAI — available in the built-in Codex Plugin Directory</summary>

- Box - Access and manage files.
- Cloudflare - Manage Workers, Pages, DNS, and infrastructure.
- Figma - Inspect designs, extract specs, and document components.
- GitHub - Review changes, manage issues, and interact with repositories.
- Gmail - Read, search, and compose emails.
- Google Drive - Edit and manage files in Google Drive.
- Hugging Face - Browse models, datasets, and spaces.
- Linear - Create and manage issues, projects, and workflows.
- Notion - Create and edit pages, databases, and content.
- Sentry - Monitor errors, triage issues, and track performance.
- Slack - Send messages, search channels, manage conversations.
- Vercel - Deploy, preview, and manage Vercel projects.

</details>

### Community Plugins

Third-party plugins built by the community.

#### Development & Workflow

<!-- pinned -->
- [Registry Broker](https://github.com/hashgraph-online/registry-broker-codex-plugin) - Delegate tasks to specialist AI agents via the HOL Registry.
- [AgentOps](https://github.com/boshu2/agentops) - DevOps layer for coding agents with flow, feedback, and memory.
- [Claude Code for Codex](https://github.com/sendbird/cc-plugin-codex) - Use Claude Code from Codex for reviews and rescue tasks.
- [Claude Octopus](https://github.com/nyldn/claude-octopus) - Multi-LLM orchestration dispatching to 8 providers.
- [Codex Agenteam](https://github.com/yimwoo/codex-agenteam) - Specialist AI agents orchestrated as a configurable team pipeline.
- [HOTL Plugin](https://github.com/yimwoo/hotl-plugin) - Human-on-the-Loop AI coding workflow plugin.

#### Tools & Integrations

- [Apple Productivity](https://github.com/matk0shub/apple-productivity-mcp) - Local Apple Calendar and Reminders for macOS.
- [Bitbucket CLI](https://github.com/avivsinai/bitbucket-cli) - Manage Bitbucket repos, PRs, and pipelines.
- [Langfuse Observability](https://github.com/avivsinai/langfuse-mcp) - Query traces, debug exceptions, analyze sessions.
- [Remotion Plugin](https://github.com/tim-osterhus/codex-remotion-plugin) - Build parameterized Remotion videos in Codex.

---

## Claude Code Extensions

Claude Code extends Anthropic's CLI with custom skills and tools. The official skill repository: [anthropics/skills](https://github.com/anthropics/skills)

### Official Skills

- [Agent Skills](https://github.com/anthropics/skills) - Public repository for Claude Code agent skills.

### Community Skills

#### Development & Workflow

- [Claude Code Skills](https://github.com/alirezarezvani/claude-skills) - 223 production-ready skills, 23 agents, and 298 Python tools.
- [Claude Code Harness](https://github.com/dadwadw233/claude-code-harness) - Blueprint skill for turning vague agent ideas into concrete designs.
- [Codex Reviewer](https://github.com/schuettc/codex-reviewer) - Second-pass review of Claude-driven plans.

#### Multi-Provider Orchestration

- [Claude Octopus](https://github.com/nyldn/claude-octopus) - Multi-LLM orchestration dispatching to Codex, Gemini, Copilot, Qwen, Perplexity, OpenRouter, Ollama, OpenCode.

---

## Google Gemini CLI Extensions

Extensions for Google's Gemini CLI. See: [Piebald-AI/awesome-gemini-cli-extensions](https://github.com/Piebald-AI/awesome-gemini-cli-extensions)

### Official Extensions

- [Gemini CLI Extensions](https://github.com/google/gemini-cli) - Official Gemini CLI and extension system.

### Community Extensions

_Contributions welcome - submit via PR_

---

## MCP Servers (Cross-Platform)

Model Context Protocol (MCP) servers work across multiple AI assistants that support the protocol. See the comprehensive list: [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) (84k stars)

### Popular MCP Servers

#### Development

- [Claude Code MCP](https://github.com/anthropics/mcp-claude-code) - Official MCP server for Claude Code.
- [Codex MCP](https://github.com/openai/mcp-codex) - Official MCP server for Codex.
- [Filesystem](https://github.com/modelcontextprotocol/server-filesystem) - Read and write to local filesystem.
- [GitHub](https://github.com/modelcontextprotocol/server-github) - Manage GitHub repos, issues, PRs.
- [Brave Search](https://github.com/modelcontextprotocol/server-brave-search) - Web search via Brave API.

#### Data & APIs

- [PostgreSQL](https://github.com/modelcontextprotocol/server-postgres) - Database queries and operations.
- [Puppeteer](https://github.com/modelcontextprotocol/server-puppeteer) - Browser automation.
- [Slack](https://github.com/modelcontextprotocol/server-slack) - Slack workspace interactions.
- [Google Maps](https://github.com/modelcontextprotocol/server-google-maps) - Location and mapping services.

### MCP Clients

- [Cursor](https://cursor.sh) - AI-powered code editor with MCP support.
- [Claude Desktop](https://claude.ai/download) - Anthropic's desktop app with MCP integration.
- [Codex](https://openai.com/codex) - OpenAI's CLI with MCP support.
- [Windsurf](https://windsurf.ai) - Codeium's AI agent with MCP support.

---

## Cross-AI Tools

Tools and frameworks that work across multiple AI assistants.

### Agent Frameworks

- [OpenAgents](https://github.com/a16z-infra/openagents) - Open-source platform for building AI agents.
- [AgentKit](https://github.com/agentkit/agentkit) - Multi-platform AI agent development kit.
- [SuperAgent](https://github.com/superagent-ai/superagent) - Build and deploy AI agents.

### Evaluation & Monitoring

- [AgentOps](https://agentops.ai) - DevOps layer for AI agents with session tracking and analytics.
- [Langfuse](https://langfuse.com) - Open-source LLM observability and analytics platform.
- [Helicone](https://helicone.ai) - Open-source AI observability platform.
- [Guardrails](https://github.com/guardrails-ai/guardrails) - Validate and correct LLM output.

### Knowledge & Context

- [Mem0](https://github.com/mem0ai/mem0) - Memory layer for AI agents.
- [Letta](https://letta.com) - Stateful AI agents with memory management.
- [Context7](https://context7.com) - Context-aware AI assistant platform.

---

## Development Resources

### Codex Plugin Development

- [Official Docs: Agent Skills](https://developers.openai.com/codex/skills)
- [Official Docs: Build Plugins](https://developers.openai.com/codex/plugins/build)
- [codex-plugin-scanner](https://github.com/hashgraph-online/codex-plugin-scanner) - Quality gate for Codex plugins

### Claude Code Development

- [Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code/overview)
- [Skill Authoring Guide](https://docs.anthropic.com/en/docs/claude-code/writing-skills)

### MCP Development

- [MCP Specification](https://spec.modelcontextprotocol.io)
- [MCP SDK](https://github.com/modelcontextprotocol/python-sdk)
- [MCP TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk)

---

## Related Projects

- [awesome-codex-plugins](https://github.com/hashgraph-online/awesome-codex-plugins) - Codex-specific plugin list
- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - Comprehensive MCP server list (84k stars)
- [awesome-mcp-clients](https://github.com/punkpeye/awesome-mcp-clients) - MCP client applications
- [awesome-ai-agents](https://github.com/e2b-dev/awesome-ai-agents) - AI agent frameworks and tools (27k stars)
- [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) - LLM app examples (104k stars)
- [codex-plugin-scanner](https://github.com/hashgraph-online/codex-plugin-scanner) - Codex plugin quality gate
- [HOL Registry](https://hol.org/registry) - Discover and install extensions

---

## Contributing

PRs welcome! Please follow the contribution guidelines and ensure extensions are validated before submitting.

```bash
# Validate Codex plugins
pipx run codex-plugin-scanner lint .
pipx run codex-plugin-scanner verify .
```

## License

[Apache 2.0](./LICENSE) — Hashgraph Online
