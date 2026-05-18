---
title: "Mermaid Visualization Standards"
short_title: "Mermaid Standards"
version: "1.1"
status: "Active"
owner: "Shaine Meister"
last_updated: "2026-05-17"
category: "Cross-Cutting"
matrix_position: "0.0"
related_sops: []
related_workflows: []
feedback_layer: "v1.0"
tags:
  - mermaid
  - visualization
  - standards
  - workflow
  - sop
  - feedback-loop
  - consistency
  - rcm
---

# Mermaid Visualization Standards

**Version**: 1.1  
**Last Updated**: 2026-05-17  
**Owner**: Shaine Meister  
**Status**: Active

> These standards follow the project’s principles of **Clarity & Consistency** and **Optimization Focus** (low mental friction). They are informed by the `mermaid-helper` skill’s type-aware recommendations for SOPs, Workflows, and Feedback Loop sections.

## Type-Specific Diagram Guidance & Examples

Different document types have different visual needs. The guidance below adapts shape selection, complexity, and focus accordingly.

### 1. SOPs (Lightweight & Supportive)

**When to use**: Inside SOP documents for exception handling, key decision points, or quick visual summaries. Keep diagrams minimal so they support (rather than replace) the procedural text.

**Recommended approach** (per `mermaid-helper`):
- Use simple classic or lightly enhanced shapes.
- Focus on 1–2 key decisions or exception paths.
- Prioritize human readability for training and daily execution.

**Example: Exception Handling Decision (for Registration SOP)**

```mermaid
%%{init: {
  "flowchart": {
    "htmlLabels": true,
    "nodeSpacing": 35,
    "rankSpacing": 50,
    "curve": "basis"
  }
}}%%
flowchart TD
    EligibilityIssue@{ shape: stadium, label: "Eligibility Issue Detected" }
    IssueType@{ shape: diamond, label: "Type of Issue?" }

    EligibilityIssue --> IssueType

    IssueType -->|Coverage Problem| ReverifyEligibility@{ shape: rect, label: "Re-verify Eligibility" }
    IssueType -->|Demographic Error| CorrectDemographics@{ shape: rect, label: "Correct Demographics" }
    IssueType -->|Newborn Grace| SendCourtesyLetter@{ shape: rect, label: "Send Courtesy Letter" }

    ReverifyEligibility --> DocumentChanges@{ shape: doc, label: "Document Changes & Rationale" }
    CorrectDemographics --> DocumentChanges
    SendCourtesyLetter --> DocumentChanges

    DocumentChanges --> ResumeProcessing@{ shape: stadium, label: "Resume Normal Processing" }

    %% Standardized RCM styling
    classDef startEnd fill:#d1fae5,stroke:#065f46,color:#064e3b
    classDef decision fill:#fef3c7,stroke:#b45309,color:#78350f
    classDef process fill:#dbeafe,stroke:#1e40af,color:#1e3a8a
    classDef document fill:#e0e7ff,stroke:#3730a3,color:#312e81

    class EligibilityIssue,ResumeProcessing startEnd
    class IssueType decision
    class ReverifyEligibility,CorrectDemographics,SendCourtesyLetter process
    class DocumentChanges document
```

**Why this style?** Lightweight, easy to embed, focuses only on the decision branches most relevant to SOP readers.

### 2. Workflows (Primary Visual Deliverable)

**When to use**: Dedicated workflow files. This is where rich semantic visualization shines.

**Recommended approach** (per `mermaid-helper` + project RCM standards):
- Use modern expanded shapes (`@{ shape: xxx }`) for semantic clarity.
- Apply the full RCM color palette and classes.
- Split complex flows into focused sections (Eligibility, COB, Authorization, etc.).
- Make closed-loop handoffs visually prominent.

**Example: Eligibility Issue Handling (Workflow style)**

```mermaid
%%{init: {
  "flowchart": {
    "htmlLabels": true,
    "nodeSpacing": 35,
    "rankSpacing": 50,
    "curve": "basis"
  }
}}%%
flowchart TD
    Start@{ shape: stadium, label: "Eligibility Issue Identified" }
    CheckType@{ shape: diamond, label: "Eligibility Type?" }

    Start --> CheckType

    CheckType -->|Active / Coverage| Reverify@{ shape: rect, label: "Re-verify Eligibility<br>Update Registration" }
    CheckType -->|Demographic Error| Correct@{ shape: rect, label: "Correct Demographics" }
    CheckType -->|Newborn Grace Period| Notify@{ shape: rect, label: "Send Notification Letter" }

    Reverify --> DocChanges@{ shape: doc, label: "Document Changes & Rationale" }
    Correct --> DocChanges
    Notify --> DocChanges

    DocChanges --> Resolve@{ shape: rect, label: "Resubmit Claim or Continue Follow-up" }
    Resolve --> End@{ shape: stadium, label: "Account Resolution" }

    %% Standardized RCM color classes
    classDef startEnd fill:#d1fae5,stroke:#065f46,color:#064e3b
    classDef decision fill:#fef3c7,stroke:#b45309,color:#78350f
    classDef process fill:#dbeafe,stroke:#1e40af,color:#1e3a8a
    classDef document fill:#e0e7ff,stroke:#3730a3,color:#312e81

    class Start,End startEnd
    class CheckType decision
    class Reverify,Correct,Resolve process
    class Notify,DocChanges document
```

**Why this style?** Rich semantics, clear visual hierarchy, and explicit start/end + document shapes — ideal as a day-to-day visual reference.

### 3. Feedback Loop Sections (Analytical / Data-Driven)

**When to use**: The standalone `## Feedback Loop & Data Collection Framework` section at the bottom of SOPs and Workflows. These diagrams should emphasize **data movement, capture points, triggers, and closed loops**.

**Recommended approach** (per `mermaid-helper`):
- More analytical focus.
- Highlight data capture, handoff triggers, destinations (e.g., Contract Intelligence, parent SOP).
- Use shapes that emphasize storage (`datastore`, `cyl`) and data movement.
- Show the closed-loop nature explicitly.

**Example: Closed-Loop Feedback & Handoff Flow**

```mermaid
%%{init: {
  "flowchart": {
    "htmlLabels": true,
    "nodeSpacing": 30,
    "rankSpacing": 45,
    "curve": "basis"
  }
}}%%
flowchart TD
    Exec@{ shape: stadium, label: "Workflow Execution<br>(Eligibility / Auth / COB)" }
    Capture@{ shape: rect, label: "Capture Structured Data" }

    Exec --> Capture

    Capture --> TriggerCondition@{ shape: diamond, label: "Trigger Condition?" }

    TriggerCondition -->|Repeated Issues| ContractInt@{ shape: rect, label: "Send to Contract Intelligence" }
    TriggerCondition -->|Normal Completion| Handoff@{ shape: rect, label: "Handoff to Parent SOP / Provider" }

    ContractInt --> Analysis@{ shape: rect, label: "Pattern Analysis &<br>Contract Mapping" }
    Handoff --> UpdateNote@{ shape: doc, label: "Update Account Note" }

    Analysis --> ClosedLoop@{ shape: stadium, label: "Closed Loop Back to Registration" }
    UpdateNote --> ClosedLoop

    %% Analytical / Data-focused + standardized styling
    classDef data fill:#f3e8ff,stroke:#6b21a8,color:#581c87
    classDef trigger fill:#fef3c7,stroke:#b45309,color:#78350f
    classDef handoff fill:#fce7f3,stroke:#9d174d,color:#831843
    classDef process fill:#dbeafe,stroke:#1e40af,color:#1e3a8a
    classDef startEnd fill:#d1fae5,stroke:#065f46,color:#064e3b

    class Capture,Analysis data
    class TriggerCondition trigger
    class ContractInt,Handoff handoff
    class Exec,UpdateNote,ClosedLoop process
```

**Why this style?** Emphasizes data capture → trigger → destination → closed loop. Uses `datastore`-style thinking and handoff coloring to make the analytical/feedback nature clear.

---

## Core Standards (Shapes, Colors, Configuration)

(Keep the existing strong sections on Recommended Node Shapes for RCM, Standardized Configuration & Styling, Best Practices, etc.)

## References

- `mermaid-helper` skill type-aware guidance (SOP / Workflow / Feedback Loop)
- Official Mermaid docs
- Project files: `core-principles.md`, `optimization-standards.md`, `workflow-template.md`

---

## Version History

| Version | Date       | Changes                                      | Author          |
|---------|------------|----------------------------------------------|-----------------|
| 1.0     | 2026-05-17 | Initial release with RCM-aligned shapes      | Shaine Meister  |
| **1.1** | 2026-05-17 | Added type-specific examples (SOP, Workflow, Feedback Loop) using `mermaid-helper` guidance | Shaine Meister  |
