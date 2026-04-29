# Configuration Variables Reference

## Environment Variables

| Variable              | Required | Default  | Description                |
|----------------------|----------|----------|----------------------------|
| `NODE_ENV`           | No       | dev      | Runtime environment        |
| `PORT`               | No       | 3000     | Server port                |
| `LOG_LEVEL`          | No       | info     | Logging verbosity          |
| `DATABASE_URL`       | Yes      | -        | PostgreSQL connection URL  |
| `REDIS_URL`          | No       | -        | Redis connection URL       |
| `API_KEY`            | Yes      | -        | API authentication key     |
| `SESSION_SECRET`     | Yes      | -        | Session encryption secret  |

## Feature Flags

| Flag                 | Default | Description                   |
|---------------------|---------|-------------------------------|
| `ENABLE_CACHE`      | true    | Enable response caching       |
| `ENABLE_METRICS`    | false   | Enable Prometheus metrics     |
| `ENABLE_RATE_LIMIT` | true    | Enable API rate limiting      |
