# Code Style Guide

## TypeScript

- Use `const` by default, `let` when needed
- Prefer interfaces over types for objects
- Use explicit return types on exported functions
- Avoid `any` - use `unknown` if the type is truly unknown

## Formatting

We use Prettier with the following config:
```json
{
  "semi": false,
  "singleQuote": false,
  "trailingComma": "all",
  "printWidth": 120
}
```

## Naming Conventions

- Files: `kebab-case.ts`
- Classes: `PascalCase`
- Functions/variables: `camelCase`
- Constants: `UPPER_SNAKE_CASE`
- Types/Interfaces: `PascalCase`

## Imports

Order imports as:
1. Node built-ins
2. External packages
3. Internal modules
4. Relative imports
