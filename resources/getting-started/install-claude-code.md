# Installing Claude Code

Claude Code is Anthropic's CLI tool that brings Claude into your development environment. This guide covers installation for VSCode and terminal.

## Prerequisites

- An Anthropic account with API access
- Node.js 18+ (for CLI installation)
- VSCode (for extension installation)

## Option 1: VSCode Extension (Recommended)

The easiest way to use Claude Code is through the VSCode extension.

### Installation Steps

1. **Open VSCode**

2. **Open Extensions**
   - Press `Cmd+Shift+X` (Mac) or `Ctrl+Shift+X` (Windows/Linux)
   - Or click the Extensions icon in the sidebar

3. **Search for Claude Code**
   - Type "Claude Code" in the search box
   - Look for the official extension by Anthropic

4. **Install**
   - Click "Install"
   - Wait for installation to complete

5. **Authenticate**
   - Open the Command Palette: `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P`
   - Type "Claude Code: Sign In"
   - Follow the authentication flow

6. **Start Using**
   - Open the Claude Code panel from the sidebar
   - Or use `Cmd+Shift+P` → "Claude Code: Open"

## Option 2: CLI Installation

For terminal-based usage or integration with other tools.

### Installation Steps

1. **Install via npm**
   ```bash
   npm install -g @anthropic-ai/claude-code
   ```

2. **Authenticate**
   ```bash
   claude auth login
   ```
   Follow the prompts to sign in.

3. **Verify Installation**
   ```bash
   claude --version
   ```

4. **Start Using**
   ```bash
   claude
   ```
   This opens an interactive session.

## Configuration

### Setting Up Commands

1. Create a `.claude/` directory in your project root:
   ```bash
   mkdir -p .claude/commands
   ```

2. Add command files (`.md` files) to `.claude/commands/`

3. Commands are available as `/command-name`

### Setting Up Skills

1. Create a `skills/` directory in your project:
   ```bash
   mkdir skills
   ```

2. Copy skill folders into this directory

3. Skills are automatically available to Claude

## Troubleshooting

### "Command not found"
- Ensure Node.js is installed: `node --version`
- Try reinstalling: `npm install -g @anthropic-ai/claude-code`

### Authentication Issues
- Clear credentials: `claude auth logout`
- Re-authenticate: `claude auth login`
- Check your Anthropic account has API access enabled

### Extension Not Working
- Reload VSCode: `Cmd+Shift+P` → "Developer: Reload Window"
- Check the Output panel for errors
- Ensure you're signed in

## Resources

- [Official Documentation](https://docs.anthropic.com/en/docs/claude-code)
- [Anthropic Console](https://console.anthropic.com) - Manage API keys
- [Claude Code GitHub](https://github.com/anthropics/claude-code)
