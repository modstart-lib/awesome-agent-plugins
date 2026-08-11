<div align="center">

# Awesome Agent Plugins

**精选 GitHub 上 AI Agent 的插件（Agent plugins）与技能（Skills）合集。**

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Agent Plugins Spec](https://img.shields.io/badge/Agent%20Plugins-v1.0.0-blueviolet)](https://agent-plugins.org/)

[English](README.md) | **中文**

</div>

本仓库收集 GitHub 上最好用的 **Agent 插件** —— 通过可复用的组件（[Agent Skills](https://agentskills.io/specification)
与 [MCP 服务器](https://modelcontextprotocol.io/specification)）扩展 AI 智能体的可移植软件包，
遵循开放、厂商中立的 [**Agent Plugins**](https://agent-plugins.org/) 标准
（以 `plugin.json` + `skills/` + `mcp.json` 形式打包）。

参考 [awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) 与
[Agent Plugins 规范](https://agent-plugins.org/specification)，本列表中的每个项目都经过 GitHub 检索与验证，
并按行业/功能分类整理。

## 目录

- [什么是 Agent 插件？](#什么是-agent-插件)
- [🧩 Agent Plugins（即将更新）](#-agent-plugins即将更新)
- [📢 当前状态](#-当前状态)
- [分类速览](#分类速览)
- [📚 精选合集](#-精选合集)
- [🏢 官方厂商技能](#-官方厂商技能)
- [🧠 框架与工作流](#-框架与工作流)
- [💻 软件开发](#-软件开发)
  - [前端](#前端)
  - [后端与 API](#后端与-api)
  - [测试与质量保障](#测试与质量保障)
  - [数据库与数据](#数据库与数据)
  - [DevOps 与云](#devops-与云)
- [🔐 安全](#-安全)
- [🎨 设计与创意](#-设计与创意)
- [📈 营销与增长](#-营销与增长)
- [📝 生产力与文档](#-生产力与文档)
- [🎓 研究与教育](#-研究与教育)
- [💰 金融与 Web3](#-金融与-web3)
- [🤖 客户端插件](#-客户端插件)
- [🔌 MCP 服务器与集成](#-mcp-服务器与集成)
- [🌐 社区与多框架](#-社区与多框架)
- [🇨🇳 中文资源](#-中文资源)
- [参与贡献](#参与贡献)
- [许可证](#许可证)

---

## 什么是 Agent 插件？

根据 [Agent Plugins](https://agent-plugins.org/) 标准，**Agent 插件**（Agent Plugin）是一种可移植的软件包，
通过可复用组件扩展 AI 智能体：

```text
my-plugin/
├── plugin.json          # 清单文件（$schema、name、version、description 等）
├── skills/              # Agent Skills（每个技能一个 SKILL.md）
│   └── summarize/
│       ├── SKILL.md
│       ├── scripts/
│       └── references/
├── mcp.json             # MCP 服务器配置
└── com.example.client/  # 客户端专属扩展命名空间
```

v1.0.0 规范定义了两种可移植组件类型：**Agent Skills** 与 **MCP 服务器**。
技术指导委员会成员来自 Amazon、Cursor、Microsoft、OpenAI 与 Vercel。

> **相关标准：** [Agent Skills](https://agentskills.io/specification) ·
> [Model Context Protocol](https://modelcontextprotocol.io/specification) ·
> [Agent Plugins 规范](https://agent-plugins.org/specification)

## 🧩 Agent Plugins（即将更新）

> 本区为符合 [Agent Plugins v1.0.0](https://agent-plugins.org/specification) 标准
> （`plugin.json` + `skills/` + `mcp.json`）的**可移植插件包预留**，将在后续更新中陆续填充。

- _（敬请期待）_ 🔜

## 📢 当前状态

> **说明：** 当前列表收录的条目以 **Agent Skills**（技能及技能合集）为主——包括技能、技能框架与技能市场。
> 符合 Agent Plugins 规范的可移植插件包部分已在上述区域预留，将在后续更新中补充。
>
> **Note:** The entries currently listed in this document are primarily **Agent Skills** and skill-oriented
> collections. A dedicated **Agent Plugins** section is reserved above and will be filled with conformant
> `plugin.json` packages in upcoming updates.

## 分类速览

| 分类 | 你能找到什么 |
| --- | --- |
| 📚 精选合集 | 最优秀的技能/插件/MCP 服务器"awesome"列表 |
| 🏢 官方厂商技能 | Anthropic、Google、Stripe、Cloudflare 等第一方技能 |
| 🧠 框架与工作流 | Agentic 开发的方法论与技能框架 |
| 💻 软件开发 | 前端、后端、测试、数据库、DevOps |
| 🔐 安全 | 安全审查、审计与 AppSec 技能 |
| 🎨 设计与创意 | UI/UX、生成艺术、视频、图像设计 |
| 📈 营销与增长 | 文案、SEO、增长工程 |
| 📝 生产力与文档 | 文档、办公文件、个人生产力 |
| 🎓 研究与教育 | 学术与科学研究技能 |
| 💰 金融与 Web3 | 支付、加密货币、交易 |
| 🤖 客户端插件 | OpenCode、Claude Code、Gemini CLI 等插件 |
| 🔌 MCP 服务器 | MCP 服务器与工具集成 |
| 🌐 社区与多框架 | 跨框架市场与社区技能 |
| 🇨🇳 中文资源 | 中文生态资源 |

---

## 📚 精选合集

发现更多 Agent 技能与插件的最佳入口。

- [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) - 精选 1000+ 来自官方开发团队与社区的 Agent Skills，兼容 Claude Code、Codex、Gemini CLI、Cursor 等。
- [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) - 精选 Claude Skills、资源与工具，用于定制 Claude AI 工作流。
- [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) - 精心挑选的 Claude Code 与 AI 智能体最佳资源合集。
- [awesome-opencode/awesome-opencode](https://github.com/awesome-opencode/awesome-opencode) - 面向 opencode.ai 的插件、主题、智能体、项目与资源精选列表。
- [davepoon/buildwithclaude](https://github.com/davepoon/buildwithclaude) - 一站式寻找 Claude Skills、Agents、Commands、Hooks、Plugins 与市场合集。
- [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills) - 345+ 个 Claude Code 技能、Agent 技能与插件（30+ Agents、70+ 自定义命令、330+ 技能）。
- [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) - 100+ AI Agents、Agent Skills 与 RAG 应用，免费开源。
- [sickn33/agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) - AAS Core：本地优先、面向 Agent 的控制平面，支持目录发现与技能自主选择。
- [0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) - Hermes Agent 的技能、插件、记忆提供者、工具、界面与指南独立目录。
- [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - 最流行的 MCP 服务器合集。
- [appcypher/awesome-mcp-servers](https://github.com/appcypher/awesome-mcp-servers) - Model Context Protocol 服务器精选列表。
- [wong2/awesome-mcp-servers](https://github.com/wong2/awesome-mcp-servers) - 另一份 MCP 服务器精选列表（含官方与社区服务器）。

## 🏢 官方厂商技能

由工具开发者发布的第一方技能。

- [anthropics/skills](https://github.com/anthropics/skills) - Anthropic 官方 Agent Skills 公共仓库（docx、pptx、xlsx、pdf、canvas-design、frontend-design、mcp-builder、webapp-testing、brand-guidelines、skill-creator 等）。
- [angular/skills](https://github.com/angular/skills) - Angular 官方技能：生成 Angular 代码、组件、服务与新应用。
- [openai](https://github.com/openai) - OpenAI 官方技能与基于 OpenAI API 构建的指导。
- [google-gemini/gemini-api-dev](https://officialskills.sh/google-gemini/skills/gemini-api-dev) - 使用 Gemini API 开发应用的最佳实践。
- [stripe/stripe-best-practices](https://officialskills.sh/stripe/skills/stripe-best-practices) - 构建 Stripe 集成的最佳实践，以及 SDK/API 升级技能。
- [vercel-labs/next-best-practices](https://officialskills.sh/vercel-labs/skills/next-best-practices) - Vercel 工程团队的 Next.js 最佳实践、缓存与升级技能。
- [cloudflare](https://officialskills.sh/cloudflare/skills/cloudflare) - 综合 Cloudflare 平台技能：Workers、Pages、存储、AI、网络、安全与 IaC。
- [netlify](https://officialskills.sh/netlify/skills/netlify-functions) - Netlify 团队技能：函数、边缘函数、Blobs、数据库、图片 CDN、表单、缓存与部署。
- [hashicorp](https://officialskills.sh/hashicorp/skills/new-terraform-provider) - Terraform 官方技能：Provider 脚手架、资源、测试模式、风格指南、Stacks 等。
- [supabase/postgres-best-practices](https://officialskills.sh/supabase/skills/postgres-best-practices) - Supabase 的 PostgreSQL 最佳实践。
- [neondatabase/neon-postgres](https://officialskills.sh/neondatabase/skills/neon-postgres) - Neon Serverless Postgres 最佳实践与可认领数据库。
- [clickhouse/clickhouse-best-practices](https://officialskills.sh/clickhouse/skills/clickhouse-best-practices) - ClickHouse 最佳实践、架构顾问与本地/云端部署。
- [sanity-io/sanity-best-practices](https://officialskills.sh/sanity-io/skills/sanity-best-practices) - Sanity Studio、GROQ、内容建模与 SEO/AEO 最佳实践。
- [firecrawl](https://officialskills.sh/firecrawl/skills/firecrawl-build) - Firecrawl 团队技能：网页搜索、抓取、抽取与浏览器交互。
- [mongodb](https://github.com/mongodb) - MongoDB 官方技能。
- [redis](https://github.com/redis) - Redis 官方技能。
- [duckdb](https://github.com/duckdb) - DuckDB 官方技能（嵌入式分析）。
- [NVIDIA](https://github.com/NVIDIA) - NVIDIA 官方技能（AI/GPU 开发）。
- [google-cloud](https://github.com/GoogleCloudPlatform) - Google Cloud 技能（GCP 开发与运维）。
- [microsoft](https://github.com/microsoft) - Microsoft 官方技能（Azure、.NET 与 AI 开发）。
- [figma](https://github.com/figma) - Figma 技能：设计转代码与 Figma API 集成。
- [expo](https://github.com/expo) - Expo 团队技能：构建、部署与调试 Expo 应用。
- [firebase](https://github.com/firebase) - Firebase 技能（Web 与移动端后端）。
- [flutter](https://github.com/flutter) - Flutter 官方技能（跨平台 UI 开发）。
- [greensock/gsap-skills](https://github.com/greensock/gsap-skills) - GSAP 官方 AI 技能：教编码智能体正确使用 GSAP。
- [typefully/typefully](https://officialskills.sh/typefully/skills/typefully) - 在 X、LinkedIn、Threads、Bluesky 与 Mastodon 创建、排期与发布社媒内容。
- [replicate/replicate](https://officialskills.sh/replicate/skills/replicate) - 使用 Replicate API 发现、比较与运行 AI 模型。
- [remotion-dev/remotion](https://officialskills.sh/remotion-dev/skills/remotion) - 使用 React 进行程序化视频创作。
- [composiohq/composio](https://officialskills.sh/composiohq/skills/composio) - 通过托管认证将 AI Agent 连接到 1000+ 外部应用。
- [veniceai/skills](https://github.com/veniceai/skills) - Venice 官方 API 技能：聊天、图像、音频、视频、模型、计费等。

## 🧠 框架与工作流

让智能体更高效的方法论、框架与工作流。

- [obra/superpowers](https://github.com/obra/superpowers) - 行之有效的 Agentic 技能框架与软件开发方法论。
- [affaan-m/ECC](https://github.com/affaan-m/ECC) - Agent 运行时性能优化系统：技能、直觉、记忆、安全与研究。
- [mattpocock/skills](https://github.com/mattpocock/skills) - "真实工程师的技能" —— 来自资深工程师 `.agents` 目录。
- [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) - 面向 AI 编码智能体的生产级工程技能。
- [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) - 基于 Andrej Karpathy 观察衍生的单一技能集，改善 Claude Code 行为。
- [garrytan/gstack](https://github.com/garrytan/gstack) - Garry Tan 的完整 Claude Code 配置：23 个观点鲜明的工具，兼任 CEO、设计师与产品经理。
- [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) - 基于文件的持久化规划，适用于 AI 编码智能体与长任务；防崩溃的 Markdown 计划。
- [phuryn/pm-skills](https://github.com/phuryn/pm-skills) - 产品经理技能市场：100+ Agentic 技能、命令与插件——从发现、策略到执行与交付。
- [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) - 触手可及的完整 AI 代理机构——从前端大师到 Reddit 社区忍者。
- [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) - 让你的 AI Agent 像房间里最懒的资深开发那样思考——最好的代码是永远不需要写的代码。
- [gemini-cli-extensions/conductor](https://github.com/gemini-cli-extensions/conductor) - 面向 AI 编码智能体（Antigravity、Claude Code）的插件，支持规格驱动开发。
- [wshobson/agents](https://github.com/wshobson/agents) - 多框架 Agentic 插件市场：Claude Code、Codex CLI、Cursor、OpenCode、GitHub Copilot。

## 💻 软件开发

### 前端

- [anthropics/frontend-design](https://github.com/anthropics/skills) - 前端设计与 UI/UX 开发工具（Anthropic 官方技能）。
- [google-labs-code/shadcn-ui](https://officialskills.sh/google-labs-code/skills/shadcn-ui) - 使用 shadcn/ui 构建 UI 组件（Google Stitch）。
- [google-labs-code/react-components](https://officialskills.sh/google-labs-code/skills/react-components) - Stitch 转 React 组件转换。
- [angular/angular-new-app](https://github.com/angular/skills) - 使用 CLI 与最新最佳实践创建新 Angular 应用。
- [callstackincubator/react-native-best-practices](https://officialskills.sh/callstackincubator/skills/react-native-best-practices) - Callstack 出品的 React Native 性能优化。
- [callstackincubator/upgrading-react-native](https://officialskills.sh/callstackincubator/skills/upgrading-react-native) - React Native 升级工作流：模板、依赖与常见坑。
- [flutter](https://github.com/flutter) - Flutter 官方技能（跨平台 UI 开发）。

### 后端与 API

- [anthropics/mcp-builder](https://github.com/anthropics/skills) - 创建 MCP 服务器以集成外部 API 与服务（Anthropic 官方技能）。
- [better-auth](https://github.com/better-auth) - Better Auth 技能：最佳实践、提供商、组织、双因素认证与错误解释。
- [trycourier/courier-skills](https://github.com/trycourier/courier-skills) - 通过邮件、短信、推送与聊天实现多通道通知。
- [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) - 每个智能体的会话间持久上下文；捕获会话期间的所有操作。
- [hey-api/hey-api](https://github.com/hey-api/hey-api) - 将 API 规范转换为生产级 SDK、校验器、Mock 等。
- [apollo-graphql](https://github.com/apollographql) - Apollo GraphQL 技能（构建 GraphQL API）。
- [auth0](https://github.com/auth0) - Auth0 技能（认证与授权）。

### 测试与质量保障

- [anthropics/webapp-testing](https://github.com/anthropics/skills) - 使用 Playwright 测试本地 Web 应用（Anthropic 官方技能）。
- [testmu-ai/playwright-skill](https://github.com/LambdaTest/agent-skills/tree/main/playwright-skill) - 生成 TS、JS、Python、Java 或 C# 的 Playwright E2E 测试。
- [testmu-ai/cypress-skill](https://github.com/LambdaTest/agent-skills/tree/main/cypress-skill) - 生成 JavaScript/TypeScript 的 Cypress E2E 与组件测试。
- [testmu-ai/pytest-skill](https://github.com/LambdaTest/agent-skills/tree/main/pytest-skill) - 生成带 fixtures、参数化与 mock 的 pytest 测试。
- [testmu-ai/jest-skill](https://github.com/LambdaTest/agent-skills/tree/main/jest-skill) - 生成带 mock 与快照的 Jest 单元/集成测试。
- [testmu-ai/selenium-skill](https://github.com/LambdaTest/agent-skills/tree/main/selenium-skill) - 生成 Java、Python、JS、C#、Ruby 或 PHP 的 Selenium WebDriver 测试。
- [testmu-ai/appium-skill](https://github.com/LambdaTest/agent-skills/tree/main/appium-skill) - 生成 Android/iOS 的 Appium 移动自动化测试。
- [testmu-ai/test-framework-migration-skill](https://github.com/LambdaTest/agent-skills/tree/main/test-framework-migration-skill) - 在 Selenium、Playwright、Puppeteer 与 Cypress 之间迁移测试。
- [code-yeongyu/oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent) - OMO/lazycodex：面向复杂代码库的极致 Token 利用编码智能体。

### 数据库与数据

- [supabase/postgres-best-practices](https://officialskills.sh/supabase/skills/postgres-best-practices) - Supabase 的 PostgreSQL 最佳实践。
- [neondatabase/neon-postgres](https://officialskills.sh/neondatabase/skills/neon-postgres) - Neon Serverless Postgres 最佳实践与可认领数据库。
- [clickhouse/clickhouse-best-practices](https://officialskills.sh/clickhouse/skills/clickhouse-best-practices) - ClickHouse 最佳实践与架构顾问。
- [tinybirdco/tinybird-best-practices](https://officialskills.sh/tinybirdco/skills/tinybird-best-practices) - Tinybird 项目指南：数据源、管道、端点与 SQL。
- [mongodb](https://github.com/mongodb) - MongoDB 官方技能。
- [redis](https://github.com/redis) - Redis 官方技能。
- [duckdb](https://github.com/duckdb) - DuckDB 官方技能。
- [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) - 将代码库（含文档、SQL 模式、配置与 PDF）转化为可查询的知识图谱。
- [Egonex-AI/Understand-Anything](https://github.com/Egonex-AI/Understand-Anything) - 比惊艳更擅长教学的图谱；将任意代码转化为交互式知识图谱。
- [volcengine/OpenViking](https://github.com/volcengine/OpenViking) - 面向 AI Agent 的自进化上下文数据库，统一记忆、知识 RAG 与技能。

### DevOps 与云

- [cloudflare](https://officialskills.sh/cloudflare/skills/cloudflare) - 综合 Cloudflare 平台技能（Workers、Pages、存储、AI、网络、安全、IaC）。
- [netlify](https://officialskills.sh/netlify/skills/netlify-functions) - Netlify 技能：函数、边缘函数、Blobs、数据库、图片 CDN、表单、缓存、部署。
- [hashicorp/terraform](https://officialskills.sh/hashicorp/skills/new-terraform-provider) - Terraform 官方技能：Provider、资源、测试、风格指南、Stacks 与导入。
- [google-cloud](https://github.com/GoogleCloudPlatform) - Google Cloud 技能（GCP）。
- [aws](https://github.com/aws) - AWS 官方技能（云基础设施与开发）。
- [azure](https://github.com/Azure) - Azure 官方技能（微软云）。
- [rohitg00/awesome-devops-mcp-servers](https://github.com/rohitg00/awesome-devops-mcp-servers) - 面向 DevOps 工具与能力的 MCP 服务器精选。

## 🔐 安全

- [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) - 面向 AI Agent 的 817 个结构化网络安全技能，映射 6 大框架（MITRE ATT&CK、NIST CSF 2 等）。
- [trailofbits](https://github.com/trailofbits) - Trail of Bits 的安全技能（安全开发与审计）。
- [coderabbit](https://github.com/coderabbitai) - CodeRabbit 技能（自动化代码审查）。
- [IBM/mcp-context-forge](https://github.com/IBM/mcp-context-forge) - 位于任意 MCP、A2A 或 REST/gRPC API 之前的 AI 网关、注册表与代理。

## 🎨 设计与创意

- [nexu-io/open-design](https://github.com/nexu-io/open-design) - 开源的 Claude Design 替代品；本地优先桌面应用；让你的编码智能体成为设计师。
- [anthropics/canvas-design](https://github.com/anthropics/skills) - 以 PNG 与 PDF 格式设计视觉艺术（Anthropic 官方技能）。
- [anthropics/algorithmic-art](https://github.com/anthropics/skills) - 使用 p5.js 与固定随机种子创作生成艺术（Anthropic 官方技能）。
- [anthropics/theme-factory](https://github.com/anthropics/skills) - 用专业主题美化产物或生成自定义主题（Anthropic 官方技能）。
- [anthropics/slack-gif-creator](https://github.com/anthropics/skills) - 创建针对 Slack 尺寸限制优化的动画 GIF（Anthropic 官方技能）。
- [google-labs-code/design-md](https://officialskills.sh/google-labs-code/skills/design-md) - 创建与管理 DESIGN.md 文件（Google Stitch）。
- [remotion-dev/remotion](https://officialskills.sh/remotion-dev/skills/remotion) - 使用 React 进行程序化视频创作。
- [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) - 全球首个开源 Agentic 视频制作系统：12 条生产管线、100+ 工具、700+ UI 流程。
- [figma](https://github.com/figma) - Figma 技能（设计转代码工作流）。

## 📈 营销与增长

- [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) - 面向 Claude Code 与 AI Agent 的营销技能：CRO、文案、SEO、分析与增长工程。
- [typefully/typefully](https://officialskills.sh/typefully/skills/typefully) - 在 X、LinkedIn、Threads、Bluesky 与 Mastodon 创建、排期与发布社媒内容。
- [sanity-io/seo-aeo-best-practices](https://officialskills.sh/sanity-io/skills/seo-aeo-best-practices) - 内容网站的 SEO 与答案引擎优化模式。
- [realkimbarrett/advertising-skills](https://github.com/realkimbarrett/advertising-skills) - Kim Barrett 的广告技能：面向 OpenClaw、Claude Code 与 AI Agent 的直复营销与付费媒体。
- [anthropics/internal-comms](https://github.com/anthropics/skills) - 编写状态报告、新闻稿与 FAQ（Anthropic 官方技能）。

## 📝 生产力与文档

- [anthropics/docx](https://github.com/anthropics/skills) - 创建、编辑与分析 Word 文档（Anthropic 官方技能）。
- [anthropics/pptx](https://github.com/anthropics/skills) - 创建、编辑与分析 PowerPoint 演示文稿（Anthropic 官方技能）。
- [anthropics/xlsx](https://github.com/anthropics/skills) - 创建、编辑与分析 Excel 电子表格（Anthropic 官方技能）。
- [anthropics/pdf](https://github.com/anthropics/skills) - 提取文本、创建 PDF 与处理表单（Anthropic 官方技能）。
- [anthropics/doc-coauthoring](https://github.com/anthropics/skills) - 协作文档编辑与共同创作（Anthropic 官方技能）。
- [googleworkspace/gws-drive](https://officialskills.sh/googleworkspace/skills/gws-drive) - 通过 `gws` CLI 管理 Google Drive 文件、文件夹与共享盘。
- [googleworkspace/gws-sheets](https://officialskills.sh/googleworkspace/skills/gws-sheets) - 读写 Google Sheets 电子表格。
- [googleworkspace/gws-docs](https://officialskills.sh/googleworkspace/skills/gws-docs) - 读写 Google Docs 文档。
- [googleworkspace/gws-gmail](https://officialskills.sh/googleworkspace/skills/gws-gmail) - 发送、读取与管理 Gmail 邮件。
- [googleworkspace/gws-calendar](https://officialskills.sh/googleworkspace/skills/gws-calendar) - 管理 Google Calendar 日历与事件。
- [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills) - Obsidian 的 Agent 技能；教你的智能体使用 Obsidian CLI 与 Markdown 等开放格式。
- [notion](https://github.com/makenotion) - Notion 技能（管理工作区与数据库）。
- [resend](https://github.com/resend) - Resend 技能（发送事务邮件）。

## 🎓 研究与教育

- [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) - Claude Code 学术研究技能：研究 → 写作 → 评审 → 修订 → 定稿。
- [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) - 将任意 AI Agent 变为 AI 科学家；排名第一的科学 Agent Skills 库。
- [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill) - 在 Reddit、X、YouTube、HN、Polymarket 与全网研究近 30 天任意主题。
- [googleworkspace/gws-classroom](https://officialskills.sh/googleworkspace/skills/gws-classroom) - 管理 Google Classroom 班级、名册与课程。

## 💰 金融与 Web3

- [stripe/stripe-best-practices](https://officialskills.sh/stripe/skills/stripe-best-practices) - 构建 Stripe 集成的最佳实践。
- [stripe/upgrade-stripe](https://officialskills.sh/stripe/skills/upgrade-stripe) - 升级 Stripe SDK 与 API 版本。
- [binance](https://github.com/binance) - Binance 技能（交易与市场数据）。
- [coinbase](https://github.com/coinbase) - Coinbase 技能（加密与支付）。
- [veniceai/venice-crypto-rpc](https://github.com/veniceai/skills/tree/main/skills/venice-crypto-rpc) - 支持加密网络的 JSON-RPC 代理。
- [internet-court/internet-court-skill](https://github.com/internet-court/internet-court-skill) - Agent 间商业的信任层——自然语言委托与 ERC-7710 授权。

## 🤖 客户端插件

面向特定 AI 编码客户端的插件、扩展与智能体。

- [awesome-opencode/awesome-opencode](https://github.com/awesome-opencode/awesome-opencode) - opencode.ai 的插件、主题、智能体与资源精选列表。
- [Opencode-DCP/opencode-dynamic-context-pruning](https://github.com/Opencode-DCP/opencode-dynamic-context-pruning) - OpenCode 动态上下文裁剪插件，智能管理会话上下文。
- [numman-ali/opencode-openai-codex-auth](https://github.com/numman-ali/opencode-openai-codex-auth) - 通过 ChatGPT Plus/Pro 订阅实现个人编码助手 OAuth 认证插件。
- [jenslys/opencode-gemini-auth](https://github.com/jenslys/opencode-gemini-auth) - OpenCode 的 Gemini 认证插件。
- [tickernelz/opencode-mem](https://github.com/tickernelz/opencode-mem) - 使用本地向量数据库为编码智能体提供持久记忆的 OpenCode 插件。
- [supermemoryai/opencode-supermemory](https://github.com/supermemoryai/opencode-supermemory) - OpenCode 的 Supermemory 插件。
- [jarrodwatts/claude-hud](https://github.com/jarrodwatts/claude-hud) - Claude Code 插件，展示实时状态：上下文用量、活跃工具、运行中的智能体等。
- [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) - 每个智能体的会话间持久上下文。
- [CherryHQ/cherry-studio](https://github.com/CherryHQ/cherry-studio) - 支持智能对话、自主 Agent 与 300+ 助手的 AI 生产力工作台。
- [zhayujie/CowAgent](https://github.com/zhayujie/CowAgent) - 开源超级 AI 助手与 Agent 框架：规划任务、运行工具与技能、自我进化。
- [nanocoai/nanoclaw](https://github.com/nanocoai/nanoclaw) - 运行在容器中的轻量级 OpenClaw 替代品；连接 WhatsApp、Telegram 等。
- [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) - 通过极简输出风格削减约 65% Token 的 Claude Code 技能。

## 🔌 MCP 服务器与集成

- [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - 最流行的 MCP 服务器合集。
- [mcp-use/mcp-use](https://github.com/mcp-use/mcp-use) - 全栈 MCP 框架：为 ChatGPT/Claude 开发 MCP 应用，为 AI Agent 开发 MCP 服务器。
- [IBM/mcp-context-forge](https://github.com/IBM/mcp-context-forge) - 位于任意 MCP、A2A 或 REST/gRPC API 之前的 AI 网关、注册表与代理。
- [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) - 大规模搜索、抓取与交互网页的上下文 API。
- [composiohq/composio](https://github.com/ComposioHQ/composio) - 通过托管认证将 AI Agent 连接到 1000+ 外部应用。
- [superpowers](https://github.com/obra/superpowers) - 作为技能框架的一部分，附带浏览器、记忆等 MCP 服务器。
- [rohitg00/awesome-devops-mcp-servers](https://github.com/rohitg00/awesome-devops-mcp-servers) - 面向 DevOps 的 MCP 服务器精选。

## 🌐 社区与多框架

- [wshobson/agents](https://github.com/wshobson/agents) - 多框架 Agentic 插件市场：Claude Code、Codex CLI、Cursor、OpenCode、GitHub Copilot。
- [VoltAgent/awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) - OpenClaw 技能精选合集：筛选并分类了 5,400+ 技能。
- [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) - 触手可及的完整 AI 代理机构。
- [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) - 面向 Claude Code 与 AI Agent 的营销技能。
- [phuryn/pm-skills](https://github.com/phuryn/pm-skills) - 包含 100+ Agentic 技能的 PM 技能市场。

## 🇨🇳 中文资源

中文相关的 Agent 技能与 MCP 资源。

- [yzfly/Awesome-MCP-ZH](https://github.com/yzfly/Awesome-MCP-ZH) - MCP 资源精选：MCP 指南、Claude MCP、MCP Servers、MCP Clients。
- [zhayujie/CowAgent](https://github.com/zhayujie/CowAgent) - 开源超级 AI 助手与 Agent 框架：规划任务、运行工具和技能、自我进化。
- [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) - 100+ AI Agents、Agent Skills 与 RAG 应用（开源）。
- [volcengine/OpenViking](https://github.com/volcengine/OpenViking) - 面向 AI Agent 的自进化上下文数据库，统一记忆、知识 RAG 与技能。
- [CherryHQ/cherry-studio](https://github.com/CherryHQ/cherry-studio) - 支持智能对话、自主 Agent 与 300+ 助手的 AI 生产力工作台。

---

## 参与贡献

非常欢迎你的贡献！请先阅读 [CONTRIBUTING.md](CONTRIBUTING.md) 指南，然后提交 Pull Request 来添加新插件或改进现有条目。

列表中所有插件均经过 **GitHub 检索与验证**，并按行业/功能分类。如果你维护着优秀的 Agent 插件并希望收录，欢迎联系我们。

## 许可证

本项目基于 [MIT 许可证](LICENSE) 发布。

列表中列出的插件归其各自所有者所有，并遵循其各自的许可证。

---

<p align="center">献给 Agent Plugins 社区 💛</p>
