# enthus GmbH — Application Development

Open-source developer tools from **enthus GmbH** — CLIs, GitHub Actions, container images, and Helm charts, all designed to be driven equally well by humans and LLM agents. Battle-tested in our own production stack.

## Command-line tools

Four CLIs with a shared design philosophy: **equally usable by humans and LLM agents**. Every command supports `--json`, context switching works the same way across all four, help text and error codes are stable, nothing is interactive by default, and every release ships multi-platform binaries (darwin / linux / windows × amd64 / arm64).

| CLI | What it does |
|---|---|
| [**atl-cli**](https://github.com/enthus-appdev/atl-cli) | Jira and Confluence from your terminal — a CLI alternative to the Atlassian MCP |
| [**esq-cli**](https://github.com/enthus-appdev/esq-cli) | Query and inspect Elasticsearch with multi-cluster context switching |
| [**n8n-cli**](https://github.com/enthus-appdev/n8n-cli) | Manage n8n workflows: pull, push, execute, activate |
| [**gh-attach**](https://github.com/enthus-appdev/gh-attach) | `gh` extension for pasting screenshots directly into PRs and issues |

## GitHub Actions & CI

| Repo | What it is |
|---|---|
| [**oss-actions**](https://github.com/enthus-appdev/oss-actions) | Reusable GitHub Actions for open-source projects — npm and Go license validators today, more to come |
| [**github-actions-runner**](https://github.com/enthus-appdev/github-actions-runner) | Actions Runner Controller (ARC) image with `curl`, `wget`, `git`, and `rsync` pre-installed — daily-rebuilt and cosign-signed |

## Container images & Helm charts

| Repo | What it is |
|---|---|
| [**docker-elasticsearch-icu**](https://github.com/enthus-appdev/docker-elasticsearch-icu) | Elasticsearch image with the `analysis-icu` plugin pre-installed (~27s saved per CI run) |
| [**helm-charts**](https://github.com/enthus-appdev/helm-charts) | Helm charts published at [`enthus-appdev.github.io/helm-charts`](https://enthus-appdev.github.io/helm-charts) — deployment charts for APIs, operators, admin UIs, and scheduled jobs |

Add the chart repository with:

```shell
helm repo add enthus https://enthus-appdev.github.io/helm-charts
helm repo update
```

## Getting everything at once

[**llm-cli-setup**](https://github.com/enthus-appdev/llm-cli-setup) is a one-command installer that bootstraps the entire CLI toolkit and wires it up for Claude Code and Codex — the fastest way to try everything at once.

---

Found a bug, want a feature, or built something on top? Open an issue on the relevant repo — we read everything.
