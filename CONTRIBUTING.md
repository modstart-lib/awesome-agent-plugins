# Contributing to Awesome Agent Plugins

First off, thank you for considering contributing! We appreciate every contribution, big or small. 🎉

This guide explains how you can add new agent plugins to the curated list, improve existing entries, or fix issues.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
- [Adding a New Plugin](#adding-a-new-plugin)
- [Entry Format](#entry-format)
- [Category Guidelines](#category-guidelines)
- [Content Quality Guidelines](#content-quality-guidelines)
- [What Gets Accepted](#what-gets-accepted)
- [Pull Request Process](#pull-request-process)
- [Issue Reporting](#issue-reporting)
- [Documentation Style](#documentation-style)

## Code of Conduct

By participating in this project, you agree to maintain a welcoming, inclusive, and respectful environment for everyone. Be kind, be constructive, and assume good faith.

## How to Contribute

There are several ways to contribute:

1. **Add a new plugin** to the README (see below).
2. **Fix typos or broken links** in the existing lists.
3. **Improve descriptions** to be more accurate and useful.
4. **Report broken or dead repositories** by opening an issue.
5. **Suggest a new category** if you notice a gap in the organization.

## Adding a New Plugin

To add a new plugin:

1. **Search first.** Make sure the plugin isn't already listed. Check both the English and Chinese READMEs.
2. **Verify the repository.** Confirm the repository exists on GitHub and is actively maintained (or at least still relevant).
3. **Find the right category.** Choose the category that best matches the plugin's primary function.
4. **Open a Pull Request** with your addition, following the entry format below.

## Entry Format

Every entry follows this format:

```markdown
- [owner/repo](https://github.com/owner/repo) - A concise, factual description of what the plugin does.
```

Guidelines:

- The **link text** should be `owner/repo` (e.g., `VoltAgent/awesome-agent-skills`), not a display name.
- The **description** should be a single sentence, 10-25 words, written in **English** for `README.md` and in **Chinese** for `README.zh-CN.md`.
- Descriptions should state **what the plugin does**, not marketing fluff. Avoid words like "amazing", "incredible", "revolutionary".
- Do not include star counts, contributor counts, or other volatile metrics — they go stale quickly.
- If the plugin belongs to multiple categories, choose the **most relevant one** and mention alternatives in the description.

### Example

```markdown
- [obra/superpowers](https://github.com/obra/superpowers) - An agentic skills framework & software development methodology that works.
```

## Category Guidelines

Plugins are organized by **industry/function**. When in doubt about placement:

1. Read the plugin's own README to understand its primary purpose.
2. Match against the existing category descriptions in the table of contents.
3. If no category fits well, propose a new one in your Pull Request — but prefer existing categories.

Current categories:

| Category | Focus |
| --- | --- |
| 📚 Curated Collections | Aggregated "awesome" lists and directories |
| 🏢 Official Vendor Skills | First-party skills published by tool vendors |
| 🧠 Frameworks & Workflows | Methodologies and skill frameworks |
| 💻 Software Development | Frontend, backend, testing, databases, DevOps |
| 🔐 Security | Security review, auditing, AppSec |
| 🎨 Design & Creative | UI/UX, art, video, image |
| 📈 Marketing & Growth | Copywriting, SEO, growth |
| 📝 Productivity & Documentation | Docs, office, personal productivity |
| 🎓 Research & Education | Academic and scientific |
| 💰 Finance & Web3 | Payments, crypto, trading |
| 🤖 Client Plugins | Client-specific plugins (OpenCode, Claude Code, etc.) |
| 🔌 MCP Servers & Integrations | MCP servers and tool integrations |
| 🌐 Community & Multi-Harness | Cross-harness marketplaces, community skills |
| 🇨🇳 Chinese Resources | Chinese-language resources |

## Content Quality Guidelines

- **Accuracy first.** Only list plugins you can verify exist. If you can't verify a repository, don't add it.
- **Prefer maintained plugins.** A repository with recent activity is more useful to readers than an abandoned one. (One-off scripts that are still referenced are acceptable.)
- **No duplicates.** Keep one entry per plugin, in the most fitting category.
- **Keep it stable.** Links must be permanent. Do not link to temporary URLs, commit hashes, or branches that may change.
- **No promotional content.** This list is curated for usefulness, not as a marketing channel.

## What Gets Accepted

We accept:

- ✅ Agent Skills, skills frameworks, and skill collections.
- ✅ MCP servers, MCP frameworks, and MCP-related tooling.
- ✅ Plugin marketplaces and multi-harness plugin collections.
- ✅ Client-specific plugins and extensions (OpenCode, Claude Code, Cursor, Gemini CLI, etc.).
- ✅ Agent workflows, methodologies, and prompt/packaging frameworks.
- ✅ Anything that packages reusable components for AI agents.

We do **not** accept:

- ❌ Commercial products without a meaningful open-source component.
- ❌ Repositories that are only tutorials or documentation (no reusable components).
- ❌ Malicious, deceptive, or low-quality AI-generated filler repositories.
- ❌ Anything that violates the [Agent Plugins](https://agent-plugins.org/) spirit of open, portable standards.

## Pull Request Process

1. **Fork** the repository and create a new branch: `git checkout -b add/plugin-name`.
2. **Make your changes** — add the entry in the correct position within the correct category, in **both** `README.md` (English) and `README.zh-CN.md` (Chinese).
3. **Keep entries alphabetical** within each category (case-insensitive, by `owner/repo`).
4. **Run the link check** if you can (e.g., `npx markdown-link-check README.md`) and fix any broken links.
5. **Commit** with a clear message, e.g., `Add: VoltAgent/awesome-agent-skills`.
6. **Push** and open a Pull Request against the `main` branch.
7. In your PR description, briefly explain **why** this plugin deserves to be listed and in which category.

> Tip: small, focused PRs (1-3 additions) are reviewed and merged much faster than large ones.

## Issue Reporting

When opening an issue, please include:

- **Broken link:** the exact URL and which section it's in.
- **Wrong category:** the plugin URL, current category, and your suggested category.
- **Outdated description:** the plugin URL and the current vs. suggested description.
- **New plugin suggestion:** the GitHub URL and a short description (you can still open a PR instead).

## Documentation Style

- Keep the two READMEs **in sync**: every entry in `README.md` must have its Chinese counterpart in `README.zh-CN.md`, and vice versa.
- Preserve the markdown formatting: one entry per line, no wrapping into multiple lines.
- Use the exact category heading style (emoji + title) when adding a new category.
- Never change the license or contribution headers without opening a discussion first.

---

Again, thank you for contributing! Every entry you add helps someone discover a better way to extend their AI agents. 💛
