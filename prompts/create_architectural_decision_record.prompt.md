---
mode: 'agent'
description: Create an Architectural Decision Record (ADR) document for AI-optimized decision documentation.
tools: ['changes', 'codebase', 'editFiles', 'extensions', 'fetch', 'githubRepo', 'openSimpleBrowser', 'problems', 'runTasks', 'search', 'searchResults', 'terminalLastCommand', 'terminalSelection', 'testFailure', 'usages', 'vscodeAPI']
---
## Create Architectural Decision Record Prompt

Create an ADR document for `${input:DecisionTitle}` using structured formatting optimized for AI consumption and human readability.

**Inputs:**
- **Context**: `${input:Context}`
- **Decision**: `${input:Decision}`
- **Alternatives**: `${input:Alternatives}`
- **Stakeholders**: `${input:Stakeholders}`

**Requirements:**
- Use precise, unambiguous language
- Follow standardized ADR format with front matter
- Include both positive and negative consequences
- Document alternatives with rejection rationale
- Structure for machine parsing and human reference

The ADR must be saved in the `/docs/adr/` directory using the naming convention: `adr-NNNN-[title-slug].md`, where NNNN is the next sequential 4-digit number (e.g., `adr-0001-database-selection.md`).

**ADR Template:**

```md
---
title: "ADR-NNNN: [Decision Title]"
status: "Proposed"
date: "YYYY-MM-DD"
authors: "[Stakeholder Names/Roles]"
tags: ["architecture", "decision"]
supersedes: ""
superseded_by: ""
---

# ADR-NNNN: [Decision Title]

## Status
**Proposed** | Accepted | Rejected | Superseded | Deprecated

## Context
[Problem statement, technical constraints, business requirements, and environmental factors requiring this decision.]

## Decision
[Chosen solution with clear rationale for selection.]

## Consequences

### Positive
- [Beneficial outcomes and advantages]
- [Performance, maintainability, scalability improvements]
- [Alignment with architectural principles]

### Negative
- [Trade-offs, limitations, drawbacks]
- [Technical debt or complexity introduced]
- [Risks and future challenges]

## Alternatives Considered

### [Alternative 1 Name]
- **Description**: [Brief technical description]
- **Rejection Reason**: [Why this option was not selected]

### [Alternative 2 Name]
- **Description**: [Brief technical description]
- **Rejection Reason**: [Why this option was not selected]

## Implementation Notes
- [Key implementation considerations]
- [Migration or rollout strategy if applicable]
- [Monitoring and success criteria]

## References
- [Related ADRs]
- [External documentation]
- [Standards or frameworks referenced]
```

Generate the complete ADR document following this template with all sections populated based on the provided inputs.