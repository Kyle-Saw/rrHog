# Contributing to rrHog

Thanks for considering a contribution! 🙌

## Ground rules
- We use **MIT** license. By contributing, you agree your contribution is licensed under MIT.
- Follow **Conventional Commits** (`feat:`, `fix:`, `docs:`, `chore:`…).
- Keep PRs focused and add/adjust tests where it makes sense.

## How to start
1. Comment on an issue (look for **good first issue** / **help wanted**).
2. Discuss design for non-trivial changes.
3. Open a draft PR early for feedback.

## Dev quickstart (high level)
- API: FastAPI (Python 3.11)  
- Worker: Python asyncio consumer  
- Web: Next.js (Node 20+)  
- Storage: ClickHouse & Postgres  
- Queue: NATS JetStream

## Testing
- Prefer small, deterministic tests.
- Add fixtures for sample rrweb batches.

## Code style
- Python: black + ruff
- TS/JS: eslint + prettier

## Community
Be kind, be constructive. See our [Code of Conduct](CODE_OF_CONDUCT.md).