# Explainability Contract: APIDocMedic

## Decision

APIDocMedic decides whether recognizable web API routes exist without a visible OpenAPI or Swagger artifact. A match becomes a documentation-readiness finding backed by the observed route and documentation signals.

## Inputs

It uses readable source text to detect common Express- or FastAPI-style HTTP route patterns and checks the file list for openapi or swagger artifacts. The decision is deterministic and evidence-based.

## Limits

It does not prove that every endpoint is undocumented or that an existing API specification is complete. Dynamically generated routes and documentation hosted outside the repository may be missed.
