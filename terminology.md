# Terminology

## Requirement

A requirement is a statement originating from a legal, regulatory, organizational, or policy source that specifies an expected obligation, condition, or constraint relevant to a system. In InspectR, requirements are the source from which compliance rules are derived.

## Compliance Engineering

Compliance Engineering is the systematic process of interpreting requirements, relating them to system designs or behaviors, and identifying evidence through which compliance-related properties can be assessed.

## Design-Time Compliance Assessment

Design-time compliance assessment is the evaluation of compliance-related properties of a system design before implementation or deployment. The assessment is based on available design evidence rather than runtime behavior.

## Policy-as-Code (PaC)

Policy-as-Code is the practice of representing policy conditions in a machine-readable and executable form so they can be automatically evaluated against structured input data.

## Rule

A rule is a formalized representation of a requirement that defines the conditions and controls to be evaluated. In InspectR, a rule operationalizes a selected requirement as machine-executable logic.

## Domain-Specific Rule Language (DSL)

A Domain-Specific Rule Language (DSL) is a specialized language designed to express compliance requirements, assessment conditions, and evidence constraints independently of a specific execution technology.

## Blueprint

A blueprint is a machine-readable representation of a planned AI or data pipeline containing components, connections, properties, and compliance-related declarations that can be assessed.

## Evidence

Evidence is the information used to support a compliance assessment. In InspectR, evidence consists of observed blueprint properties, derived facts, and their provenance.

## Fact

A fact is a typed evidence element extracted or derived from a blueprint and used during rule evaluation.

## Intermediate Representation (IR)

An Intermediate Representation (IR) is a normalized assessment-facing model that separates compliance assessment logic from blueprint-specific input formats.

## Compliance Inspection

Compliance inspection is the process of evaluating available evidence against formalized rules to determine whether selected compliance-related properties are represented in a system design.

## Inspection Engine

An inspection engine is a software component that evaluates compliance rules against structured evidence and produces assessment results.

## Open Policy Agent (OPA)

Open Policy Agent (OPA) is an open-source policy engine that evaluates policies against structured input data and returns decisions to the calling system.

## Rego

Rego is the declarative policy language used by Open Policy Agent to express and execute policy logic.

## Traceability

Traceability is the ability to link assessment findings to their originating requirements, rules, evidence, and supporting rationale.

## Result

A result is the output of a rule evaluation containing an assessment status together with supporting information such as evidence, rationale, and references.

## Assessment Status

An assessment status represents the outcome of rule evaluation:

- **PASS** – Required conditions are satisfied by the available evidence.
- **FAIL** – A required condition is violated.
- **UNKNOWN** – Available evidence is insufficient to determine the outcome.
- **HUMAN** – The assessment reaches a boundary requiring human judgment.
- **NOT_APPLICABLE** – The rule's applicability conditions are not met.
- **ERROR** – A technical failure prevents successful evaluation.

## InspectR

InspectR is the research artefact developed in this thesis. It is a design-time compliance inspection engine that evaluates AI and data-pipeline blueprints against formalized compliance rules using a Policy-as-Code approach.
