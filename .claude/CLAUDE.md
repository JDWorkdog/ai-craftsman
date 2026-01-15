# AI Craftsman Workspace

A productivity workspace for Claude Code. Use slash commands to create PRDs, research topics, draft emails, brainstorm, and more.

## Commands

| Command | Purpose | Output |
|---------|---------|--------|
| `/prd` | Create Product Requirements Documents | `output/drafts/` |
| `/research` | Research any topic | `output/research/` |
| `/prompt` | Build AI prompts | `output/prompts/` |
| `/extract-style` | Extract brand styles | `output/analysis/` |
| `/email` | Draft professional emails | (screen) |
| `/brainstorm` | Generate ideas | `output/brainstorms/` |
| `/add-task` | Quick task capture | `output/tasks/` |
| `/user-story` | Write user stories | `output/drafts/` |
| `/daily` | Daily journal | `output/journal/` |

## Output Folder

All generated content lives in `output/`. This folder is gitignored so your work stays private.

- `research/` - Research reports
- `drafts/` - PRDs, user stories, documents
- `prompts/` - Saved AI prompts
- `brainstorms/` - Brainstorming sessions
- `tasks/` - Task lists (inbox, work, personal, ideas)
- `journal/` - Daily entries
- `analysis/` - Style guides

## Task Folders

Tasks are organized into 4 simple folders:
- `_inbox/` - Quick capture, sort later (default)
- `work/` - Work-related tasks
- `personal/` - Personal tasks
- `ideas/` - Someday/maybe items

## Auto-Journaling

When you talk about your day - accomplishments, tasks, plans - Claude automatically logs it to your journal. You don't need to run `/daily` explicitly.

## File Naming

- Journal: `YYYY-MM-DD-DAY.md` (e.g., `2025-01-15-WED.md`)
- Other files: `YYYY-MM-DD_topic_type.md` (e.g., `2025-01-15_user-auth_prd.md`)

## Permissions

Claude can create and update journal and task files without asking. This keeps the flow smooth for daily capture.

## Reference Materials

- `/prompts/` - Universal prompts for Claude, ChatGPT, Gemini
- `/guides/` - Role-based starting points
- `/resources/` - Getting started docs
- `/_examples/` - Sample file formats
