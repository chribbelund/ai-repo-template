---
applyTo: "**"
---
# Security Rules

- Never hardcode secrets, tokens, or credentials.
- Validate and sanitize external input.
- Use parameterized queries and safe serializers.
- Do not leak stack traces or sensitive internals to clients.
- Enforce authorization server-side even if UI hides actions.
- Prefer secure defaults for headers, cookies, CORS, and transport.
