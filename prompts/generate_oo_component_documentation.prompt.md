---
mode: 'chat'
description: 'Generate comprehensive, standardized documentation for object-oriented components following industry best practices and architectural documentation standards.'
tools: ['changes', 'codebase', 'editFiles', 'extensions', 'fetch', 'githubRepo', 'openSimpleBrowser', 'problems', 'runTasks', 'search', 'searchResults', 'terminalLastCommand', 'terminalSelection', 'testFailure', 'usages', 'vscodeAPI']
---

## Generate Standard OO Component Documentation

Your goal is to create comprehensive documentation for the object-oriented component `${input:ComponentName}` using the provided source code files and context.

Analyze the component files: `${input:ComponentFiles}` within the system context: `${input:SystemContext}` and generate documentation targeted for: `${input:TargetAudience}`.

Consider any existing diagrams: `${input:ExistingDiagrams}` and special requirements: `${input:SpecialRequirements}` when creating the documentation.

**Documentation Standards:**
- Follow C4 Model documentation levels (Context, Containers, Components, Code)
- Align with Arc42 software architecture documentation template
- Comply with IEEE 1016 Software Design Description standard
- Use Agile Documentation principles (just enough documentation that adds value)
- Ensure audience-focused writing for developers and maintainers

**Required Documentation Structure:**

## 1. Component Overview

### Purpose/Responsibility
[Clearly state what this component does and its primary responsibility in the system]

### Scope
**Included:** [What functionality is included in this component]
**Excluded:** [What functionality is explicitly not handled by this component]

### Context
[Describe how this component fits within the larger system architecture and its relationships with other components]

## 2. Architecture Section

### Design Patterns
[Identify and document the design patterns used (Repository, Factory, Observer, etc.)]

### Dependencies
[List all internal and external dependencies with their purposes]

### Relationships
[Document how this component interacts with other system components]

### Visual Diagrams
[Suggest appropriate diagrams: UML class diagrams, sequence diagrams, component diagrams]
```mermaid
// Suggested diagram placeholder - replace with actual Mermaid syntax
classDiagram
    class ComponentName {
        // Add class structure
    }
```

## 3. Interface Documentation

### Public Interfaces
[Document all public interfaces, their purposes, and usage patterns]

### Methods/Properties
| Method/Property | Purpose | Parameters | Return Type | Usage Notes |
|-----------------|---------|------------|-------------|-------------|
| [Name] | [Purpose] | [Parameters] | [Type] | [Notes] |

### Events/Callbacks
[Document any events, callbacks, or notification mechanisms]

## 4. Implementation Details

### Concrete Classes
[Document the main implementation classes and their responsibilities]

### Configuration
[Describe any configuration requirements, settings, or initialization parameters]

### Algorithms
[Document key algorithms, business logic, or complex processing]

### Performance Characteristics
[Document performance considerations, bottlenecks, and optimization approaches]

## 5. Usage Examples

### Basic Usage
```csharp
// Basic usage example
var component = new ComponentName();
component.DoSomething();
```

### Advanced Usage
```csharp
// Advanced configuration and usage patterns
var options = new ComponentOptions
{
    // Configuration settings
};
var component = ComponentFactory.Create(options);
await component.ProcessAsync(data);
```

### Configuration Examples
[Provide examples of different configuration scenarios]

### Best Practices
[Document recommended usage patterns and best practices]

## 6. Quality Attributes

### Security
[Document security considerations, authentication, authorization, data protection]

### Performance
[Document performance characteristics, scalability limits, resource usage]

### Reliability
[Document error handling, fault tolerance, recovery mechanisms]

### Maintainability
[Document coding standards, testing approaches, documentation maintenance]

### Extensibility
[Document extension points, plugin architecture, customization options]

## 7. Reference Information

### Dependencies
[List all dependencies with versions and purposes]

### Configuration Reference
[Complete configuration options and their effects]

### Testing Guidelines
[Document how to test this component, mock dependencies, test data setup]

### Troubleshooting
[Common issues, error messages, diagnostic approaches]

### Related Documentation
[Links to related specifications, API documentation, external resources]

### Change History
[Document major changes, version history, migration notes]

**Analysis Instructions:**

1. **Code Analysis**: Examine the provided source code files to identify:
   - Class structures and inheritance hierarchies
   - Design patterns and architectural decisions
   - Public APIs and interfaces
   - Dependencies and external integrations
   - Configuration mechanisms
   - Error handling approaches

2. **Design Pattern Recognition**: Identify and document patterns such as:
   - Creational patterns (Factory, Builder, Singleton)
   - Structural patterns (Adapter, Decorator, Facade)
   - Behavioral patterns (Observer, Strategy, Command)

3. **Interface Documentation**: For each public method/property, document:
   - Purpose and responsibility
   - Input parameters with types and constraints
   - Return values and their meanings
   - Possible exceptions and error conditions
   - Usage examples and best practices

4. **Quality Assessment**: Evaluate and document:
   - Performance implications and bottlenecks
   - Security considerations and vulnerabilities
   - Reliability and error handling robustness
   - Maintainability and code organization
   - Testing coverage and strategies

5. **Context Integration**: Consider the system context to document:
   - How the component integrates with other system parts
   - Data flow and communication patterns
   - Deployment and configuration requirements
   - Monitoring and operational considerations

**Language-Specific Optimizations:**

- **C#/.NET**: Include async/await patterns, dependency injection, configuration patterns, resource disposal
- **Java**: Include Spring framework patterns, annotations, exception handling, packaging
- **TypeScript/JavaScript**: Include module patterns, async patterns, type definitions, npm considerations
- **Python**: Include package structure, virtual environments, type hints, testing frameworks

**Error Handling:**

- If source code is incomplete, request specific missing information
- If component context is unclear, ask clarifying questions about system architecture
- If design patterns are non-standard, document the custom approaches used
- If documentation requirements are unclear, suggest alternative documentation formats

**Output Format:**
Generate a well-structured Markdown document with:
- Clear heading hierarchy
- Code blocks for examples and interfaces
- Tables for method/property documentation
- Bullet points for feature lists
- Mermaid diagram suggestions with appropriate syntax
- Proper markdown formatting for readability and maintainability

Focus on creating living documentation that serves as both reference material and onboarding guide for developers working with this component.