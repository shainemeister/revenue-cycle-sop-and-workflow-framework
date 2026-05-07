# [Workflow Title]

**Version**: 1.0  
**Last Updated**: [Date]  
**Owner**: Shaine Meister  
**Status**: Draft / In Review / Active

> **Framework Alignment Check**  
> Before finalizing this workflow, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> This workflow is intended as the **simplified, visual quick-reference companion** to its parent SOP (see `modular-structure.md` – Recommended Design Patterns: SOP + Companion Workflow Pairing).

## Process Overview

Keep this to 2–4 sentences maximum. Focus on the end-to-end flow, its purpose, and key outcomes. Be concise.

## Visual Process Flow

Keep the diagram simple and focused on the main flow. Avoid unnecessary complexity or excessive branching unless essential for understanding.

```mermaid
flowchart TD
    A[Start] --> B[Step 1]
    B --> C{Decision?}
    C -->|Yes| D[Step 2]
    C -->|No| E[Step 3]
    D --> F[End]
    E --> F