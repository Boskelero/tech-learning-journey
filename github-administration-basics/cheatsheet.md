# GitHub Administration Cheat Sheet

## Repository Roles

| Role | Permissions |
|--------|--------|
| Read | View repositories |
| Triage | Manage issues and pull requests |
| Write | Push code and manage content |
| Maintain | Manage repository without destructive actions |
| Admin | Full repository control |

---

## Branch Protection

Recommended settings:

- Require pull requests before merging
- Require approvals
- Require status checks
- Block force pushes
- Restrict branch deletion

---

## Organizations

Organizations allow:

- Team collaboration
- Centralized permission management
- Repository ownership
- Access control

---

## Teams

Use teams to:

- Group users
- Assign repository permissions
- Manage access at scale

---

## Security Features

### Dependabot

- Dependency updates
- Security alerts

### Secret Scanning

Detects:

- API keys
- Tokens
- Credentials

### Code Scanning

Detects:

- Security vulnerabilities
- Code quality issues

---

## GitHub Actions

Automate:

- Testing
- Builds
- Deployments
- CI/CD workflows

Example workflow:

```yaml
name: CI

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4
```

---

## Useful Admin Tasks

- Manage collaborators
- Create teams
- Configure branch protection
- Review security alerts
- Configure Actions permissions
- Audit repository access