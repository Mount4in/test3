# Release Process

## Versioning

We follow semantic versioning (SemVer):
- MAJOR: Breaking changes
- MINOR: New features (backwards compatible)
- PATCH: Bug fixes

## Release Steps

1. Create release branch: `release/v1.2.3`
2. Update CHANGELOG.md
3. Bump version in package.json
4. Create PR to main
5. After merge, tag the release
6. CI publishes to npm automatically

## Hotfix Process

1. Branch from latest release tag
2. Apply fix
3. Create PR to main AND release branch
