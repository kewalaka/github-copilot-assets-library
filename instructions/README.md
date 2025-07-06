# Custom Instructions

This folder contains example custom instructions for GitHub Copilot. For more information on how to use these, see the [GitHub Copilot custom instructions](https://code.visualstudio.com/docs/copilot/copilot-customization#_custom-instructions).

## Available Instruction Files

| File | Pattern | Description |
|------|---------|-------------|
| [azure-developer-solution-accelerator.md](azure-developer-solution-accelerator.md) | `**` |  |
| [copilot-thought-logging.instructions.md](copilot-thought-logging.instructions.md) | `**` | See process Copilot is following where you can edit this to reshape the interaction or save when follow up may be needed |
| [csharp-14-best-practices.instructions.md](csharp-14-best-practices.instructions.md) | `**/*.cs` |  |
| [csharp-best-practices.instructions.md](csharp-best-practices.instructions.md) | `**/*.cs` |  |
| [markdown.instructions.md](markdown.instructions.md) | `**/*.md` | Documentation and content creation standards |


## Usage

To use these instructions:

1. Copy the desired `.instructions.md` file to your VS Code user settings folder or workspace `.github/instructions` folder
1. Select the new instruction set through the chat interface in VS Code
