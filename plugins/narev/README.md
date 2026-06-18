# Narev Cursor Plugin

Real-time LLM pricing, cost estimation, Narev documentation, and usage-based billing skills for AI agents.

## What's included

- **MCP server** — hosted at `https://mcp.narev.ai` (configured automatically on install; no API key required for pricing and docs tools)
- **5 skills** vendored from [narevai/skills](https://github.com/narevai/skills)

| Skill | Purpose |
|-------|---------|
| `narev-starter` | Start here — routes to the right skill or docs path |
| `narev-lookup-llm-pricing` | Pricing API reference (seven public endpoints) |
| `narev-update-llm-pricing` | Pin/snapshot live pricing into your repo |
| `narev-nextjs-patterns` | Next.js App Router + Vercel AI SDK billing |
| `clerk-narev` | Clerk auth + Narev/Polar usage-based billing |

## Example prompts

| You say | Skill |
|---------|-------|
| "How does the Narev pricing API work?" | `narev-lookup-llm-pricing` |
| "Calculate USD for this token usage" | `narev-lookup-llm-pricing` |
| "Snapshot model pricing into a JSON file in my repo" | `narev-update-llm-pricing` |
| "Which Narev skill should I use for billing middleware?" | `narev-starter` |
| "Set up a new Next.js app with Narev billing and usage dashboard" | `narev-nextjs-patterns` |
| "Add Narev billing to my existing Next.js chat route" | `narev-nextjs-patterns` |

## MCP tools

When the plugin is installed, the agent can use these MCP tools:

- `list_providers`, `list_models`, `get_prices`, `calculate_cost` — live pricing
- `search_narev_docs`, `query_docs_filesystem_narev_docs` — Narev documentation

## Upstream

Skills are vendored from [narevai/skills](https://github.com/narevai/skills). To sync updates, copy the `skills/` directory from the upstream repository.

## Resources

- [Narev documentation](https://narev.ai/docs)
- [Agent quickstart](https://narev.ai/docs/quickstart-agents)
