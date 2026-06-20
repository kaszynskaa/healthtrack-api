## Summary
<!-- What does this PR do and why? One or two sentences. -->

## Changes Made
<!-- List the files changed and the reason for each change. -->
- 
- 

## Type of Change
<!-- Check all that apply. -->
- [ ] Bug fix
- [ ] New feature
- [ ] Refactor (no behaviour change)
- [ ] CI/infrastructure change
- [ ] Documentation update

## Breaking Changes
<!-- Does anything break for existing callers? API contract, env vars, DB schema? -->
- [ ] No breaking changes
- [ ] Breaking change — describe below and update CLAUDE.md:

## Database Migrations
<!-- Any schema changes? New tables, columns, indexes, or data backfills? -->
- [ ] No database changes
- [ ] Migration required — file: `migrations/`
- [ ] Data backfill required — estimated rows affected:

## Performance Impact
<!-- Will this change affect response times, query counts, or memory usage? -->
- [ ] No performance impact
- [ ] Potential impact — describe below:

## Feature Flags
<!-- Is this change gated behind a flag? Can it be rolled back without a deploy? -->
- [ ] No feature flag needed
- [ ] Feature flag: `FLAG_NAME=` — default off, enable via env var

## Security
<!-- Has this been reviewed for OWASP Top 10 issues? -->
- [ ] No secrets added to source code
- [ ] No hardcoded credentials or API keys
- [ ] All SQL queries use parameterised statements (no f-string queries)
- [ ] No PII logged or exposed in API responses
- [ ] `bandit` scan reviewed (CI Security job summary)

## Testing
<!-- How was this tested? The CI pipeline runs automatically — note anything tested manually. -->
- [ ] `pytest tests/` passes locally
- [ ] New tests added for changed behaviour
- [ ] `docker compose up` works and `GET /health` returns 200
- [ ] Manual testing:

## CI Pipeline
<!-- These run automatically on every PR — confirm you have reviewed the results. -->
- [ ] Lint (flake8 + black) — passing
- [ ] Test — passing, coverage above threshold
- [ ] Security (bandit + safety) — reviewed findings in job summary
- [ ] AI Skills (security-audit) — no CRITICAL findings, or CRITICAL findings are acknowledged below:

## Deployment Notes
<!-- Anything the person deploying needs to do after merge? -->
- New env vars to add to `.env` / GitHub Secrets:
- Services to restart:
- Cache to flush:

## Checklist
- [ ] PR title follows `type(scope): description` format
- [ ] Code reviewed by at least one team member
- [ ] CLAUDE.md updated if project context or scope changed
- [ ] `.env.example` updated if new env vars were added
- [ ] No debug `print()` or `logger.debug()` left in code
