# Copilot Instructions

<!-- This file tells GitHub Copilot how to behave in this project.
     Uncomment and fill in any section to add more specific guidance. -->

## General Principles

- **Show, don't tell.** Use code examples to illustrate suggestions — don't just describe what to do.
- **Plain language.** Write comments, docs, and feedback in clear, simple English.

## Project Context

- **Name**: <!-- e.g. "Acme Admin Portal" -->
- **Stack**: <!-- e.g. "Next.js 14, TypeScript, Postgres" -->
- **Audience**: <!-- e.g. "Internal staff" or "Public-facing customers" -->

---

## Code Style & Quality

- Match the conventions already in this codebase.
- Keep functions short and focused — one job per function.
- Use clear, descriptive names.
- No hardcoded values — use named constants or config.
- Remove unused code and imports.

<!--
More specific guidance to consider adding:
- Avoid abbreviations unless standard in this stack (e.g. `req`, `res`)
- Clever is not a compliment — write for humans first
- Reference your linter or style guide, e.g. "See `.eslintrc` for rules"
-->

---

## Standards & Best Practices

- Apply language and framework best practices by default.
- Prefer the simplest solution that works.
- Use standard library or built-ins over third-party dependencies where possible.
- Reference official docs as the source of truth (MDN, language specs, framework docs)

<!--
More specific guidance to consider adding:
- List any specs or standards this project follows, e.g. "REST API follows JSON:API spec"
-->

---

## Security

- Never hardcode secrets or credentials — use environment variables.
- Validate and sanitize all user input.
- Never log sensitive data (passwords, tokens, PII).
- Apply least privilege — request only the permissions actually needed
- Flag auth, payment, or PII code with a `# security-sensitive` comment

<!--
More specific guidance to consider adding:
- Note any project-specific requirements, e.g. "Auth is handled by Auth0 — do not roll custom auth"
-->

---

## Accessibility

- Follow WCAG 2.1 AA as a baseline for all UI code.
- Use semantic HTML over generic `<div>` where possible.
- Every image needs a meaningful `alt` attribute, or `alt=""` if decorative.
- All interactive elements must be keyboard accessible
- Don't rely on color alone to convey meaning — pair it with text or an icon

<!--
More specific guidance to consider adding:
- Note any accessibility tooling in use, e.g. "Run `axe` in CI"
-->

---

## Testing

- Test the happy path, edge cases, and error conditions.
- Test behavior and outcomes — not implementation details.
- Test names should describe expected behavior, e.g. `returns 404 when user not found`

<!--
More specific guidance to consider adding:
- Specify your test framework and coverage threshold, e.g. "Jest, 80% coverage required"
-->

---

## Agent & Tool Use

- Suggest changes — do not apply edits directly to files.
- Check if a file or function already exists before creating a new one.
- Only change files within the current task's scope.
- Check the standard library before adding a new dependency
- List available tools or MCP servers, e.g. "Use the `github` MCP for PR and issue lookups"

<!--
More specific guidance to consider adding:
- Prefer editing existing files over creating new ones for small changes
-->

---

## Plain Language

- Comments explain _why_, not _what_.
- Keep inline comments short and specific.
- Write comments in plain English — avoid filler like "this function handles..."

<!--
More specific guidance to consider adding:
- If a comment needs more than two lines, consider restructuring the code instead
-->

---

## Project-Specific Notes

<!--
Add anything unique to this project that Copilot should always know, for example:
- "This is a monorepo — shared utilities live in `/packages/shared`"
- "API routes follow the pattern `/api/v1/[resource]`"
- "We use feature flags via LaunchDarkly before shipping new UI"
-->
