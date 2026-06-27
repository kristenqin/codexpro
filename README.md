<p align="center">
  <img src="docs/favicon.svg" width="72" height="72" alt="CodexPro logo">
</p>

<h1 align="center">CodexPro</h1>

<p align="center">
  Use ChatGPT like your local coding agent for one token-protected workspace.
</p>

<p align="center">
  <a href="https://www.npmjs.com/package/codexpro"><img alt="npm" src="https://img.shields.io/npm/v/codexpro?style=flat-square"></a>
  <a href="https://github.com/rebel0789/codexpro/actions"><img alt="CI" src="https://img.shields.io/github/actions/workflow/status/rebel0789/codexpro/ci.yml?branch=main&style=flat-square"></a>
  <a href="https://github.com/rebel0789/codexpro/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/github/license/rebel0789/codexpro?style=flat-square"></a>
  <a href="https://rebel0789.github.io/codexpro/"><img alt="Website" src="https://img.shields.io/badge/site-GitHub%20Pages-67e8f9?style=flat-square"></a>
</p>

<p align="center">
  <a href="https://rebel0789.github.io/codexpro/">Website</a>
  ·
  <a href="docs/README_ZH.md">中文 README</a>
  ·
  <a href="https://rebel0789.github.io/codexpro/zh.html">中文网站</a>
  ·
  <a href="https://github.com/rebel0789/codexpro">Star on GitHub</a>
  ·
  <a href="https://www.npmjs.com/package/codexpro">npm</a>
  ·
  <a href="docs/DOMAIN_SETUP.md">Stable URL guide</a>
  ·
  <a href="docs/FAQ.md">FAQ</a>
  ·
  <a href="docs/SECURITY.md">Security</a>
</p>

## Quick Start

Install the CLI:

```bash
npm install -g codexpro
```

Then run setup inside the repo you want ChatGPT to work on:

```bash
cd /path/to/your/repo
codexpro setup
```

CodexPro copies the ChatGPT Server URL for you. In ChatGPT, open `Settings -> Apps -> Advanced settings -> Create app`, paste that URL, and choose `Authentication: No Authentication / None`.

After setup, daily use from the same repo is just:

```bash
codexpro start
```

## Documentation

- **[Full README](docs/README.md)** - Complete feature guide and usage reference
- **[FAQ](docs/FAQ.md)** - Frequently asked questions
- **[中文 README](docs/README_ZH.md)** - Chinese documentation
- **[中文 FAQ](docs/FAQ_ZH.md)** - Chinese FAQ
- **[Domain Setup](docs/DOMAIN_SETUP.md)** - Setting up stable URLs with ngrok or Cloudflare
- **[Security](docs/SECURITY.md)** - Security policy and threat model
- **[Contributing](docs/CONTRIBUTING.md)** - Contribution guidelines
- **[Changelog](docs/CHANGELOG.md)** - Version history
- **[Launch Checklist](docs/PUBLIC_LAUNCH_CHECKLIST.md)** - Release and launch checklist
- **[Design](docs/design.md)** - Design system and principles

## Examples & Configuration

- **[AGENTS.md Example](config/AGENTS.example.md)** - Instructions for ChatGPT and Codex
- **[Config Example](config/config.example.env)** - Environment variable reference
- **[ChatGPT Prompt](config/CHATGPT_PROMPT.md)** - Suggested ChatGPT prompt
- **[Codex Prompt](config/CODEX_PROMPT.md)** - Suggested Codex prompt

## About CodexPro

CodexPro is a local MCP/App SDK-style connector that lets ChatGPT inspect, edit, and hand off work to Codex inside a local dev workspace.

### What it is:
- A local MCP bridge for the workspace you choose
- A way for ChatGPT Developer Mode to inspect, edit, verify, and hand off work
- A repo-backed context system using explicit files such as `AGENTS.md` and `.ai-bridge`
- A developer tool with conservative defaults

### What it is NOT:
- A hosted coding service
- A model unlock, proxy, resale layer, or quota workaround
- Permanent ChatGPT memory across every chat
- An OS sandbox or substitute for repo/terminal judgment

### Requirements
- Node.js 20+
- ChatGPT Plus or Pro account with Apps / Developer Mode access

## License

MIT
