# MIC — Proposed software architecture / Arquitectura propuesta

**This document describes a future architecture, not an implemented system.**

## Conceptual separation
```text
Public documentation (GitHub)
       |
       +-- Educational interface (synthetic cases; optional future OSS)
       |       +-- Case content with explicit reuse rights
       |       +-- Generic interaction engine
       |       +-- Accessibility/localization tests
       |
       +-- Technical specifications and issue tracker

Protected research environment (separate access controls)
       +-- Versioned instrument item bank
       +-- Research consent and participant management
       +-- Restricted scoring / interpretation specifications
       +-- Research datasets and analysis pipeline
```

## Data protection by design
- Prefer zero data collection for public educational demonstrations.
- Use synthetic cases only in the public codebase.
- Never embed patient information, tokens or restricted assessment content in client-side code.
- For future human-participant research, define legal basis, consent, retention, access controls, deletion, encryption, incident response and research governance before collecting data.
- Treat self-reported platform responses as claims requiring independent verification where appropriate.

## Proposed module contracts
**Case engine:** receives a versioned synthetic scenario and permitted response options; returns explanatory educational feedback, not a diagnosis.

**Questionnaire engine:** receives a versioned schema; validates answer completeness and missing-data semantics; never silently converts unknown answers into zeros.

**Reporting layer:** displays provenance, version, limitations and uncertainty; labels exploratory outputs as exploratory.

**Research pipeline:** separate, access-controlled environment with data minimization, de-identification and documented analysis plans.

## Quality and safety gates
- Unit tests for routing, missing data and report generation.
- Accessibility testing and human usability review.
- Threat modeling for sensitive-data entry, prompt injection and misleading output.
- Clinical and ethical expert review before claims of assessment use.
- Explicit release checklist for any open-source module.

## License boundary
The repository is currently public but unlicensed. Any future software license must specify exactly what is released; it does not automatically extend to MIC theory, instrument items, trademarks, research data or protected scoring methods.
