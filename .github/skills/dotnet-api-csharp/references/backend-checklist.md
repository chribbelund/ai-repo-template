# Backend Delivery Checklist

## Design

- Endpoint contract is explicit and documented by type
- Request/response DTOs are separated from domain models
- Authorization requirements are defined per endpoint

## Implementation

- Cancellation token is threaded through async calls
- Logging includes operation context and identifiers
- Persistence uses scoped DbContext and proper transaction boundaries

## Validation and Errors

- Model validation is enforced consistently
- Domain/infra exceptions are translated to API-safe responses
- No stack traces or internal implementation details in client responses

## Tests

- Unit tests cover happy path + edge cases
- Integration tests verify status codes and payload contracts
- Regression tests added for fixed bugs

## Performance

- Read paths avoid unnecessary tracking/projection bloat
- Pagination and limits are applied to list endpoints
- Query shape reviewed for N+1 and large includes
