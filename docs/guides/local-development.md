# Local Development Setup

## System Requirements

- macOS 12+, Ubuntu 22.04+, or Windows 11 with WSL2
- 8GB RAM minimum
- 10GB free disk space

## IDE Setup

### VS Code (Recommended)

Install recommended extensions:
```
code --install-extension dbaeumer.vscode-eslint
code --install-extension esbenp.prettier-vscode
code --install-extension bradlc.vscode-tailwindcss
```

### JetBrains

Enable TypeScript service and ESLint integration in settings.

## First-Time Setup

```bash
# Clone and install
git clone <repo-url>
cd <project>
npm install

# Setup local services
docker-compose -f config/templates/docker-compose.dev.yml up -d

# Initialize database
npm run db:migrate
npm run db:seed

# Start development server
npm run dev
```

## Useful Commands

| Command          | Description               |
|-----------------|---------------------------|
| `npm run dev`   | Start dev server          |
| `npm test`      | Run test suite            |
| `npm run lint`  | Run linter                |
| `npm run build` | Production build          |
| `npm run clean` | Remove build artifacts    |
