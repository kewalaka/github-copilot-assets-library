---
mode: 'agent'
description: Generate a comprehensive Architectural Decision Record (ADR) document that captures the context, decision, consequences, and alternatives for important technical decisions made during software development or system design.
tools: ['changes', 'codebase', 'editFiles', 'extensions', 'fetch', 'githubRepo', 'openSimpleBrowser', 'problems', 'runTasks', 'search', 'searchResults', 'terminalLastCommand', 'terminalSelection', 'testFailure', 'usages', 'vscodeAPI']
---
## Create Architectural Decision Record (ADR) Prompt

Your goal is to create a comprehensive Architectural Decision Record (ADR) document for `${input:DecisionTitle}`.

An ADR is a structured document that captures important technical decisions made during software development or system design. It serves as a permanent record of the reasoning behind decisions, helping teams understand the context and rationale for future reference and onboarding.

**Background Context**: `${input:Context}`
**Chosen Decision**: `${input:Decision}`
**Alternative Options**: `${input:Alternatives}`
**Key Stakeholders**: `${input:Stakeholders}`

**Best Practices for ADR Documentation:**
- Use clear, professional technical writing suitable for technical teams
- Follow established ADR templates and conventions
- Include both positive and negative consequences
- Provide sufficient context for future readers who weren't involved in the decision
- Document alternatives that were considered and why they were rejected
- Use consistent formatting and structure
- Ensure decisions are actionable and specific
- Make the document self-contained with no external dependencies for understanding

**ADR Quality Standards:**
- Follow industry-standard ADR format with proper sections
- Use precise, explicit, and unambiguous language
- Clearly distinguish between facts, assumptions, and opinions
- Include metadata (date, status, stakeholders) for tracking
- Provide rationale for the chosen solution
- Document trade-offs and implications honestly
- Structure content for easy parsing and future reference

**Task Execution Steps:**
1. Extract and validate the decision title and context information
2. Structure the background/context section with clear problem statement
3. Document the chosen decision with detailed rationale
4. Analyze and list consequences (both positive and negative)
5. Document alternatives that were considered and why they were rejected
6. Include proper metadata (date, status, stakeholders)
7. Format the document according to standard ADR conventions
8. Add related decisions or references if applicable

**Error Handling Guidelines:**
- If context is insufficient, provide template sections with placeholders for manual completion
- If decision details are vague, include general ADR structure with guidance for completion
- If alternatives are missing, suggest common alternatives based on the decision type
- Ensure the document is still useful even with minimal input

**Output Requirements:**
- Generate a Markdown document following standard ADR format
- Use proper heading hierarchy and structured sections
- Include professional formatting suitable for version control systems
- Ensure the document is ready for technical documentation systems
- Make it suitable for team collaboration and future reference

**ADR Template Structure:**
The output must follow this standardized format:

```markdown
# Architectural Decision Record: [Decision Title]

**Status:** [Proposed/Accepted/Rejected/Superseded/Deprecated]

**Date:** [Decision Date]

**Context:**
[Background information, problem statement, and situation requiring the decision. Include technical constraints, business requirements, and environmental factors.]

**Decision:**
[The chosen solution or approach with clear rationale for why this option was selected.]

**Consequences:**

*Positive:*
- [Beneficial outcomes and advantages of this decision]
- [Performance, maintainability, or scalability improvements]
- [Alignment with architectural principles or business goals]

*Negative:*
- [Drawbacks, limitations, or trade-offs]
- [Technical debt or complexity introduced]
- [Potential risks or future challenges]

**Alternatives Considered:**
- **[Alternative 1]**: [Brief description and reason for rejection]
- **[Alternative 2]**: [Brief description and reason for rejection]
- **[Alternative N]**: [Brief description and reason for rejection]

**Authors/Participants:** [Names or roles of people involved in the decision]

**Related Decisions:** [Links to related ADRs if applicable]
```

**Example Scenarios:**
This prompt is suitable for documenting decisions such as:
- Technology stack choices (React vs Vue.js, PostgreSQL vs MongoDB)
- Architectural patterns (microservices vs monolith, event-driven vs request-response)
- Infrastructure and deployment strategies
- Security and compliance approaches
- API design decisions
- Database schema design choices

**Automation Value:**
This prompt automates the creation of properly structured ADRs, ensuring consistency across team decision documentation and saving 30-60 minutes typically required for manual ADR creation. It promotes systematic thinking about alternatives and consequences while maintaining professional documentation standards.

Generate the ADR document now based on the provided inputs, following the template structure and quality standards outlined above.