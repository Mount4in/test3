# Architecture Overview

## Directory Structure

```
src/
├── cli/          # CLI entry points
├── components/   # Shared components
├── config/       # Configuration management
├── core/         # Core business logic
├── git/          # Git integration
├── providers/    # AI provider integrations
├── tool/         # Tool implementations
└── util/         # Utility functions
```

## Key Patterns

### Dependency Injection
Components receive dependencies via constructor injection.

### Event-Driven Architecture
The system uses an event bus for loose coupling between modules.

### Repository Pattern
Data access is abstracted through repository interfaces.

## Data Flow

1. CLI parses user input
2. Core processes the request
3. Providers handle AI interactions
4. Tools execute actions
5. Results flow back through the chain
