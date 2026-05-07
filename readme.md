# Revenue Cycle SOP & Workflow Framework

**Status**: In Development  
**Last Updated**: May 2026  
**Owner**: Shaine Meister  
**Scope**: This framework focuses on revenue cycle management processes and is designed to be adaptable across different healthcare organizations and systems.

## Overview

This repository contains a **modular, platform-agnostic framework** for developing, organizing, and optimizing Standard Operating Procedures (SOPs) and workflows within revenue cycle management.

The goal is to create a reusable system of documentation and process design that can be adapted across different organizations, systems, and roles while maintaining strong alignment with industry standards and regulatory requirements.

## Purpose

The framework exists to:

- Provide a consistent, scalable method for building and maintaining revenue cycle SOPs and workflows.
- Serve as portable intellectual property that can be carried across different companies and platforms.
- Balance operational effectiveness with regulatory compliance and process optimization.
- Create clear separation between high-level strategy, reusable templates, and specific procedural documentation.

## Core Principles

This framework is built on the following foundational ideas:

- **Modularity** — Components can be adapted, extended, or replaced without disrupting the overall system.
- **Clarity & Consistency** — Documentation follows standardized formats to improve readability and maintainability.
- **Regulatory Alignment** — All processes respect industry regulations and compliance requirements.
- **Optimization Focus** — Every SOP and workflow is designed with efficiency, accuracy, and continuous improvement in mind, with emphasis on reducing mental friction and enabling intuitive flow.
- **Portability** — The framework is intentionally designed to be system- and organization-agnostic.

## Framework Components

This project is organized into four main areas:

| Component     | Purpose                                                                 | Location          |
|---------------|-------------------------------------------------------------------------|-------------------|
| **Framework** | Core principles, modular design, regulatory foundations, and optimization standards | `framework/`      |
| **Templates** | Reusable templates for creating consistent SOPs and workflows           | `templates/`      |
| **SOPs**      | Detailed Standard Operating Procedures for specific revenue cycle areas | `sops/`           |
| **Workflows** | Process flows, decision trees, and visual process documentation         | `workflows/`      |

## Current Focus Areas

Initial development of this framework is centered on establishing a strong foundational structure. The four primary components are being developed in parallel:

- **Framework** — Defining the guiding principles, modular design approach, regulatory foundations, and optimization standards.
- **Templates** — Creating standardized templates to ensure consistency when building new SOPs and workflows.
- **SOPs** — Developing clear, well-structured operating procedures for key revenue cycle functions.
- **Workflows** — Designing visual process flows and decision frameworks that support the SOPs.

Specific SOPs and workflows under active development, along with their current status, are tracked in the `plan.md` file. This separation keeps the high-level structure clear while allowing detailed progress tracking in one central location.

## How to Use This Framework

1. Review the documents in the `framework/` folder to understand the guiding principles and structure.
2. Use the templates in the `templates/` folder when creating new SOPs or workflows.
3. Follow the established format and structure when developing content in the `sops/` and `workflows/` folders.
4. Maintain version history and clear documentation so processes remain understandable and maintainable over time.

## How to Create a New SOP or Workflow (Step-by-Step Process)

This section provides a clear, repeatable process for creating new content while maintaining full continuity with the framework. Follow these steps in order.

### Step 1: Review the Framework Documents
Before creating any new content, review the relevant sections of the framework to ensure alignment:

- Read `core-principles.md` (especially Principles 1–4 and 7) to internalize the philosophy of simplicity, intuitive flow, usability over exhaustiveness, and continuous improvement.
- Review `modular-structure.md` (especially the “Recommended Design Patterns” section) to understand the **SOP + Companion Workflow** pairing approach.
- Check `regulatory-foundations.md` for how to integrate compliance considerations lightly and appropriately.
- Review `optimization-standards.md` to understand how to design for predictable navigation with minimal mental friction and reduced text volume.

### Step 2: Decide on the Deliverable(s)
- Determine whether you need an **SOP**, a **Workflow**, or **both** (recommended pairing).
  - Create an **SOP** when the process requires documented context, roles, regulatory notes, quality checks, or training value.
  - Create a **Workflow** when the process benefits from a simplified, visual quick-reference for day-to-day use.
  - For most processes, create **both** as companion documents (see `modular-structure.md` – Recommended Design Patterns).

### Step 3: Copy the Appropriate Template
- Go to the `templates/` folder.
- Copy `sop-template.md` if creating an SOP.
- Copy `workflow-template.md` if creating a Workflow.
- Paste the copy into the target location (`sops/` or `workflows/`) and rename it appropriately (e.g., `registration.md` or `registration-workflow.md`).

### Step 4: Fill in the Content
- Complete each section of the template.
- Keep language concise and focused on essential actions (optimize for predictable navigation with minimal mental friction).
- Include decision points where relevant.
- Add brief regulatory context in the designated section (do not reproduce full regulatory text).
- For Workflows: Keep the Mermaid diagram simple and focused on the main flow.

### Step 5: Add Cross-References
- In the SOP’s “Companion Workflow” section, link to the corresponding Workflow (if one exists).
- In the Workflow’s “Parent SOP” section, link to the corresponding SOP.
- Ensure both documents reference the relevant framework files where appropriate (the templates already include guidance for this).

### Step 6: Update Supporting Files
- Add the new SOP/Workflow to the `plan.md` file with its current status and priority.
- If this is a significant addition, consider updating the “Current Focus Areas” or “Status & Roadmap” sections in this `readme.md`.

### Step 7: Review for Framework Alignment
Before finalizing, perform a quick self-check:
- Does this document align with the Core Principles (especially Simplicity First, Intuitive Flow, and Usability Over Exhaustiveness)?
- Is the text volume minimized while preserving necessary regulatory and procedural integrity?
- Does the document follow the modular structure and template standards?
- If a companion document exists, do the two files clearly reference each other?

### Step 8: Commit and Version
- Commit the new file(s) with a clear message describing what was created.
- Update the Version History table inside the document.
- Update `plan.md` to reflect the new status.

## Collaboration & Maintenance

This framework is being developed collaboratively. High-level direction, feedback, and new content requests are managed through direct communication and issues. All documentation follows the standards defined in this repository to ensure consistency and long-term usability.

Version history is maintained through Git. When updating existing documents, changes should be clearly described and dated.

## Status & Roadmap

This framework is currently in the foundational development phase. The initial focus is on building out the core framework principles, establishing reusable templates, and developing initial SOPs and workflows for key revenue cycle functions.

Future phases may include:
- Expansion into additional revenue cycle areas
- Refinement of optimization and measurement standards
- Development of supporting tools and examples

Progress on individual SOPs and workflows is tracked in the `plan.md` file.