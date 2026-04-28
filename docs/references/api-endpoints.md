# API Reference

## Authentication

All API requests require authentication via Bearer token:
```
Authorization: Bearer <token>
```

## Endpoints

### GET /api/health
Health check endpoint.

Response: `200 OK`
```json
{ "status": "healthy", "version": "1.0.0" }
```

### POST /api/sessions
Create a new session.

Request:
```json
{
  "model": "claude-sonnet-4-20250514",
  "context": "optional context string"
}
```

### GET /api/sessions/:id
Get session details.

### DELETE /api/sessions/:id
End a session.
