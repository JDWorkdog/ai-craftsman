# Setting Up Claude Projects

Claude Projects let you create persistent workspaces with custom instructions, uploaded files, and conversation history. This guide shows you how to set up and use Claude Actions within Projects.

## What are Claude Projects?

Projects are workspaces in Claude.ai that:
- Maintain context across conversations
- Store uploaded files for reference
- Apply custom instructions to all conversations
- Keep conversation history organized

## Creating a Project

1. **Go to Claude.ai**
   - Visit [claude.ai](https://claude.ai)
   - Sign in to your account

2. **Access Projects**
   - Click "Projects" in the left sidebar
   - Or look for the folder icon

3. **Create New Project**
   - Click "New Project" or the + button
   - Give your project a descriptive name (e.g., "Product Work", "Research Hub")

4. **Configure Project** (optional)
   - Add a description
   - Upload relevant files
   - Set custom instructions (this is where Claude Actions go)

## Adding Claude Actions

Claude Actions are custom instructions that give Claude specialized capabilities.

### Steps to Add an Action

1. **Open Project Settings**
   - Click the gear icon in your project
   - Or find "Project Settings" in the menu

2. **Find Custom Instructions**
   - Look for "Custom Instructions" or "Project Instructions"
   - This is where you'll paste the action

3. **Copy the Action**
   - Go to the [claude-actions](../../claude-actions/) directory in this repo
   - Open the action file you want
   - Copy everything below the "---" separator (the actual instructions)

4. **Paste and Save**
   - Paste into your project's custom instructions
   - Click Save

5. **Test It**
   - Start a new conversation in the project
   - Ask Claude to perform the action's task

## Combining Multiple Actions

You can add multiple actions to one project:

```markdown
## Prompt Engineering
[Paste prompt engineering action here]

## Research
[Paste research action here]

## PRD Creation
[Paste PRD action here]
```

Just separate them with headers so they're organized.

## Best Practices

### Organize by Workflow
Create separate projects for different types of work:
- **Product Project** - PRD, user stories, release notes
- **Research Project** - Research, analysis, brainstorming
- **Writing Project** - Emails, content, communication

### Upload Reference Files
Add files that Claude should reference:
- Style guides
- Templates
- Previous examples
- Company documentation

### Keep Instructions Focused
Don't overload custom instructions. If you need many capabilities, consider:
- Creating separate projects
- Using Claude Code instead

## Troubleshooting

### Instructions Not Working
- Make sure you saved the project settings
- Start a new conversation (old conversations may not pick up changes)
- Check for formatting issues in the pasted instructions

### Claude Ignoring Instructions
- Keep instructions clear and specific
- Don't contradict yourself across multiple actions
- Remind Claude of the instructions if needed: "Following the project instructions..."

### File Upload Issues
- Check file size limits
- Ensure file format is supported
- Try re-uploading

## Limitations

| Feature | Supported |
|---------|-----------|
| Custom Instructions | Yes |
| File Uploads | Yes |
| Web Browsing | Depends on plan |
| Code Execution | No |
| File Creation | No |
| Terminal Access | No |

For advanced automation, use [Claude Code](install-claude-code.md) instead.
