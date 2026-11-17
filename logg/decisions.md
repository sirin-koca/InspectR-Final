# Decisions Log (ADR)

This document records significant technical, architectural, and research decisions made during the development of InspectR. The purpose is to provide traceability, rationale, and justification for design choices throughout the MSc project.

---

## ADR-001: InspectR as a Design-Time Compliance Assessment Tool

**Date:** YYYY-MM-DD

### Decision
InspectR will focus on design-time compliance assessment rather than run-time monitoring.

### Rationale
The research objective is to determine whether compliance requirements can be assessed from structured AI-system and data-pipeline blueprints before implementation and deployment.

### Consequences
- Requires machine-readable architectural models.
- Focuses on inspectable properties rather than operational behavior.
- Reduces dependency on deployed systems and execution logs.

---

## ADR-002: Policy-as-Code as Representation of Compliance Requirements

**Date:** YYYY-MM-DD

### Decision
Compliance requirements are represented as Policy-as-Code rules.

### Rationale
Policy-as-Code enables automated evaluation, repeatability, transparency, and traceability of compliance checks.

### Alternatives Considered
- Natural-language requirements
- Manual expert assessment
- Custom rule implementations

### Consequences
- Rules are machine-readable and executable.
- Regulatory requirements must be translated into formal representations.

---

## ADR-003: Separation of Research Documentation and Source Code

**Date:** YYYY-MM-DD

### Decision
Documentation is stored within the repository under `/docs`.

### Rationale
Documentation evolves alongside implementation and benefits from version control.

### Consequences
- Single source of truth.
- Full traceability between design decisions and implementation.

---

## ADR-004: Public Repository

**Date:** YYYY-MM-DD

### Decision
InspectR-Final remains publicly accessible on GitHub.

### Rationale
The repository contains only professional research artifacts, source code, documentation, and supporting materials. No confidential or personal information is included.

### Consequences
- Supports transparency and reproducibility.
- Facilitates supervisor and collaborator access.
- Requires continued attention to repository hygiene.

---

## ADR-005: Migration from InspectR-PoC to InspectR-Final

**Date:** YYYY-MM-DD

### Decision
InspectR-Final supersedes the earlier InspectR-PoC repository.

### Rationale
The PoC served as an exploratory prototype. InspectR-Final represents the research artifact used for the MSc thesis.

### Consequences
- Research history remains documented.
- Development efforts are consolidated in a single repository.

---

## ADR-006: Test-Driven Validation

**Date:** YYYY-MM-DD

### Decision
Automated tests are maintained under `/tests`.

### Rationale
Validation improves confidence in the correctness and stability of the prototype.

### Consequences
- Changes can be verified systematically.
- Supports reproducibility of research results.

---

## Template

## ADR-XXX: Title

**Date:** YYYY-MM-DD

### Decision

### Rationale

### Alternatives Considered

### Consequences