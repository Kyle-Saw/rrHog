# rrHog — OSS Web Analytics & Session Replay (rrweb + ClickHouse)

> Open-source, self-hosted web analytics & session monitoring built on **rrweb** with **async ingestion** for rock-solid reliability.  
> Stack: **FastAPI** (ingest/read) • **NATS JetStream** (queue) • **ClickHouse** (events) • **Postgres** (meta) • **Next.js** (UI)

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Docs](https://img.shields.io/badge/docs-Architecture-brightgreen)](ARCHITECTURE.md)
[![Good First Issues](https://img.shields.io/github/labels/YOUR_ORG/rrHog/good%20first%20issue)](#)

**Why rrHog?** Most analytics pipelines lose data when DBs or networks hiccup. rrHog **ACKs fast** and persists to a **durable queue** first, so ingestion keeps flowing even if storage is down.

## Features
- 🌀 **Async ingest** → instant `202` to clients
- 🎥 **Session replay** with rrweb & rrweb-player
- ⚡ **ClickHouse** analytics (blazing-fast queries)
- 🧰 **Next.js** dashboard (App Router)
- 🐳 **Docker Compose** one-box deploy
- 🔒 Per-project keys, rate limits, and basic PII guards

## Quick start (high level)
1. `docker compose up -d` (services: nginx, nats, clickhouse, postgres, api, worker, web)
2. Create a project → get **WRITE** and **READ** keys.
3. Add rrweb snippet to your site and post batched segments to `/i`.

See **[ARCHITECTURE.md](ARCHITECTURE.md)** for schemas, mermaid diagrams, and example API/worker snippets.

## Repo metadata (GitHub)
- **Description:** `rrHog — Open-source, self-hosted web analytics & session replay built on rrweb. FastAPI + NATS JetStream + ClickHouse, Next.js UI.`
- **Topics (11):** `open-source, self-hosted, web-analytics, session-replay, session-recording, rrweb, clickhouse, fastapi, nats-jetstream, postgresql, nextjs`

## Community
- Start here: [CONTRIBUTING.md](CONTRIBUTING.md)
- Code of Conduct: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
- Support: [SUPPORT.md](SUPPORT.md)
- Roadmap: [ROADMAP.md](ROADMAP.md)

## Security
Please report vulnerabilities privately — see [SECURITY.md](SECURITY.md).

## License
MIT © 2025 You & Contributors — see [LICENSE](LICENSE).

> 💖 Want to support? Add a **GitHub Sponsors** button by creating `.github/FUNDING.yml` later.
