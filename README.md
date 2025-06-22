
# Github Copilot Assets Library

There are many ways GitHub Copilot can be used to help you with not just your coding tasks, but also with ideation, problem solving, understanding, planning, research and so much more.

The biggest challenge is either creating or finding the right prompts and tools to get the most out of GitHub Copilot - and when to use them.

I've spend many hours building own tools and prompts and chat modes to help me with my work, and I want to share them with you.

This repository provides the following types of assets:

1. **Copilot Instructions**: These are custom instructions that you can add to your GitHub repository to enhance the way GitHub Copilot interacts with your code. They can be used to set the tone, style, and context of the responses you receive from Copilot. See the [Custom Instructions](https://code.visualstudio.com/docs/copilot/copilot-customization#_custom-instructions) for more information. This is available in both Visual Studio Code and Visual Studio. These can be configured at the user and workspace level.
1. **Custom Code Generation Instructions (experimental)**: These are similar to Copilot Instructions, but specifically designed for code generation tasks. They provide additional context and guidelines for generating code snippets. See the [Code Generation Instructions Examples](https://code.visualstudio.com/docs/copilot/copilot-customization#_custom-instructions-examples) for more information. This is only available in Visual Studio Code. These can be configured at the user and workspace level.
1. **Prompt Files (experiemental)**: Prompt files are reusable prompts for common tasks like generating code or performing a code review. You define the prompt content in a Markdown file. A prompt file is a standalone prompt that you can run directly in chat. Optionally, you can also include guidelines about how the task should be performed. See the [Prompt Files](https://code.visualstudio.com/docs/copilot/copilot-customization#_prompt-files-experimental) for more information. This is only available in Visual Studio Code. These can be configured at the user and workspace level.
1. **Custom Chat Modes**: Aside from the core chat modes of Ask, Edit and Agnet, _custom chat modes_ consist of a set of instructions and tools that are applied when you switch to that mode. For example, a "Plan" chat mode could include instructions for generating an implementation plan and only use read-only tools. By creating a custom chat mode, you can quickly switch to that specific configuration without having to manually select relevant tools and instructions each time. For more information, see the [Custom Chat Modes](https://code.visualstudio.com/docs/copilot/chat/chat-modes#_custom-chat-modes) documentation. This is only available in Visual Studio Code. These can be configured at the user and workspace level.
1. **Tool Sets**: Tool sets are collections of tools that you can use in your chats. They allow you to group related tools together and switch between different sets of tools easily. These aren't fully docmented yet, but are included for completeness. Tool sets are only available in Visual Studio Code. These can only be configured at the user level.
1. **MCP Servers**: MCP servers are a way to provide additional functionality to GitHub Copilot by allowing it to call out to external services using Model Context Protocol. See the [MCP Servers](https://code.visualstudio.com/docs/copilot/chat/mcp-servers) documentation for more information. This is only available in both Visual Studio Code and Visual Studio. These can be configured at the user and workspace level.

## Copilot Features Comparison Table

| Feature Name | Description | VS Code/VS Support | Configure at Workspace or Config Level |
|--------------|-------------|--------------------|----------------------------------------|
| Copilot Instructions | [Custom instructions](https://code.visualstudio.com/docs/copilot/copilot-customization#_custom-instructions) to set tone, style, and context for Copilot responses. | VS Code & VS | User & Workspace |
| Custom Code Generation Instructions | [Code generation instructions](https://code.visualstudio.com/docs/copilot/copilot-customization#_custom-instructions-examples) for code generation tasks. | VS Code only | User & Workspace |
| Prompt Files | [Prompt files](https://code.visualstudio.com/docs/copilot/copilot-customization#_prompt-files-experimental) are reusable prompts for common tasks. | VS Code only | User & Workspace |
| Custom Chat Modes | [Custom chat modes](https://code.visualstudio.com/docs/copilot/chat/chat-modes#_custom-chat-modes) combine instructions and tools for specific workflows. | VS Code only | User & Workspace |
| Tool Sets | Collections of tools for chat, allowing easy switching between tool groups. Not fully documented. | VS Code only | User only |
| MCP Servers | [MCP Servers](https://code.visualstudio.com/docs/copilot/chat/mcp-servers) enable Copilot to call external services via Model Context Protocol. | VS Code & VS | User & Workspace |

## Copilot Feature Library

### Copilot Instructions

Examples for Copilot Instructions can be found in the [.github/copilot-instructions.md](.github/copilot-instructions.md) file.

| Example File | Usage |
|--------------|-------|
| [.github/copilot-instructions.md](.github/copilot-instructions.md) | Place in your repo to set custom Copilot instructions for all contributors. |

### Custom Code Generation Instructions

Examples for Custom Code Generation Instructions can be found in the `.github/` folder (if present, e.g., `csharp-codegen-instructions.md`).

| Example File | Usage |
|--------------|-------|
| `.github/csharp-codegen-instructions.md` | Add to your repo to guide Copilot's code generation for specific scenarios. |

### Prompt Files

Prompt file examples are found in the [`.github/prompts/`](.github/prompts/) folder.

| Example File | Usage |
|--------------|-------|
| [create_github_issues_for_unmet_spec_requirements.prompt.md](.github/prompts/create_github_issues_for_unmet_spec_requirements.prompt.md) | Create GitHub issues for requirements not met in specifications. |
| [create_github_issue_feature_from_spec.prompt.md](.github/prompts/create_github_issue_feature_from_spec.prompt.md) | Generate GitHub issues for new features based on specifications. |
| [create_spec.prompt.md](.github/prompts/create_spec.prompt.md) | Generate technical specifications for projects. |
| [dotnet_best_practices.prompt.md](.github/prompts/dotnet_best_practices.prompt.md) | Review .NET code for best practices and improvements. |
| [dotnet_design_pattern_review.prompt.md](.github/prompts/dotnet_design_pattern_review.prompt.md) | Analyze .NET code for design pattern usage and recommendations. |
| [update_avm_modules_in_bicep.prompt.md](.github/prompts/update_avm_modules_in_bicep.prompt.md) | Update Azure Verified Modules in Bicep templates. |
| [update_llms.prompt.md](.github/prompts/update_llms.prompt.md) | Update Large Language Model configurations and settings. |

### Custom Chat Modes

Chat mode examples are found in the [`.github/chatmodes/`](.github/chatmodes/) folder:

| Example File | Usage |
|--------------|-------|
| [azure_verified_modules_bicep.chatmode.md](.github/chatmodes/azure_verified_modules_bicep.chatmode.md) | Specialized mode for working with Azure Verified Modules in Bicep templates. |
| [expert_dotnet_software_engineer.chatmode.md](.github/chatmodes/expert_dotnet_software_engineer.chatmode.md) | Expert-level guidance for .NET software engineering tasks. |
| [expert_react_frontend_engineer.chatmode.md](.github/chatmodes/expert_react_frontend_engineer.chatmode.md) | Expert-level guidance for React frontend development. |
| [janitor.chatmode.md](.github/chatmodes/janitor.chatmode.md) | Code cleanup and maintenance tasks mode. |
| [mentor.chatmode.md](.github/chatmodes/mentor.chatmode.md) | Provides guidance and support through questioning and hints. |
| [plan.chatmode.md](.github/chatmodes/plan.chatmode.md) | Focused on creating implementation plans and project planning. |
| [semantic_kernel_dotnet.chatmode.md](.github/chatmodes/semantic_kernel_dotnet.chatmode.md) | Specialized mode for Semantic Kernel .NET development. |
| [semantic_kernel_python.chatmode.md](.github/chatmodes/semantic_kernel_python.chatmode.md) | Specialized mode for Semantic Kernel Python development. |
| [specification.chatmode.md](.github/chatmodes/specification.chatmode.md) | Mode for creating technical specifications and documentation. |

### Tool Sets

Tool set examples aren't currently documented in detail, but they allow you to group related tools for easier access in chat. Tool sets are only available in Visual Studio Code and can be configured at the user level.

### MCP Servers

MCP Server configurations are found in the [`.vscode/mcp.json`](.vscode/mcp.json) file.

| Server Name | Usage |
|-------------|-------|
| filesystem | Provides file system access capabilities to Copilot for reading and writing files. |
| playwright | Enables web automation and testing capabilities through Playwright. |
| github | Integrates GitHub API functionality for repository operations and management. |
| giphy | Adds GIF search and integration capabilities through the Giphy API. |