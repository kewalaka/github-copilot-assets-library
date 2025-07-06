# Prompt Files (experimental)

This folder contains example prompt files (experimental) for GitHub Copilot. For more information on how to use these, see the [GitHub Copilot prompt files](https://code.visualstudio.com/docs/copilot/copilot-customization#_prompt-files-experimental).

## Prompt Files Index

A list of prompt files available in this repository:

| Name | Example File | Usage |
|------|--------------|-------|
| Create Architectural Decision Record | [create_architectural_decision_record.prompt.md](create_architectural_decision_record.prompt.md) | Create an Architectural Decision Record (ADR) document for AI-optimized decision documentation. |
| Create GitHub Issue from Specification | [create_github_issue_feature_from_specification.prompt.md](create_github_issue_feature_from_specification.prompt.md) | Create GitHub Issue for feature request from specification file using feature_request.yml template. |
| Create GitHub Issue from Implementation Plan | [create_github_issues_feature_from_implementation_plan.prompt.md](create_github_issues_feature_from_implementation_plan.prompt.md) | Create GitHub Issues from implementation plan phases using feature_request.yml or chore_request.yml templates. |
| Create GitHub Issues for Unmet Specification Requirements | [create_github_issues_for_unmet_specification_requirements.prompt.md](create_github_issues_for_unmet_specification_requirements.prompt.md) | Create GitHub Issues for unimplemented requirements from specification files using feature_request.yml template. |
| Implementation Plan Update Prompt | [create_implementation_plan.prompt.md](create_implementation_plan.prompt.md) | Create a new implementation plan file for new features, refactoring existing code or upgrading packages, design, architecture or infrastructure. |
| Create LLMs.txt File from Repository Structure | [create_llms.prompt.md](create_llms.prompt.md) | Create an llms.txt file from scratch based on repository structure following the llms.txt specification at https://llmstxt.org/ |
| Generate Standard OO Component Documentation | [create_oo_component_documentation.prompt.md](create_oo_component_documentation.prompt.md) | Create comprehensive, standardized documentation for object-oriented components following industry best practices and architectural documentation standards. |
| Create Specification Prompt | [create_specification.prompt.md](create_specification.prompt.md) | Create a new specification file for the solution, optimized for Generative AI consumption. |
| .NET/C# Best Practices | [dotnet_best_practices.prompt.md](dotnet_best_practices.prompt.md) |  |
| .NET/C# Design Pattern Review | [dotnet_design_pattern_review.prompt.md](dotnet_design_pattern_review.prompt.md) |  |
| Update Azure Verified Modules in Bicep Files | [update_avm_modules_in_bicep.prompt.md](update_avm_modules_in_bicep.prompt.md) | Update Azure Verified Modules (AVM) to latest versions in Bicep files. |
| Implementation Plan Update Prompt | [update_implementation_plan.prompt.md](update_implementation_plan.prompt.md) | Update an existing implementation plan file with new or update requirements to provide new features, refactoring existing code or upgrading packages, design, architecture or infrastructure. |
| Update LLMs.txt File | [update_llms.prompt.md](update_llms.prompt.md) | Update the llms.txt file in the root folder to reflect changes in documentation or specifications following the llms.txt specification at https://llmstxt.org/ |
| Update Markdown File Index | [update_markdown_file_index.prompt.md](update_markdown_file_index.prompt.md) | Update a markdown file section with an index/table of files from a specified folder. |
| Update Standard OO Component Documentation | [update_oo_component_documentation.prompt.md](update_oo_component_documentation.prompt.md) | Update existing object-oriented component documentation following industry best practices and architectural documentation standards. |
| Update Specification | [update_specification.prompt.md](update_specification.prompt.md) | Update an existing specification file for the solution, optimized for Generative AI consumption based on new requirements or updates to any existing code. |


## Usage

To use these prompt files:

1. Copy the desired `.prompt.md` file from this folder to your VS Code user settings folder or workspace `.github/prompts` folder
1. Access the prompt file through the chat interface in VS Code by typing `/` and selecting the prompt from the list

    ![Prompt file execution in Visual Studio Code](../images/run-custom-prompt-file.png)