<p align="center">
  <a href="https://pullminder.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://pullminder.com/favicon.svg">
      <img src="https://pullminder.com/favicon.svg" height="64" alt="Pullminder">
    </picture>
  </a>
</p>

<h3 align="center">A verification layer for AI-assisted pull requests</h3>

<p align="center">
  Risk scores · Reviewer briefs · Policy enforcement · CLI-first analysis · GitHub-native
</p>

<p align="center">
  <a href="https://pullminder.com"><strong>Website</strong></a> · <a href="https://docs.pullminder.com"><strong>Docs</strong></a> · <a href="https://pullminder.com/trial"><strong>Start Free Trial</strong></a>
</p>

---

AI makes writing code 10x faster — but it makes reviewing code 10x harder. Teams are drowning in high-volume, low-trust pull requests that bypass critical security and architectural checks.

**Pullminder** sits between your AI IDE and your production branch. It analyzes every PR and returns a risk score, reviewer brief, flagged issues, and policy outcome — fitting naturally into existing GitHub workflows.

### What Pullminder does

- **Risk Scoring** — 8 heuristic analyzers evaluate each PR for security flaws, complexity, test coverage gaps, and AI-generated content patterns
- **Reviewer Briefs** — AI-generated summaries that tell reviewers exactly what to focus on, cutting review time in half
- **Policy Engine** — Enforce team rules with composable YAML rule packs from an open registry of 25 detection and policy packs
- **CLI-First Analysis** — Run rule packs offline against local diffs or remote PRs from your terminal. SARIF, JUnit, and GitHub annotation output for CI integration
- **AI Agent Interop** — Every CLI command supports `--agent` for structured JSON output, making Pullminder a tool for Copilot, Claude Code, Cursor, and other AI coding agents
- **GitHub-Native** — Runs as a GitHub App with Check Runs, PR comments, and status checks. Nothing to install on your machine

### Works with every AI coding tool

Pullminder analyzes PRs from **GitHub Copilot**, **Cursor**, **Claude Code**, **Windsurf**, and any other tool that opens pull requests.

### Get started

```bash
# Install the CLI
brew install pullminder/tap/pullminder

# Initialize your project
pullminder init

# Analyze your current branch (offline, zero config)
pullminder check
```

### Use as a GitHub Action

```yaml
- uses: pullminder/action@v1
```

### Open source

| Repository | Description |
|---|---|
| [cli](https://github.com/pullminder/cli) | Cross-platform CLI with 13 commands for local and remote PR analysis |
| [registry](https://github.com/pullminder/registry) | Official rule pack registry — 25 detection and policy packs |
| [npm](https://github.com/pullminder/npm) | npm wrapper for the CLI |
| [homebrew-tap](https://github.com/pullminder/homebrew-tap) | Homebrew tap for macOS/Linux |
| [action](https://github.com/pullminder/action) | GitHub Action for CI integration |
| [.github](https://github.com/pullminder/.github) | Org profile and community health files |
