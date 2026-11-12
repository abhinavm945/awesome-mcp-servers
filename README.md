# Awesome MCP Servers & Tools [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated directory of production-grade **Model Context Protocol (MCP)** servers, developer tools, and client configurations for **Cursor IDE**, **Anthropic Claude Desktop**, **Codeium Windsurf**, and autonomous AI agents.

The **Model Context Protocol (MCP)** is an open standard introduced by Anthropic that connects frontier Large Language Models to local databases, developer tools, internal file systems, and external APIs.

---

## ⚡ 1-Click Installation & Package Management

The fastest way to discover, configure, and install any MCP server listed here is using the open-source **[AIStoreHub CLI](https://www.aistorehub.in/cli)** (`pip install aistorehub`):

```bash
# 1. Install package manager
pip install aistorehub

# 2. Inject verified tools directly into your editor
aihub mcp install community/postgres-mcp --client cursor
aihub mcp install @modelcontextprotocol/server-filesystem --client claude
aihub mcp install community/sqlite-mcp --client windsurf

# 3. View all active servers
aihub list --client cursor
```

*Automates schema validation, resolves non-login `$PATH` binary bugs, and creates timestamped safety backups of your config files before modifying them.*

Explore the full interactive registry at **[https://www.aistorehub.in](https://www.aistorehub.in)**.

* **[AIStoreHub MCP Server Catalog](https://www.aistorehub.in/categories/mcp-servers)** — 250+ community-verified tools with 1-click install.
* **[Omniroute Multi-LLM Router](https://www.aistorehub.in/community/catalog/omniroute)** — Dynamic model fallback and latency-optimized routing.
* **[Super Video Maker](https://www.aistorehub.in/community/catalog/super-video-maker-skill)** — Autonomous video composition and timeline stitching pipeline.
* **[PostgreSQL Inspector](https://www.aistorehub.in/community/catalog/mcp-server-postgres)** — Real-time schema discovery and SQL migration testing.
* **[Filesystem MCP](https://www.aistorehub.in/community/catalog/mcp-filesystem)** — Sandboxed directory execution for Cursor and Claude.

---

## 📋 Contents

- [Registries & Discovery Platforms](#-registries--discovery-platforms)
- [Databases & Storage](#-databases--storage)
- [Developer Tools & Version Control](#-developer-tools--version-control)
- [Web Browsing & Real-Time Search](#-web-browsing--real-time-search)
- [Filesystem & Local Workflows](#-filesystem--local-workflows)
- [Productivity & Communication](#-productivity--communication)
- [Supported MCP Clients](#-supported-mcp-clients)
- [Troubleshooting & Debugging Playbook](#-troubleshooting--debugging-playbook)
- [Contributing](#-contributing)

---

## 🌐 Registries & Discovery Platforms

- **[AIStoreHub](https://www.aistorehub.in)** — Open registry and 1-click Python package manager (`pip install aistorehub`) for verified MCP servers, autonomous agents, and tool manifests with automated backups for Cursor, Claude Desktop, and Windsurf.
- **[Model Context Protocol Registry](https://github.com/modelcontextprotocol)** — Official reference server implementations managed by Anthropic.
- **[Smithery](https://smithery.ai)** — Directory of community-hosted MCP servers.

---

## 💾 Databases & Storage

Tools that enable AI models to inspect schemas, execute safe `SELECT` queries, and draft migrations.

- **[PostgreSQL MCP](https://www.aistorehub.in/search?q=postgres)** (`@modelcontextprotocol/server-postgres`) — Connect Claude or Cursor directly to PostgreSQL databases. Read schemas, view table relations, and execute analytical SQL.
  ```bash
  aihub mcp install @modelcontextprotocol/server-postgres --client cursor
  ```
- **[SQLite Local](https://www.aistorehub.in/search?q=sqlite)** (`mcp-server-sqlite`) — Inspect, query, and modify local `.db` and `.sqlite` files safely.
  ```bash
  aihub mcp install mcp-server-sqlite --client cursor
  ```
- **[Supabase MCP](https://www.aistorehub.in/search?q=supabase)** (`@supabase/mcp-server-supabase`) — Query Supabase PostgreSQL databases, inspect Auth user tables, and monitor Edge Functions.
- **[Redis MCP](https://www.aistorehub.in/search?q=redis)** (`mcp-server-redis`) — Real-time key inspection, hash map debugging, and cache invalidation.
- **[MySQL MCP Server](https://www.aistorehub.in/search?q=mysql)** (`mcp-server-mysql`) — MySQL schema inspection and query runner with read-only guardrails.

---

## 🛠️ Developer Tools & Version Control

Tools that give coding agents active terminal and repository awareness.

- **[GitHub MCP](https://www.aistorehub.in/search?q=github)** (`@modelcontextprotocol/server-github`) — Search codebases across repositories, create branches, inspect commits, and draft Pull Requests.
  ```bash
  aihub mcp install @modelcontextprotocol/server-github --client cursor
  ```
- **[GitLab MCP](https://www.aistorehub.in/search?q=gitlab)** (`@modelcontextprotocol/server-gitlab`) — Full GitLab project inspection, merge request workflows, and pipeline monitoring.
- **[Sentry MCP](https://www.aistorehub.in/search?q=sentry)** (`@modelcontextprotocol/server-sentry`) — Retrieve real-time production stack traces, error issues, and unresolved crash reports.
- **[Docker MCP](https://www.aistorehub.in/search?q=docker)** — List running containers, inspect Docker compose topologies, and tail container logs.
- **[Linear MCP](https://www.aistorehub.in/search?q=linear)** — Read active team sprints, update issue statuses, and link PRs to engineering tickets.

---

## 🔍 Web Browsing & Real-Time Search

Give local LLMs real-time access to live web pages and documentation.

- **[Brave Search MCP](https://www.aistorehub.in/search?q=brave)** (`@modelcontextprotocol/server-brave-search`) — Execute real-time web searches and news queries without ad tracking or paywall limits.
  ```bash
  aihub mcp install @modelcontextprotocol/server-brave-search --client claude
  ```
- **[Puppeteer Browser](https://www.aistorehub.in/search?q=puppeteer)** (`@modelcontextprotocol/server-puppeteer`) — Headless Chrome automation for navigating SPAs, taking full-page screenshots, and scraping dynamic JavaScript content.
- **[Fetch MCP](https://www.aistorehub.in/search?q=fetch)** (`@modelcontextprotocol/server-fetch`) — Fetch, sanitize, and convert raw HTML pages directly into clean LLM-friendly Markdown.
- **[Firecrawl MCP](https://www.aistorehub.in/search?q=firecrawl)** — Deep web scraping and multi-page crawl engine for LLM documentation indexing.

---

## 📁 Filesystem & Local Workflows

- **[Filesystem MCP](https://www.aistorehub.in/search?q=filesystem)** (`@modelcontextprotocol/server-filesystem`) — Secure local file manipulation across selected directories with path-traversal sandboxing.
  ```bash
  aihub mcp install @modelcontextprotocol/server-filesystem --client claude
  ```
- **[Memory MCP](https://www.aistorehub.in/search?q=memory)** (`@modelcontextprotocol/server-memory`) — Persistent knowledge graph memory across distinct chat sessions.
- **[Google Drive MCP](https://www.aistorehub.in/search?q=drive)** — Search, read, and export documents, spreadsheets, and slides directly into agent context.

---

## 💬 Productivity & Communication

- **[Slack MCP](https://www.aistorehub.in/search?q=slack)** (`@modelcontextprotocol/server-slack`) — Read channel message histories, draft messages, and search Slack workspace threads.
- **[Discord MCP](https://www.aistorehub.in/search?q=discord)** — Community bot management and server channel search.
- **[Notion MCP](https://www.aistorehub.in/search?q=notion)** — Read and write to Notion databases, engineering wikis, and design specs.

---

## 🖥️ Supported MCP Clients

| Client | Config File Location | Quick Setup Command |
| :--- | :--- | :--- |
| **Cursor IDE** | `~/.cursor/mcp.json` | `aihub mcp install <server> --client cursor` |
| **Claude Desktop (macOS)** | `~/Library/Application Support/Claude/claude_desktop_config.json` | `aihub mcp install <server> --client claude` |
| **Claude Desktop (Win)** | `%APPDATA%\Claude\claude_desktop_config.json` | `aihub mcp install <server> --client claude` |
| **Codeium Windsurf** | `~/.codeium/windsurf/mcp_config.json` | `aihub mcp install <server> --client windsurf` |

---

## 🔧 Troubleshooting & Debugging Playbook

Encountering a red status indicator or a crash? Here are the top 3 failure modes:

1. **Stdout Stream Contamination (`Connection closed`)**:
   * *Problem*: If an MCP server prints non-JSON text (`console.log()` or `print()`) to standard output, it breaks the JSON-RPC message framing.
   * *Fix*: Route all logs strictly to `stderr` (`console.error` in Node, `sys.stderr.write` in Python).
2. **Missing Binary Path (`spawn npx ENOENT`)**:
   * *Problem*: GUI applications (Claude Desktop) do not inherit your terminal's shell `$PATH`.
   * *Fix*: Use absolute paths: `/opt/homebrew/bin/npx` (macOS) or `C:\Program Files\nodejs\npx.cmd` (Windows).
3. **Trailing Commas in JSON**:
   * *Problem*: Standard JSON parsers reject trailing commas after the last item.
   * *Fix*: Run `python -m json.tool <config-file>` or let `aihub mcp install` validate schemas automatically.

Read our complete technical handbooks on AIStoreHub:
* **[Top 25 Model Context Protocol Servers Handbook (2026)](https://www.aistorehub.in/blog/top-mcp-servers-cursor-claude-2026)**
* **[How to Build an MCP Server with Python FastMCP](https://www.aistorehub.in/blog/how-to-build-python-mcp-server-fastmcp)**
* **[Where is claude_desktop_config.json? Exact Paths for Windows & Mac](https://www.aistorehub.in/blog/claude-desktop-mcp-setup-troubleshooting-guide)**
* **[How to Add & Configure MCP in Cursor: Complete mcp.json Setup Guide](https://www.aistorehub.in/blog/cursor-mcp-setup-guide-troubleshooting-tools)**
* **[Fixing MCP Error -32000 Connection Closed & Exit Code 1 Errors](https://www.aistorehub.in/blog/mcp-connection-closed-exit-code-debugging-guide)**

---

## 🤝 Contributing

Contributions are warmly welcomed!

To submit a new MCP server or tool to this list:
1. Fork this repository.
2. Add your server under the appropriate category in alphabetical order.
3. Ensure your server includes a clear description, repository link, and install snippet.
4. Submit a Pull Request.

---

## 📄 License

This repository is licensed under the [MIT License](LICENSE).
