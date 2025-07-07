# Custom Chat Modes

This folder contains example custom chat modes for GitHub Copilot. For more information on how to use these, see the [GitHub Copilot custom chat modes](https://code.visualstudio.com/docs/copilot/chat/chat-modes#_custom-chat-modes).

## Available Chat Modes

| Name | File | Usage |
|------|------|-------|
| Azure Principal Architect | [azure-principal-architect.chatmode.md](azure-principal-architect.chatmode.md) | Provide expert Azure Principal Architect guidance using Azure Well-Architected Framework principles and Microsoft best practices. |
| Azure SaaS Architect | [azure-saas-architect.chatmode.md](azure-saas-architect.chatmode.md) | Provide expert Azure SaaS Architect guidance focusing on multitenant applications using Azure Well-Architected SaaS principles and Microsoft best practices. |
| Azure AVM Bicep mode | [azure-verified-modules-bicep.chatmode.md](azure-verified-modules-bicep.chatmode.md) | Create, update, or review Azure IaC in Bicep using Azure Verified Modules (AVM). |
| Azure AVM Terraform mode | [azure-verified-modules-terraform.chatmode.md](azure-verified-modules-terraform.chatmode.md) | Create, update, or review Azure IaC in Terraform using Azure Verified Modules (AVM). |
| Critical thinking | [critical-thinking.chatmode.md](critical-thinking.chatmode.md) | Challenge assumptions and encourage critical thinking to ensure the best possible solution and outcomes. |
| C#/.NET Janitor | [csharp-dotnet-janitor.chatmode.md](csharp-dotnet-janitor.chatmode.md) | Perform janitorial tasks on C#/.NET code including cleanup, modernization, and tech debt remediation. |
| Demonstrate Understanding | [demonstrate-understanding.chatmode.md](demonstrate-understanding.chatmode.md) | Validate user understanding of code, design patterns, and implementation details through guided questioning. |
| Expert .NET software engineer | [expert-dotnet-software-engineer.chatmode.md](expert-dotnet-software-engineer.chatmode.md) | Provide expert .NET software engineering guidance using modern software design patterns. |
| Expert React Frontend Engineer | [expert-react-frontend-engineer.chatmode.md](expert-react-frontend-engineer.chatmode.md) | Provide expert React frontend engineering guidance using modern TypeScript and design patterns. |
| Implementation Plan Generation Mode | [implementation-plan.chatmode.md](implementation-plan.chatmode.md) | Generate an implementation plan for new features or refactoring existing code. |
| Universal Janitor | [janitor.chatmode.md](janitor.chatmode.md) | Perform janitorial tasks on any codebase including cleanup, simplification, and tech debt remediation. |
| Mentor | [mentor.chatmode.md](mentor.chatmode.md) | Help mentor the engineer by providing guidance and support. |
| Principal software engineer | [principal-software-engineer.chatmode.md](principal-software-engineer.chatmode.md) | Provide principal-level software engineering guidance with focus on engineering excellence, technical leadership, and pragmatic implementation. |
| Semantic Kernel .NET | [semantic-kernel-dotnet.chatmode.md](semantic-kernel-dotnet.chatmode.md) | Create, update, refactor, explain or work with code using the .NET version of Semantic Kernel. |
| Semantic Kernel Python | [semantic-kernel-python.chatmode.md](semantic-kernel-python.chatmode.md) | Create, update, refactor, explain or work with code using the Python version of Semantic Kernel. |
| Idea Generator | [simple-app-idea-generator.chatmode.md](simple-app-idea-generator.chatmode.md) | Brainstorm and develop new application ideas through fun, interactive questioning until ready for specification creation. |
| Specification | [specification.chatmode.md](specification.chatmode.md) | Generate or update specification documents for new or existing functionality. |
| Technical Debt Remediation Plan | [tech-debt-remediation-plan.chatmode.md](tech-debt-remediation-plan.chatmode.md) | Generate technical debt remediation plans for code, tests, and documentation. |


## Usage

To use these chat modes:

1. Copy the desired `.chatmode.md` file to your VS Code user settings folder or workspace `.github/chatmodes` folder
1. Select the new chat mode through the chat interface in VS Code
