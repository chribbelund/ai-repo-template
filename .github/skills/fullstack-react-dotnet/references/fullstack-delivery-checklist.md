# Fullstack Delivery Checklist

## Contract Alignment

- API request/response contract agreed and typed
- Error contract is consistent (validation, auth, conflict, not-found)
- Frontend mapping matches backend nullability/enums

## Security

- Auth token/session handling is consistent client/server
- Authorization enforced server-side
- Sensitive fields are never exposed to UI unless required

## Quality

- Backend tests cover business and endpoint behavior
- Frontend tests cover major interactions and failure states
- At least one critical end-to-end path validated manually or automated

## Operability

- Logs and traces can correlate a request through UI -> API
- New failure modes documented and observable
- Rollback or mitigation path exists for risky changes
