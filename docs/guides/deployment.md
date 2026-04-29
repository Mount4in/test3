# Deployment Guide

## Environments

| Environment | Branch   | URL                        |
|------------|----------|----------------------------|
| Development | dev     | dev.example.com            |
| Staging     | staging | staging.example.com        |
| Production  | main    | app.example.com            |

## CI/CD Pipeline

Deployments are automated via GitHub Actions:
1. Push to branch triggers build
2. Tests run in parallel
3. Successful builds deploy to corresponding environment

## Manual Deployment

In rare cases where manual deployment is needed:
```bash
npm run build
npm run deploy -- --env staging
```

## Rollback

To rollback to a previous version:
```bash
npm run deploy:rollback -- --env production --version <tag>
```
