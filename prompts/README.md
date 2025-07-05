# Prompt Files (experimental)

This folder contains example prompt files (experimental) for GitHub Copilot. For more information on how to use these, see the [GitHub Copilot prompt files](https://code.visualstudio.com/docs/copilot/copilot-customization#_prompt-files-experimental).

## Prompt Files Index

A list of prompt files available in this repository:

| Name | Example File | Usage |
|------|--------------|-------|
| Create Architectural Decision Record (ADR) | [create_architectural_decision_record.prompt.md](create_architectural_decision_record.prompt.md) | Generate a comprehensive Architectural Decision Record (ADR) document that captures the context, decision, consequences, and alternatives for important technical decisions made during software development or system design. |
| Create GitHub Issues for Unmet Requirements | [create_github_issues_for_unmet_spec_requirements.prompt.md](create_github_issues_for_unmet_spec_requirements.prompt.md) | Create GitHub Issues for each requirement in a specification file that is not already implemented in the codebase using the GitHub Issue template feature_request.yml. |
| Create GitHub Issue from Spec | [create_github_issue_feature_from_spec.prompt.md](create_github_issue_feature_from_spec.prompt.md) | Create a GitHub Issue for a feature request using the GitHub Issue template feature_request.yml from a specification file. |
| Create Implementation Plan | [create_implementation_plan.prompt.md](create_implementation_plan.prompt.md) | Create a new implementation plan file for new features, refactoring existing code or upgrading packages, design, architecture or infrastructure. |
| Create Specification | [create_specification.prompt.md](create_specification.prompt.md) | Create a new specification file for the solution, optimized for Generative AI consumption. |
| .NET Best Practices Review | [dotnet_best_practices.prompt.md](dotnet_best_practices.prompt.md) | Ensure .NET/C# code meets best practices specific to the solution/project including documentation, structure, and design patterns. |
| .NET Design Pattern Review | [dotnet_design_pattern_review.prompt.md](dotnet_design_pattern_review.prompt.md) | Review C#/.NET code for design pattern implementation and suggest improvements for the solution/project. |
| Update AVM Modules in Bicep | [update_avm_modules_in_bicep.prompt.md](update_avm_modules_in_bicep.prompt.md) | Update Azure Verified Modules to latest versions in Bicep files. |
| Update Implementation Plan | [update_implementation_plan.prompt.md](update_implementation_plan.prompt.md) | Update an existing implementation plan file with new or update requirements to provide new features, refactoring existing code or upgrading packages, design, architecture or infrastructure. |
| Update LLMs | [update_llms.prompt.md](update_llms.prompt.md) | Update the llms.txt file in the root folder to reflect changes in documentation or specifications. |
| Update Markdown File Index | [update_markdown_file_index.prompt.md](update_markdown_file_index.prompt.md) | Update a markdown file section with an index/table of files from a specified folder. |
| Update Specification | [update_specification.prompt.md](update_specification.prompt.md) | Update an existing specification file for the solution, optimized for Generative AI consumption based on new requirements or updates to any existing code. |

## Usage

To use these prompt files:

1. Copy the desired `.prompt.md` file from this folder to your VS Code user settings folder or workspace `.github/prompts` folder
1. Access the prompt file through the chat interface in VS Code by typing `/` and selecting the prompt from the list

    ![Prompt file execution in Visual Studio Code](images/run-custom-prompt-file.png)
