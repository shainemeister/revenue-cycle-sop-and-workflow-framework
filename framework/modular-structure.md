# Modular Structure

**Version**: 1.0  
**Last Updated**: May 2026  
**Owner**: Shaine Meister

## Introduction

A key strength of this framework is its **modularity** — the ability to adapt, extend, or replace individual components without disrupting the overall system. This design enables the framework to remain relevant and useful across different organizations, systems, revenue cycle functions, and evolving operational needs.

Traditional SOP systems are often rigid and tightly coupled. When one part changes, the entire system becomes difficult to maintain. This framework takes the opposite approach: it is intentionally designed as a set of loosely coupled, composable components that can be mixed, matched, and adapted as needed.

This document explains the modular structure of the framework and provides guidance on how to maintain and leverage that modularity over time.

## Core Concepts of Modularity

### Separation of Concerns
Each major component of the framework has a clearly defined purpose and scope. Changes in one area should have minimal impact on other areas. This separation makes the system easier to understand, maintain, and evolve.

### Composability
Individual components (principles, templates, SOPs, and workflows) can be combined in different ways to meet specific needs. A new revenue cycle area can be added by creating new SOPs and workflows that follow existing templates, without requiring changes to the core principles or regulatory foundations.

### Abstraction Layers
The framework uses abstraction to hide unnecessary complexity. High-level principles and templates provide stable foundations, while specific SOPs and workflows can vary in detail and format as needed for different contexts.

### Portability
Because the framework is designed to be system- and organization-agnostic, its components can be carried from one environment to another. Modularity ensures that only the necessary pieces need to be adapted when moving between contexts.

## Modular Components

The framework is organized into four primary components, each with a distinct role:

| Component     | Primary Responsibility                          | Modularity Characteristics |
|---------------|-------------------------------------------------|----------------------------|
| **Framework** | Core principles, structure, regulatory foundations, and optimization standards | Provides stable, reusable foundations that rarely change |
| **Templates** | Standardized starting points for SOPs and workflows | Reusable patterns that enforce consistency while allowing customization |
| **SOPs**      | Detailed procedural documentation for specific areas | Can be added, removed, or modified independently |
| **Workflows** | Visual process flows and decision frameworks    | Can be developed at different levels of detail depending on need |

Because these components are loosely coupled, development or updates in one area do not require changes in the others.

## Adaptation Patterns

The modular design supports several common adaptation scenarios:

### Adapting to Different Organizations
When implementing this framework in a new organization, the core principles and templates remain largely unchanged. Only the specific SOPs and workflows need to be created or adjusted to reflect local processes, terminology, and requirements.

### Adapting to Different Revenue Cycle Areas
New functional areas (e.g., billing, denials, patient access) can be added by creating new folders and documents in the `sops/` and `workflows/` sections. These new components follow the existing templates and reference the core principles, ensuring consistency without requiring changes to the framework itself.

### Adapting Level of Detail
Some environments may require highly detailed SOPs, while others benefit from more concise, high-level guidance. The modular structure allows different levels of detail to coexist. Teams can choose the appropriate depth for their context while still operating within the same overall framework.

### Scaling or Simplifying
Organizations can start with a minimal implementation (core principles + a few key SOPs) and gradually expand. Conversely, a mature implementation can be streamlined by retiring or consolidating components that are no longer needed.

## Implementation Guidelines

To maintain the benefits of modularity:

- **Follow templates consistently** — New SOPs and workflows should start from the templates in the `templates/` folder. This ensures structural consistency even when content varies.
- **Limit scope of changes** — When updating a document, consider whether the change should be made in a specific SOP, in a template, or in the core framework. Changes that affect many documents should be made at the template or framework level.
- **Document dependencies clearly** — When one document references another, use clear links and explain the relationship. This prevents hidden coupling.
- **Version components independently** — Each SOP, workflow, and framework document can evolve on its own timeline. Use clear versioning and change logs to track evolution.
- **Evaluate against core principles** — Before adding or modifying any component, assess whether it aligns with the principles defined in `core-principles.md`.

> **Deeper guidance**: See `core-principles.md` (Principle 5 – Modularity & Adaptability) for the philosophical foundation that underpins these implementation guidelines.

## Relationship to Other Framework Documents

This document provides the **implementation mechanics** for modularity and adaptability.

- `core-principles.md` — Defines the philosophical foundation, particularly Principle 5 (Modularity & Adaptability). This document explains *how* that principle is put into practice through structure, components, and adaptation patterns.
- `regulatory-foundations.md` — Describes how regulatory and compliance requirements are integrated into the framework in a modular way, allowing compliance elements to be adapted without affecting other components.
- `optimization-standards.md` — Explains how continuous improvement, measurement, and efficiency practices can be applied modularly across different components and at different levels of the framework.

## Purpose of This Document

`modular-structure.md` serves as the practical guide for maintaining and leveraging the modular nature of this framework. It ensures that as the framework grows and evolves, it remains flexible, maintainable, and portable across different contexts.