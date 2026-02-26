# Shinkaimon Hub Deploy

Docker Compose deployment for [shinkaimon-hub](https://hub.docker.com/r/polylvst/shinkaimon-hub) (backend), [shinkaimon-hub-fe](https://hub.docker.com/r/polylvst/shinkaimon-hub-fe) (frontend), and PostgreSQL with pgvector.

## Quick Start

```bash
docker compose up -d
```

Frontend will be available at `http://localhost:3001`.

## Services

| Service | Port | Description |
|---|---|---|
| shinkaimon-hub | 8001 | FastAPI backend |
| shinkaimon-hub-fe | 3001 | SvelteKit frontend (nginx) |
| hub-db | 5433 | PostgreSQL 16 with pgvector |

## Data

- `hub_pgdata` — PostgreSQL data (Docker volume)
- `.deepface/` — Face recognition model cache
