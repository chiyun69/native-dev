# ✅ Code Review & QA

## Review Checklist

### Critical
- No sensitive data (API keys, secrets) committed.
- Proper use of secure storage and permissions.
- Error handling for exceptions and edge cases.
- Remove/minimize debug logs in production; never log sensitive info.
- No unresolved merge conflict markers.
- Dependencies are up to date and free of known vulnerabilities.

### High
- Code style compliance.
- Test coverage targets.
- Avoid blocking UI threads.
- Performance: avoid memory leaks, unnecessary allocations, and main thread work.

### Medium
- No hardcoded strings (all user-facing strings are externalized).
- Accessibility: content descriptions, touch targets, color contrast.
- Public functions/classes have KDoc comments.

