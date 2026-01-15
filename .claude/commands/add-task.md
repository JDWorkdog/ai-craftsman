Help me quickly add a task.

**IMPORTANT: Format questions clearly - each question MUST be on its own numbered line. DO NOT combine questions into a paragraph.**

Ask me:
1. What's the task?
2. Category? (work/personal/ideas) - default to inbox if not specified
3. Priority? (High/Medium/Low) - optional
4. Due date? - optional

Then:
- Determine the folder: work, personal, ideas, or _inbox (default)
- Append to `output/tasks/[folder]/tasks.md`
- Format:
  ```
  ## [TASK-###] Task Name
  - **Status**: Not Started
  - **Priority**: [High/Medium/Low]
  - **Due**: [date if provided]

  [Brief description if provided]
  ---
  ```
- Generate sequential TASK-### ID for that folder (check existing tasks.md for last number)
- Create file if it doesn't exist with header: `# [Folder Name] Tasks`
- Confirm what was added and where

**Quick capture is the goal** - don't make me fill out everything. Default to inbox if unclear.
