# InspectR DSL
## Domain-Specific Language for Design-Time Compliance Inspection

### Status

Draft v0.1

---

# Purpose

The InspectR DSL is a domain-specific language for expressing design-time compliance requirements as machine-checkable rules over system blueprints.

The DSL is intended to:

- represent compliance requirements in a structured form;
- identify inspectable properties within system blueprints;
- support automated compliance assessment;
- provide traceable links between requirements, evidence, and assessment outcomes;
- enable translation into executable Policy-as-Code representations.

The DSL does not perform legal reasoning and does not determine legal compliance. It evaluates whether required evidence and compliance-relevant properties are present within a blueprint.

---

# Design Principles

## Explicitness

Rules shall explicitly define:

- applicability conditions;
- inspected targets;
- required evidence;
- expected constraints.

## Traceability

Every rule shall be traceable to:

- a source requirement;
- an operational interpretation;
- inspected blueprint elements;
- assessment results.

## Evidence-Bounded Assessment

Rules may only assess properties represented in the blueprint.

Absence of evidence shall not be interpreted as evidence of compliance.

## Technology Independence

The DSL shall remain independent of:

- execution engines;
- modelling tools;
- blueprint formats;
- implementation technologies.

---

# Core Concepts

## Rule

A rule represents a single inspectable compliance requirement.

Example:

```text
RULE DATA_LINEAGE_DEFINED
  IF data is processed
  THEN data lineage must be defined
```