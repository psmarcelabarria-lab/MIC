# MIC — Technical development roadmap / Hoja de ruta tecnológica

**Status:** Proposal; milestones are not completed deliverables.  
**Goal:** Build transparent educational tools and, separately, research-grade assessment infrastructure for the MIC.

## Phase A — Requirements and traceability
**Deliverables:** domain-to-requirement map, intended-user matrix, risk register, data-flow diagrams, public/protected material boundary.
**Acceptance evidence:** each feature linked to a stated use case, limitation and review owner.

## Phase B — Educational demonstrator (candidate open-source component)
**Deliverables:** accessible interactive reflection flow with synthetic cases; localization; plain-language explanations; automated tests.
**Acceptance evidence:** no clinical diagnosis or unsupported scoring; works without collecting personal data; tested keyboard navigation and mobile layout.
**Possible release:** UI shell, generic case engine, accessibility tests and documentation, subject to explicit licensing.

## Phase C — Research instrument infrastructure (not automatically open source)
**Deliverables:** versioned item bank stored privately; configurable response schemas; missing-data rules; reviewer workflow; audit trails; export formats.
**Acceptance evidence:** traceable version history, documented scoring assumptions, privacy and security review.
**Boundary:** protected MIC item content, scoring keys and participant data remain outside the public repository.

## Phase D — Evidence and evaluation
**Deliverables:** expert content-validity protocol, usability study, preregistration or protocol where appropriate, reliability and validity analyses matched to intended use.
**Acceptance evidence:** reproducible analysis plan, documented samples, limitations and transparent reporting.
**Important:** software tests are not psychometric validation.

## Phase E — Responsible release
**Deliverables:** explicit license for selected software, CONTRIBUTING update, security policy, changelog, version tags, tests and sample synthetic data.
**Acceptance evidence:** repository contains functional, tested, documented reusable code; licensing applies only to explicitly identified files.

## Potential use of Claude development resources
- Generate and refactor interface components and test suites, subject to human review.
- Review accessibility, localization, documentation and code quality.
- Assist with threat modeling and specification consistency.
- Support synthetic test fixtures and reproducible data-processing pipelines.
- Compare implementation against approved requirements.

**Not delegated to AI:** construct definition, expert judgments, informed consent, clinical safety decisions, statistical interpretation or validation claims.

## Success criteria
Success means a traceable and testable implementation, not a large number of commits. Milestones should be updated only when evidence exists. Public documentation should always distinguish planned, in progress and completed work.
