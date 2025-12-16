# Claude Actions

Claude Actions are reusable workflows you can add to your Claude.ai Projects. Unlike Claude Code (which requires VSCode), Claude Actions work directly in the Claude.ai web interface.

## What are Claude Actions?

When you create a Project in Claude.ai, you can add "Custom Instructions" that guide Claude's behavior. Claude Actions are pre-built instructions that give Claude specialized capabilities for specific tasks.

## How to Use

### Step 1: Create or Open a Project
1. Go to [claude.ai](https://claude.ai)
2. Click on "Projects" in the sidebar
3. Create a new project or open an existing one

### Step 2: Add the Action
1. Click the gear icon to open project settings
2. Find "Custom Instructions" or "Project Instructions"
3. Copy the contents of the action file (everything below the setup instructions)
4. Paste into your project's custom instructions
5. Save the project

### Step 3: Use the Action
Start a conversation in your project. The action's capabilities are now available. You can:
- Ask Claude to perform the action's task
- Reference the action by name
- Claude will follow the workflow defined in the action

## Available Actions

Browse the `.md` files in this directory. Each file contains:
- **Description** - What the action does
- **Setup Instructions** - How to add it to your project
- **The Action Itself** - The instructions to copy

## Tips

### Combining Actions
You can add multiple actions to a single project by combining their instructions. Just make sure they don't conflict.

### Customizing Actions
Feel free to modify the instructions to fit your specific needs. Add your company name, preferred formats, or additional context.

### Project Organization
Create separate projects for different workflows:
- "Product Work" project with PRD and user story actions
- "Research" project with research and analysis actions
- "Writing" project with email and content actions

## Limitations vs Claude Code

Claude Actions are simpler but more limited than Claude Code:

| Feature | Claude Actions | Claude Code |
|---------|---------------|-------------|
| Web Interface | Yes | No (VSCode/CLI) |
| File Access | Upload only | Full read/write |
| Terminal Access | No | Yes |
| Complexity | Simple workflows | Advanced automation |
| Setup | Copy/paste | Installation required |

For simple, repeatable prompts, Claude Actions are perfect. For complex automation with file manipulation, use Claude Code.
