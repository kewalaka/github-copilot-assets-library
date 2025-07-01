# Prompt Files (experimental)

This folder contains example prompt files (experimental) for GitHub Copilot. For more information on how to use these, see the [GitHub Copilot prompt files](https://code.visualstudio.com/docs/copilot/copilot-customization#_prompt-files-experimental).

## Prompt Files Index

A list of prompt files available in this repository:

| Name | Example File | Usage |
|------|--------------|-------|
| Create GitHub Issues for Unmet Requirements | [create_github_issues_for_unmet_spec_requirements.prompt.md](create_github_issues_for_unmet_spec_requirements.prompt.md) | Create GitHub issues for requirements not met in specifications. |
| Create GitHub Issue from Spec | [create_github_issue_feature_from_spec.prompt.md](create_github_issue_feature_from_spec.prompt.md) | Generate GitHub issues for new features based on specifications. |
| Create Plan | [create_plan.prompt.md](create_plan.prompt.md) | Create a new implementation plan file for features, refactoring, upgrades, or architecture, optimized for Generative AI. |
| Create Specification | [create_specification.prompt.md](create_specification.prompt.md) | Create a new specification file for the solution, optimized for Generative AI consumption. |
| .NET Best Practices Review | [dotnet_best_practices.prompt.md](dotnet_best_practices.prompt.md) | Review .NET code for best practices and improvements. |
| .NET Design Pattern Review | [dotnet_design_pattern_review.prompt.md](dotnet_design_pattern_review.prompt.md) | Analyze .NET code for design pattern usage and recommendations. |
| Update AVM Modules in Bicep | [update_avm_modules_in_bicep.prompt.md](update_avm_modules_in_bicep.prompt.md) | Update Azure Verified Modules in Bicep templates. |
| Update LLMs | [update_llms.prompt.md](update_llms.prompt.md) | Update Large Language Model configurations and settings. |
| Update Markdown File Index | [update_markdown_file_index.prompt.md](update_markdown_file_index.prompt.md) | Update a markdown file section with an index/table of files from a specified folder. |
| Update Plan | [update_plan.prompt.md](update_plan.prompt.md) | Update an existing implementation plan file with new or updated requirements to provide new features, refactoring existing code or upgrading packages, design, architecture or infrastructure. |
| Update Specification | [update_spec.prompt.md](update_spec.prompt.md) | Update an existing specification file for the solution, optimized for Generative AI consumption based on new requirements or updates to any existing code. |

## Usage

To use these prompt files:

1. Copy the desired `.prompt.md` file from this folder to your VS Code user settings folder or workspace `.github/prompts` folder
1. Access the prompt file through the chat interface in VS Code by typing `/` and selecting the prompt from the list

    ![Prompt file execution in Visual Studio Code](images/run-custom-prompt-file.png)
