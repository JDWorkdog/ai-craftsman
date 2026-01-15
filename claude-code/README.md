# Claude Code Commands & Skills

> **Note:** Commands have moved to `.claude/commands/` in the project root. This folder is kept for reference only. When you clone this repo, the commands are already set up and ready to use.

## Quick Start

If you cloned this repo, commands are already available. Just run:
```
/prd
/research
/brainstorm
```

See the main [README](../README.md) for the full list of available commands.

---

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

## Creating Your Own Commands

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

Place command files in `.claude/commands/` in your project root.

## Reference Commands

The `commands/` folder here contains the original prompts used to create the active commands in `.claude/commands/`. These are kept for reference and can be used to understand the command structure.

## Reference Prompts

For prompts that work across multiple LLMs (Claude, ChatGPT, Gemini), see the [prompts/](../prompts/) directory.
