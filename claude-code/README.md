# Claude Code Commands & Skills

This directory contains commands and skills for [Claude Code](https://docs.anthropic.com/en/docs/claude-code), Anthropic's CLI tool for Claude that integrates with VSCode.

## What is Claude Code?

Claude Code is a command-line tool and VSCode extension that lets you interact with Claude directly in your development environment. It supports:

- **Slash Commands** - Quick workflows triggered with `/command-name`
- **Skills** - Modular capability packages for specialized tasks
- **File Access** - Claude can read, edit, and create files
- **Terminal Access** - Claude can run shell commands

## Installation

See our detailed guide: [Install Claude Code](../resources/getting-started/install-claude-code.md)

**Quick Start:**
1. Install the VSCode extension: Search "Claude Code" in Extensions
2. Or install the CLI: `npm install -g @anthropic-ai/claude-code`
3. Authenticate with your Anthropic API key

## Using Commands

### Installing Commands
1. Create a `.claude/commands/` directory in your project root
2. Copy command `.md` files from this repo's `commands/` folder
3. Restart Claude Code or reload the window

### Running Commands
In Claude Code, type `/` followed by the command name:
```
/prd
/research
/prompt
```

Claude will execute the workflow defined in the command file.

## Using Skills

### Installing Skills
1. Create a `skills/` directory in your project root
2. Copy skill folders from this repo's `skills/` directory
3. Skills are available immediately

### Invoking Skills
Skills are typically invoked by Claude when relevant, or you can ask Claude to use a specific skill:
```
"Use the document-skills to create a PowerPoint deck"
```

## Directory Structure

```
claude-code/
├── commands/           # Slash commands (.md files)
│   ├── prompt.md       # Prompt engineering workflow
│   ├── prd.md          # PRD creation workflow
│   └── ...
└── skills/             # Skill packages (folders)
    ├── document-skills/
    └── ...
```

## Creating Your Own

### Commands
Commands are Markdown files that define a workflow. See [Anthropic's documentation](https://docs.anthropic.com/en/docs/claude-code/tutorials/custom-commands) for details.

Basic structure:
```markdown
Description of what this command does.

Ask me:
1. First question?
2. Second question?

Then:
- Step one
- Step two
- Step three
```

### Skills
Skills are more complex packages. See the skill-creator guide for details on building your own skills.
