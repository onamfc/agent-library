# Infrastructure Agent

A Senior Software Infrastructure Engineer (DevOps) persona focused on CI/CD, deployment pipelines, and infrastructure automation.

## When to Use

- Setting up CI/CD for a new project
- Optimizing slow or flaky builds
- Configuring deployment pipelines with GitHub Actions
- Establishing branch protection and release strategies
- Debugging failed workflows
- Auditing infrastructure for security and reliability gaps

## When NOT to Use

- Writing application business logic
- Frontend/backend feature development
- Database schema design (use a database-focused agent)
- General code review (use a code review agent)

## Model Recommendations

| Model | Suitability | Notes |
|-------|-------------|-------|
| Claude Code | Excellent | Can read repo, propose and apply changes directly |
| Cursor | Excellent | Good for inline workflow editing |
| Claude API | Good | Works well for analysis and recommendations |
| GPT-4 | Good | Solid alternative for workflow generation |

## Context Requirements

This agent works best with:

- Access to `.github/workflows/` directory
- `package.json`, `Cargo.toml`, or equivalent dependency files
- Understanding of the deployment target (Railway, Vercel, AWS, etc.)

## Limitations

- Assumes GitHub Actions as the CI platform
- Does not handle secrets management beyond GitHub Secrets references
- No direct infrastructure provisioning (Terraform, Pulumi, etc.)

## Customization

Fork and modify for:

- Different CI platforms (GitLab CI, CircleCI, Jenkins)
- Different deployment targets (Vercel, Fly.io, AWS)
- Organization-specific compliance requirements
- Additional quality gates (security scanning, license checks)
