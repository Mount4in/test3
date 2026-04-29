# Error Codes Reference

## Application Errors

| Code     | Message              | Resolution                        |
|----------|---------------------|-----------------------------------|
| `E001`   | Auth failed         | Check API key is valid            |
| `E002`   | Session expired     | Create new session                |
| `E003`   | Rate limited        | Wait and retry with backoff       |
| `E004`   | Invalid input       | Check request body format         |
| `E005`   | Resource not found  | Verify resource ID                |
| `E006`   | Conflict            | Resolve conflicting state         |
| `E007`   | Internal error      | Contact support with request ID   |

## Database Errors

| Code     | Message              | Resolution                        |
|----------|---------------------|-----------------------------------|
| `D001`   | Connection failed   | Check DATABASE_URL                |
| `D002`   | Migration failed    | Check migration files             |
| `D003`   | Query timeout       | Optimize query or increase limit  |
