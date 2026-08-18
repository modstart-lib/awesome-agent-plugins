<div align="center">

# Awesome Agent Plugins

**A curated collection of Agent plugins & skills for AI agents, from GitHub.**

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Agent Plugins Spec](https://img.shields.io/badge/Agent%20Plugins-v1.0.0-blueviolet)](https://agent-plugins.org/)

**English** | [中文](README.zh-CN.md)

</div>

This repository collects the best **Agent plugins** — reusable packages that extend AI agents with
[Agent Skills](https://agentskills.io/specification) and [MCP servers](https://modelcontextprotocol.io/specification) —
built around the open, vendor-neutral [**Agent Plugins**](https://agent-plugins.org/) standard
(packaged as `plugin.json` + `skills/` + `mcp.json`).

Inspired by [awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) and the
[Agent Plugins specification](https://agent-plugins.org/specification), everything listed here has been
discovered and verified on GitHub, and is organized by industry / function.

## Table of Contents

- [What is an Agent Plugin?](#what-is-an-agent-plugin)
- [🧩 Agent Plugins (Coming Soon)](#-agent-plugins-coming-soon)
- [📢 Current Status](#-current-status)
- [Quick Overview by Category](#quick-overview-by-category)
- [📚 Curated Collections](#-curated-collections)
- [🏢 Official Vendor Skills](#-official-vendor-skills)
- [🧠 Frameworks & Workflows](#-frameworks--workflows)
- [💻 Software Development](#-software-development)
  - [Frontend](#frontend)
  - [Backend & API](#backend--api)
  - [Testing & QA](#testing--qa)
  - [Databases & Data](#databases--data)
  - [DevOps & Cloud](#devops--cloud)
- [🔐 Security](#-security)
- [🎨 Design & Creative](#-design--creative)
- [📈 Marketing & Growth](#-marketing--growth)
- [📝 Productivity & Documentation](#-productivity--documentation)
- [🎓 Research & Education](#-research--education)
- [💰 Finance & Web3](#-finance--web3)
- [🤖 Client Plugins](#-client-plugins)
- [🔌 MCP Servers & Integrations](#-mcp-servers--integrations)
- [🌐 Community & Multi-Harness](#-community--multi-harness)
- [🇨🇳 Chinese Resources](#-chinese-resources)
- [Contributing](#contributing)
- [License](#license)

---

## What is an Agent Plugin?

According to the [Agent Plugins](https://agent-plugins.org/) standard, an **Agent Plugin** is a portable
package that extends AI agents with reusable components:

```text
my-plugin/
├── plugin.json          # manifest ($schema, name, version, description, ...)
├── skills/              # Agent Skills (SKILL.md per skill)
│   └── summarize/
│       ├── SKILL.md
│       ├── scripts/
│       └── references/
├── mcp.json             # MCP server configuration
└── com.example.client/  # client-specific extension namespace
```

The v1.0.0 specification defines exactly two portable component types: **Agent Skills** and **MCP servers**.
It is backed by a Technical Steering Committee with maintainers from Amazon, Cursor, Microsoft, OpenAI,
and Vercel.

> **Related standards:** [Agent Skills](https://agentskills.io/specification) ·
> [Model Context Protocol](https://modelcontextprotocol.io/specification) ·
> [Agent Plugins spec](https://agent-plugins.org/specification)

## 🧩 Agent Plugins (Coming Soon)

> This section is **reserved** for portable **Agent Plugins** that conform to the
> [Agent Plugins v1.0.0](https://agent-plugins.org/specification) standard (`plugin.json` + `skills/` + `mcp.json`).
> It will be populated in upcoming updates.

- _(to be added — stay tuned)_ 🔜

## 📢 Current Status

> **Note:** The entries currently listed in this document are primarily **Agent Skills** and skill-oriented
> collections (skills, skill frameworks, skill marketplaces). A dedicated **Agent Plugins** section is
> reserved above and will be filled with conformant `plugin.json` packages in upcoming updates.
>
> 当前列表收录的条目以 **Agent Skills**（技能及技能合集）为主；符合 Agent Plugins 规范的可移植插件包
> 将在上方的预留区陆续补充。

## Quick Overview by Category

| Category | What you'll find |
| --- | --- |
| 📚 Curated Collections | The best "awesome" lists for skills, plugins, MCP servers |
| 🏢 Official Vendor Skills | First-party skills from Anthropic, Google, Stripe, Cloudflare, etc. |
| 🧠 Frameworks & Workflows | Methodologies and skill frameworks for agentic development |
| 💻 Software Development | Frontend, backend, testing, databases, DevOps |
| 🔐 Security | Security review, auditing, and AppSec skills |
| 🎨 Design & Creative | UI/UX, generative art, video, image design |
| 📈 Marketing & Growth | Copywriting, SEO, growth engineering |
| 📝 Productivity & Documentation | Docs, office files, personal productivity |
| 🎓 Research & Education | Academic and scientific research skills |
| 💰 Finance & Web3 | Payments, crypto, trading |
| 🤖 Client Plugins | Plugins for OpenCode, Claude Code, Gemini CLI, etc. |
| 🔌 MCP Servers | MCP servers and tool integrations |
| 🌐 Community & Multi-Harness | Cross-harness marketplaces and community skills |
| 🇨🇳 Chinese Resources | Chinese-language resources |

---

## 📚 Curated Collections

The best places to discover more agent skills and plugins.

- [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) - Curated collection of 1000+ agent skills from official dev teams and the community, compatible with Claude Code, Codex, Gemini CLI, Cursor, and more.
- [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) - Curated list of awesome Claude Skills, resources, and tools for customizing Claude AI workflows.
- [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) - Hand-picked collection of the finest resources for Claude Code and AI agents.
- [awesome-opencode/awesome-opencode](https://github.com/awesome-opencode/awesome-opencode) - Curated list of awesome plugins, themes, agents, projects, and resources for opencode.ai.
- [davepoon/buildwithclaude](https://github.com/davepoon/buildwithclaude) - A single hub to find Claude Skills, Agents, Commands, Hooks, Plugins, and Marketplace collections.
- [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) - 345+ Claude Code skills, agent skills, and plugins (30+ agents, 70+ custom commands, 330+ skills).
- [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) - 100+ AI Agents, Agent Skills, and RAG apps, free and open source.
- [sickn33/agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) - AAS Core: local, agent-first control plane for catalog discovery and agent-owned skill selection.
- [0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) - Independent directory of skills, plugins, memory providers, tools, surfaces, and guides for Hermes Agent.
- [Agent Plugins Directory](https://agentpluginsdirectory.com) - Verified web directory for the Agent Plugins standard: every plugin.json on GitHub fetched daily and checked against the official 1.0.0 schema, with published stats and a free validator.
- [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - The most popular collection of MCP servers.
- [appcypher/awesome-mcp-servers](https://github.com/appcypher/awesome-mcp-servers) - Curated list of Model Context Protocol servers.
- [wong2/awesome-mcp-servers](https://github.com/wong2/awesome-mcp-servers) - Another curated list of MCP servers (incl. official and community servers).

## 🏢 Official Vendor Skills

First-party skills published by the teams that build the tools.

- [anthropics/skills](https://github.com/anthropics/skills) - The official public repository for Anthropic Agent Skills (docx, pptx, xlsx, pdf, canvas-design, frontend-design, mcp-builder, webapp-testing, brand-guidelines, skill-creator, and more).
- [angular/skills](https://github.com/angular/skills) - Official Angular skills for generating Angular code, components, services, and new apps.
- [openai](https://github.com/openai) - OpenAI agent skills & guidance for building with the OpenAI API.
- [google-gemini/gemini-api-dev](https://officialskills.sh/google-gemini/skills/gemini-api-dev) - Best practices for developing Gemini-powered apps using the Gemini API.
- [stripe/stripe-best-practices](https://officialskills.sh/stripe/skills/stripe-best-practices) - Best practices for building Stripe integrations, plus SDK/API upgrade skills.
- [vercel-labs/next-best-practices](https://officialskills.sh/vercel-labs/skills/next-best-practices) - Next.js best practices, caching, and upgrade skills from the Vercel engineering team.
- [cloudflare](https://officialskills.sh/cloudflare/skills/cloudflare) - Comprehensive Cloudflare platform skill covering Workers, Pages, storage, AI, networking, security, and IaC.
- [netlify](https://officialskills.sh/netlify/skills/netlify-functions) - Netlify team skills: functions, edge functions, blobs, DB, image CDN, forms, caching, and deploys.
- [hashicorp](https://officialskills.sh/hashicorp/skills/new-terraform-provider) - Official Terraform skills: provider scaffolding, resources, test patterns, style guide, stacks, and more.
- [supabase/postgres-best-practices](https://officialskills.sh/supabase/skills/postgres-best-practices) - PostgreSQL best practices for Supabase.
- [neondatabase/neon-postgres](https://officialskills.sh/neondatabase/skills/neon-postgres) - Best practices for Neon Serverless Postgres and claimable Postgres provisioning.
- [clickhouse/clickhouse-best-practices](https://officialskills.sh/clickhouse/skills/clickhouse-best-practices) - Best practices for ClickHouse, architecture advisor, and local/cloud deployment.
- [sanity-io/sanity-best-practices](https://officialskills.sh/sanity-io/skills/sanity-best-practices) - Sanity Studio, GROQ, content modeling, and SEO/AEO best practices.
- [firecrawl](https://officialskills.sh/firecrawl/skills/firecrawl-build) - Firecrawl team skills for web search, scraping, extraction, and browser interaction.
- [mongodb](https://github.com/mongodb) - Official MongoDB skills for working with MongoDB databases and drivers.
- [redis](https://github.com/redis) - Official Redis skills for working with Redis data structures and clients.
- [duckdb](https://github.com/duckdb) - Official DuckDB skills for embedded analytics.
- [NVIDIA](https://github.com/NVIDIA) - NVIDIA skills for AI/GPU development.
- [google-cloud](https://github.com/GoogleCloudPlatform) - Google Cloud skills for GCP development and operations.
- [microsoft](https://github.com/microsoft) - Microsoft skills for Azure, .NET, and AI development.
- [figma](https://github.com/figma) - Figma skills for design-to-code and Figma API integration.
- [expo](https://github.com/expo) - Expo team skills for building, deploying, and debugging Expo apps.
- [firebase](https://github.com/firebase) - Firebase skills for web and mobile backends.
- [flutter](https://github.com/flutter) - Flutter skills for cross-platform UI development.
- [greensock/gsap-skills](https://github.com/greensock/gsap-skills) - Official AI skills teaching coding agents to correctly use GSAP.
- [typefully/typefully](https://officialskills.sh/typefully/skills/typefully) - Create, schedule, and publish social media content across X, LinkedIn, Threads, Bluesky, and Mastodon.
- [replicate/replicate](https://officialskills.sh/replicate/skills/replicate) - Discover, compare, and run AI models using Replicate's API.
- [remotion-dev/remotion](https://officialskills.sh/remotion-dev/skills/remotion) - Programmatic video creation with React.
- [composiohq/composio](https://officialskills.sh/composiohq/skills/composio) - Connect AI agents to 1000+ external apps with managed authentication.
- [veniceai/skills](https://github.com/veniceai/skills) - Official Venice API skills: chat, image, audio, video, models, billing, and more.

## 🧠 Frameworks & Workflows

Methodologies, frameworks, and workflows that make agents more effective.

- [obra/superpowers](https://github.com/obra/superpowers) - An agentic skills framework & software development methodology that works.
- [affaan-m/ECC](https://github.com/affaan-m/ECC) - The agent harness performance optimization system: skills, instincts, memory, security, and research.
- [mattpocock/skills](https://github.com/mattpocock/skills) - "Skills for Real Engineers" — skills straight from a senior engineer's `.agents` directory.
- [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) - Production-grade engineering skills for AI coding agents.
- [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) - A single CLAUDE.md-derived skill set to improve Claude Code behavior, based on Andrej Karpathy's observations.
- [garrytan/gstack](https://github.com/garrytan/gstack) - Garry Tan's exact Claude Code setup: 23 opinionated tools serving as CEO, Designer, and PM.
- [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) - Persistent file-based planning for AI coding agents and long-running tasks; crash-proof markdown plans.
- [phuryn/pm-skills](https://github.com/phuryn/pm-skills) - PM Skills Marketplace: 100+ agentic skills, commands, and plugins — from discovery to strategy, execution, and delivery.
- [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) - A complete AI agency at your fingertips — from frontend wizards to Reddit community ninjas.
- [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) - Makes your AI agent think like the laziest senior dev in the room — the best code is code you never write.
- [gemini-cli-extensions/conductor](https://github.com/gemini-cli-extensions/conductor) - A plugin for AI coding agents (Antigravity, Claude Code) enabling Spec-Driven Development.
- [wshobson/agents](https://github.com/wshobson/agents) - Multi-harness agentic plugin marketplace for Claude Code, Codex CLI, Cursor, OpenCode, and GitHub Copilot.

## 💻 Software Development

### Frontend

- [anthropics/frontend-design](https://github.com/anthropics/skills) - Frontend design and UI/UX development tools (official Anthropic skill).
- [google-labs-code/shadcn-ui](https://officialskills.sh/google-labs-code/skills/shadcn-ui) - Build UI components with shadcn/ui (Google Stitch).
- [google-labs-code/react-components](https://officialskills.sh/google-labs-code/skills/react-components) - Stitch-to-React component conversion.
- [angular/angular-new-app](https://github.com/angular/skills) - Create new Angular apps using the CLI with modern best practices.
- [callstackincubator/react-native-best-practices](https://officialskills.sh/callstackincubator/skills/react-native-best-practices) - Performance optimization for React Native apps from Callstack.
- [callstackincubator/upgrading-react-native](https://officialskills.sh/callstackincubator/skills/upgrading-react-native) - React Native upgrade workflow: templates, dependencies, and common pitfalls.
- [flutter](https://github.com/flutter) - Official Flutter skills for cross-platform UI development.

### Backend & API

- [anthropics/mcp-builder](https://github.com/anthropics/skills) - Create MCP servers to integrate external APIs and services (official Anthropic skill).
- [better-auth](https://github.com/better-auth) - Better Auth skills: best practices, providers, organization, two-factor, and error explanation.
- [trycourier/courier-skills](https://github.com/trycourier/courier-skills) - Multi-channel notifications via email, SMS, push, and chat.
- [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) - Persistent context across sessions for every agent; captures everything your agent does during a session.
- [hey-api/hey-api](https://github.com/hey-api/hey-api) - Turn API specifications into production-ready SDKs, validators, mocks, and more.
- [apollo-graphql](https://github.com/apollographql) - Apollo GraphQL skills for building GraphQL APIs.
- [auth0](https://github.com/auth0) - Auth0 skills for authentication and authorization.

### Testing & QA

- [anthropics/webapp-testing](https://github.com/anthropics/skills) - Test local web applications using Playwright (official Anthropic skill).
- [testmu-ai/playwright-skill](https://github.com/LambdaTest/agent-skills/tree/main/playwright-skill) - Generate Playwright E2E tests in TS, JS, Python, Java, or C#.
- [testmu-ai/cypress-skill](https://github.com/LambdaTest/agent-skills/tree/main/cypress-skill) - Generate Cypress E2E and component tests in JavaScript or TypeScript.
- [testmu-ai/pytest-skill](https://github.com/LambdaTest/agent-skills/tree/main/pytest-skill) - Generate pytest tests in Python with fixtures, parametrize, and mocking.
- [testmu-ai/jest-skill](https://github.com/LambdaTest/agent-skills/tree/main/jest-skill) - Generate Jest unit and integration tests in JS/TS with mocking and snapshots.
- [testmu-ai/selenium-skill](https://github.com/LambdaTest/agent-skills/tree/main/selenium-skill) - Generate Selenium WebDriver tests in Java, Python, JS, C#, Ruby, or PHP.
- [testmu-ai/appium-skill](https://github.com/LambdaTest/agent-skills/tree/main/appium-skill) - Generate Appium mobile automation for Android and iOS in Java, Python, or JS.
- [testmu-ai/test-framework-migration-skill](https://github.com/LambdaTest/agent-skills/tree/main/test-framework-migration-skill) - Migrate tests between Selenium, Playwright, Puppeteer, and Cypress.
- [code-yeongyu/oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent) - OMO/lazycodex: the coding agent for tokenmaxxers; the one and only agent harness for complex codebases.

### Databases & Data

- [supabase/postgres-best-practices](https://officialskills.sh/supabase/skills/postgres-best-practices) - PostgreSQL best practices for Supabase.
- [neondatabase/neon-postgres](https://officialskills.sh/neondatabase/skills/neon-postgres) - Neon Serverless Postgres best practices and claimable databases.
- [clickhouse/clickhouse-best-practices](https://officialskills.sh/clickhouse/skills/clickhouse-best-practices) - ClickHouse best practices and architecture advisor.
- [tinybirdco/tinybird-best-practices](https://officialskills.sh/tinybirdco/skills/tinybird-best-practices) - Tinybird project guidelines for datasources, pipes, endpoints, and SQL.
- [mongodb](https://github.com/mongodb) - Official MongoDB skills.
- [redis](https://github.com/redis) - Official Redis skills.
- [duckdb](https://github.com/duckdb) - Official DuckDB skills.
- [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) - Turn any codebase, with its docs, SQL schemas, configs, and PDFs, into a queryable knowledge graph.
- [Egonex-AI/Understand-Anything](https://github.com/Egonex-AI/Understand-Anything) - Graphs that teach > graphs that impress; turn any code into an interactive knowledge graph.
- [volcengine/OpenViking](https://github.com/volcengine/OpenViking) - Self-evolving Context Database for AI agents; unify agent memory, knowledge RAG, and skills.

### DevOps & Cloud

- [cloudflare](https://officialskills.sh/cloudflare/skills/cloudflare) - Comprehensive Cloudflare platform skill (Workers, Pages, storage, AI, networking, security, IaC).
- [netlify](https://officialskills.sh/netlify/skills/netlify-functions) - Netlify skills: functions, edge functions, blobs, DB, image CDN, forms, caching, deploys.
- [hashicorp/terraform](https://officialskills.sh/hashicorp/skills/new-terraform-provider) - Official Terraform skills: providers, resources, tests, style guide, stacks, and import.
- [google-cloud](https://github.com/GoogleCloudPlatform) - Google Cloud skills for GCP.
- [aws](https://github.com/aws) - AWS skills for cloud infrastructure and development.
- [azure](https://github.com/Azure) - Azure skills for Microsoft cloud.
- [rohitg00/awesome-devops-mcp-servers](https://github.com/rohitg00/awesome-devops-mcp-servers) - Curated MCP servers focused on DevOps tools and capabilities.

## 🔐 Security

- [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) - 817 structured cybersecurity skills for AI agents, mapped to 6 frameworks (MITRE ATT&CK, NIST CSF 2, and more).
- [trailofbits](https://github.com/trailofbits) - Security skills by Trail of Bits for secure development and auditing.
- [coderabbit](https://github.com/coderabbitai) - CodeRabbit skills for automated code review.
- [IBM/mcp-context-forge](https://github.com/IBM/mcp-context-forge) - An AI Gateway, registry, and proxy that sits in front of any MCP, A2A, or REST/gRPC APIs.

## 🎨 Design & Creative

- [nexu-io/open-design](https://github.com/nexu-io/open-design) - The open-source Claude Design alternative; local-first desktop app; your coding agent becomes a designer.
- [anthropics/canvas-design](https://github.com/anthropics/skills) - Design visual art in PNG and PDF formats (official Anthropic skill).
- [anthropics/algorithmic-art](https://github.com/anthropics/skills) - Create generative art using p5.js with seeded randomness (official Anthropic skill).
- [anthropics/theme-factory](https://github.com/anthropics/skills) - Style artifacts with professional themes or generate custom themes (official Anthropic skill).
- [anthropics/slack-gif-creator](https://github.com/anthropics/skills) - Create animated GIFs optimized for Slack size constraints (official Anthropic skill).
- [google-labs-code/design-md](https://officialskills.sh/google-labs-code/skills/design-md) - Create and manage DESIGN.md files (Google Stitch).
- [remotion-dev/remotion](https://officialskills.sh/remotion-dev/skills/remotion) - Programmatic video creation with React.
- [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) - World's first open-source agentic video production system: 12 production pipelines, 100+ tools, 700+ UI flows.
- [figma](https://github.com/figma) - Figma skills for design-to-code workflows.

## 📈 Marketing & Growth

- [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) - Marketing skills for Claude Code and AI agents: CRO, copywriting, SEO, analytics, and growth engineering.
- [typefully/typefully](https://officialskills.sh/typefully/skills/typefully) - Create, schedule, and publish social media content across X, LinkedIn, Threads, Bluesky, and Mastodon.
- [sanity-io/seo-aeo-best-practices](https://officialskills.sh/sanity-io/skills/seo-aeo-best-practices) - SEO and answer-engine optimization patterns for content sites.
- [realkimbarrett/advertising-skills](https://github.com/realkimbarrett/advertising-skills) - Advertising skills for OpenClaw, Claude Code & AI agents: direct response, paid media, and more.
- [anthropics/internal-comms](https://github.com/anthropics/skills) - Write status reports, newsletters, and FAQs (official Anthropic skill).

## 📝 Productivity & Documentation

- [anthropics/docx](https://github.com/anthropics/skills) - Create, edit, and analyze Word documents (official Anthropic skill).
- [anthropics/pptx](https://github.com/anthropics/skills) - Create, edit, and analyze PowerPoint presentations (official Anthropic skill).
- [anthropics/xlsx](https://github.com/anthropics/skills) - Create, edit, and analyze Excel spreadsheets (official Anthropic skill).
- [anthropics/pdf](https://github.com/anthropics/skills) - Extract text, create PDFs, and handle forms (official Anthropic skill).
- [anthropics/doc-coauthoring](https://github.com/anthropics/skills) - Collaborative document editing and co-authoring (official Anthropic skill).
- [googleworkspace/gws-drive](https://officialskills.sh/googleworkspace/skills/gws-drive) - Manage Google Drive files, folders, and shared drives via the `gws` CLI.
- [googleworkspace/gws-sheets](https://officialskills.sh/googleworkspace/skills/gws-sheets) - Read and write Google Sheets spreadsheets.
- [googleworkspace/gws-docs](https://officialskills.sh/googleworkspace/skills/gws-docs) - Read and write Google Docs documents.
- [googleworkspace/gws-gmail](https://officialskills.sh/googleworkspace/skills/gws-gmail) - Send, read, and manage Gmail email.
- [googleworkspace/gws-calendar](https://officialskills.sh/googleworkspace/skills/gws-calendar) - Manage Google Calendar calendars and events.
- [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills) - Agent skills for Obsidian; teach your agent to use Obsidian CLI and open formats including Markdown.
- [notion](https://github.com/makenotion) - Notion skills for managing Notion workspaces and databases.
- [resend](https://github.com/resend) - Resend skills for sending transactional email.

## 🎓 Research & Education

- [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) - Academic Research Skills for Claude Code: research → write → review → revise → finalize.
- [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) - Turn any AI agent into an AI Scientist; the #1 Agent Skills library for science.
- [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) - Research any topic across Reddit, X, YouTube, HN, Polymarket, and the web over the last 30 days.
- [googleworkspace/gws-classroom](https://officialskills.sh/googleworkspace/skills/gws-classroom) - Manage Google Classroom classes, rosters, and coursework.

## 💰 Finance & Web3

- [stripe/stripe-best-practices](https://officialskills.sh/stripe/skills/stripe-best-practices) - Best practices for building Stripe integrations.
- [stripe/upgrade-stripe](https://officialskills.sh/stripe/skills/upgrade-stripe) - Upgrade Stripe SDK and API versions.
- [binance](https://github.com/binance) - Binance skills for trading and market data.
- [coinbase](https://github.com/coinbase) - Coinbase skills for crypto and payments.
- [veniceai/venice-crypto-rpc](https://github.com/veniceai/skills/tree/main/skills/venice-crypto-rpc) - JSON-RPC proxying for supported crypto networks.
- [internet-court/internet-court-skill](https://github.com/internet-court/internet-court-skill) - The trust layer for agent-to-agent commerce — natural-language mandates and ERC-7710 delegations.

## 🤖 Client Plugins

Plugins, extensions, and agents for specific AI coding clients.

- [awesome-opencode/awesome-opencode](https://github.com/awesome-opencode/awesome-opencode) - Curated list of awesome plugins, themes, agents, and resources for opencode.ai.
- [Opencode-DCP/opencode-dynamic-context-pruning](https://github.com/Opencode-DCP/opencode-dynamic-context-pruning) - Dynamic context pruning plugin for OpenCode; intelligently manages conversation context.
- [numman-ali/opencode-openai-codex-auth](https://github.com/numman-ali/opencode-openai-codex-auth) - OAuth authentication plugin for personal coding assistance with ChatGPT Plus/Pro subscription.
- [jenslys/opencode-gemini-auth](https://github.com/jenslys/opencode-gemini-auth) - Gemini auth plugin for OpenCode.
- [tickernelz/opencode-mem](https://github.com/tickernelz/opencode-mem) - OpenCode plugin that gives coding agents persistent memory using a local vector database.
- [supermemoryai/opencode-supermemory](https://github.com/supermemoryai/opencode-supermemory) - Supermemory plugin for OpenCode.
- [jarrodwatts/claude-hud](https://github.com/jarrodwatts/claude-hud) - A Claude Code plugin that shows what's happening: context usage, active tools, running agents, and more.
- [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) - Persistent context across sessions for every agent.
- [CherryHQ/cherry-studio](https://github.com/CherryHQ/cherry-studio) - AI productivity studio with smart chat, autonomous agents, and 300+ assistants.
- [zhayujie/CowAgent](https://github.com/zhayujie/CowAgent) - Open-source super AI assistant & agent harness; plans tasks, runs tools and skills, self-evolves.
- [nanocoai/nanoclaw](https://github.com/nanocoai/nanoclaw) - A lightweight alternative to OpenClaw that runs in containers for security; connects to WhatsApp, Telegram, and more.
- [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) - Claude Code skill that cuts ~65% of tokens by talking like a caveman (laconic output style).

## 🔌 MCP Servers & Integrations

- [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - The most popular collection of MCP servers.
- [mcp-use/mcp-use](https://github.com/mcp-use/mcp-use) - The fullstack MCP framework to develop MCP apps for ChatGPT/Claude and MCP servers for AI agents.
- [IBM/mcp-context-forge](https://github.com/IBM/mcp-context-forge) - AI gateway, registry, and proxy in front of any MCP, A2A, or REST/gRPC API.
- [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) - The context API to search, scrape, and interact with the web at scale.
- [composiohq/composio](https://github.com/ComposioHQ/composio) - Connect AI agents to 1000+ external apps with managed authentication.
- [superpowers](https://github.com/obra/superpowers) - Includes MCP servers for browsing, memory, and more as part of its skills framework.
- [rohitg00/awesome-devops-mcp-servers](https://github.com/rohitg00/awesome-devops-mcp-servers) - Curated MCP servers for DevOps tools.

## 🌐 Community & Multi-Harness

- [wshobson/agents](https://github.com/wshobson/agents) - Multi-harness agentic plugin marketplace for Claude Code, Codex CLI, Cursor, OpenCode, GitHub Copilot.
- [VoltAgent/awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) - The awesome collection of OpenClaw skills: 5,400+ skills filtered and categorized.
- [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) - A complete AI agency at your fingertips.
- [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) - Marketing skills for Claude Code and AI agents.
- [phuryn/pm-skills](https://github.com/phuryn/pm-skills) - PM skills marketplace with 100+ agentic skills.

## 🇨🇳 Chinese Resources

中文相关的 Agent 技能与 MCP 资源。

- [yzfly/Awesome-MCP-ZH](https://github.com/yzfly/Awesome-MCP-ZH) - MCP 资源精选：MCP 指南、Claude MCP、MCP Servers、MCP Clients。
- [zhayujie/CowAgent](https://github.com/zhayujie/CowAgent) - 开源超级 AI 助手与 Agent 框架：规划任务、运行工具和技能、自我进化。
- [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) - 100+ AI Agents、Agent Skills 与 RAG 应用（开源）。
- [volcengine/OpenViking](https://github.com/volcengine/OpenViking) - 面向 AI Agent 的自进化上下文数据库，统一记忆、知识 RAG 与技能。
- [CherryHQ/cherry-studio](https://github.com/CherryHQ/cherry-studio) - 支持智能对话、自主 Agent 与 300+ 助手的 AI 生产力工作台。

---

## Contributing

Your contributions are always welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) guide first,
then open a Pull Request to add new plugins or improve existing entries.

All listed plugins are **discovered and verified on GitHub** and organized by industry/function. If you
maintain a great agent plugin and want it listed here, we'd love to hear from you.

## License

This project is licensed under the [MIT License](LICENSE).

The listed plugins are the property of their respective owners and released under their own licenses.

---

<p align="center">Made with ❤️ for the Agent Plugins community.</p>
