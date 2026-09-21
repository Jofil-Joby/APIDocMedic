# APIDocMedic

> Portable agent for detecting recognizable API routes that lack OpenAPI or Swagger documentation.

## What it does

APIDocMedic scans source files for common Express-style HTTP route definitions and checks whether recognizable OpenAPI or Swagger documentation is present.

### Diagnostic fingerprint

**Route discovery → documentation gap → evidence → API documentation plan**

## Why this agent is distinct

APIDocMedic connects implementation evidence to developer-facing API documentation. It is not an API correctness checker and does not claim that undocumented routes are broken. Its job is to surface a documentation gap that can be acted on.

## Workflow

```text
API source
   ↓
Route detector
   ↓
OpenAPI / Swagger presence check
   ↓
Evidence-backed finding
   ↓
Documentation recommendation
```

## Verification

Includes:
- OpenGAP-compatible passport metadata
- API-documentation fixture
- behavior and explainability contracts
- OpenAI / CrewAI / Claude Code / Lyzr adapters
- automated adapter verification

OpenGAP validation passed and all four generated framework exports have been exercised successfully.

## Design principle

**Implementation and documentation should agree.** APIDocMedic looks for evidence that the API surface has a corresponding documentation surface.

## Medic family

APIDocMedic is the API-documentation specialist in the larger portable Medic family.