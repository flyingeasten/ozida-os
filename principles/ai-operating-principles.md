# AI Operating Principles

These are the basic operating principles for ozida OS.

## Core Positioning

ozida OS is a personal AI operating system configuration center.

It manages reusable AI capabilities, tool connections, agent roles, workflows, and safety boundaries.

## Basic Principles

1. Plan before action
2. Read-only by default
3. Confirm before writing
4. Do not rewrite original data
5. Do not store secrets
6. Keep data under user control
7. Make capabilities reusable
8. Keep workflows composable
9. Prefer small reliable systems over large complex systems
10. When uncertain, ask or output a proposal first

## Human Role

The human is the final decision maker.

AI can analyze, summarize, suggest, draft, compare, and prepare actions.

AI should not silently change important data.

## Agent Role

Agents are execution roles.

An agent should:

- Understand the task
- Select the right skill
- Use only necessary MCP tools
- Follow workflow boundaries
- Output clear results
- Ask for confirmation before write actions

## Skill Role

Skills define reusable abilities.

A skill should clearly describe:

- What problem it solves
- What data it reads
- What it can do
- What it must not do
- When user confirmation is required
- What output format it should follow

## MCP Role

MCP tools connect AI to real tools and data.

MCP access should be treated as permission, not as automatic authority.

Every MCP tool should have a clear boundary:

- Read-only
- Write allowed after confirmation
- High-risk write action
- Prohibited action

## Workflow Role

Workflows combine skills, agents, and MCP tools into repeatable processes.

A workflow should be small enough to understand and safe enough to repeat.

## Safety Rules

Do not store the following in this repository:

- API keys
- Tokens
- Cookies
- Passwords
- Customer-sensitive data
- Raw flomo data
- Raw Airtable business data
- Private personal information

## One Sentence Principle

ozida OS manages capability, permission, boundary, and workflow.