[<img width="150" height="150" alt="image" src="https://github.com/user-attachments/assets/50293d6f-3b8a-45f0-ae2a-84ea80042396" />
](https://avatars.githubusercontent.com/u/284823564?s=200&v=4)

# PgShift

**Start with Postgres. Shift only when you must.**

Most teams add Redis, Kafka, Elasticsearch, and Pinecone before they actually need them. The result is distributed infrastructure that costs more to operate than the product earns.

PostgreSQL already handles most of what those services do. PgShift gives you a clean API on top of those capabilities — and tells you exactly when it is time to move on.

---

## Modules

| Package | Replaces | Postgres primitive |
|---|---|---|
| [`@pgshift/search`](https://github.com/pgshift/pgshift/tree/main/packages/search) | Elasticsearch, Typesense | TSVector + pg_trgm |
| [`@pgshift/cache`](https://github.com/pgshift/pgshift/tree/main/packages/cache) | Redis (read-heavy) | Materialized views |
| [`@pgshift/queue`](https://github.com/pgshift/pgshift/tree/main/packages/queue) | BullMQ, SQS, RabbitMQ | SKIP LOCKED |
| [`@pgshift/cron`](https://github.com/pgshift/pgshift/tree/main/packages/cron) | EventBridge, cron services | pg_cron |
| [`@pgshift/vector`](https://github.com/pgshift/pgshift/tree/main/packages/vector) | Pinecone, Weaviate | pgvector + HNSW |
| [`@pgshift/state`](https://github.com/pgshift/pgshift/tree/main/packages/state) | Custom trigger logic | Triggers + RLS |
| [`@pgshift/workflow`](https://github.com/pgshift/pgshift/tree/main/packages/workflow) | Temporal, Step Functions | SKIP LOCKED + JSONB |

---

## Links

- **Docs** — [pgshift.dev](https://pgshift.dev)
- **npm** — [npmjs.com/~pgshift](https://www.npmjs.com/~pgshift)
- **License** — MIT
