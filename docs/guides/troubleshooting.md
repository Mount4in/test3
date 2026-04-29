# Troubleshooting

Common issues and their solutions.

## Build Failures

### Missing dependencies

```
Error: Cannot find module 'xyz'
```

Solution: Run `npm install` to install missing packages.

### Node version mismatch

Ensure you're using Node.js 18+:
```bash
node --version
```

### Port already in use

```bash
lsof -i :3000
kill -9 <PID>
```

## Test Failures

### Timeout errors

Increase the test timeout in your config:
```json
{
  "testTimeout": 30000
}
```

### Database connection errors

Verify your local database is running and credentials match `.env.local`.
