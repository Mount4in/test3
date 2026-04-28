# Testing Guide

## Running Tests

```bash
# All tests
npm test

# Unit tests only
npm run test:unit

# Integration tests
npm run test:integration

# With coverage
npm run test:coverage
```

## Writing Tests

### Unit Tests

Place unit tests next to the file they test:
```
src/util/format.ts
src/util/format.test.ts
```

### Integration Tests

Place integration tests in `tests/integration/`:
```
tests/integration/api.test.ts
tests/integration/auth.test.ts
```

## Mocking

Use `vi.mock()` for module mocking:
```typescript
vi.mock("../database", () => ({
  query: vi.fn().mockResolvedValue([]),
}))
```
