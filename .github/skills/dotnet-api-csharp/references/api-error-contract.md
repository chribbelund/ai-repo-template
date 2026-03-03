# API Error Contract (Recommended)

Use RFC 7807 `ProblemDetails` (or equivalent repo standard):

- `type`: stable URI for error class
- `title`: short human-readable summary
- `status`: HTTP status code
- `detail`: safe user-facing details
- `instance`: request path or trace reference

## Mapping Guidance

- Validation failure -> `400` or `422`
- Unauthorized -> `401`
- Forbidden -> `403`
- Not found -> `404`
- Conflict (duplicate/state) -> `409`
- Unhandled error -> `500` with sanitized detail
