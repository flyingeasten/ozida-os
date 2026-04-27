# Memo Todo Loop Skill

## Skill Name

memo-todo-loop

## Purpose

This skill manages a lightweight daily todo system based on flomo memos.

It helps identify, organize, and track tasks without turning flomo into a heavy task management system.

## Scope

Included:

- Identify todos from memos
- Generate daily todo list
- Track completion status
- Suggest status updates

Not included:

- Complex project management
- Long-term task planning systems
- Automatic data modification without confirmation

## Inputs

- flomo memos
- Tags such as:
  - #状态/待办
  - #状态/待跟进
  - #状态/已完成
  - #today

## Capabilities

- Extract todo items from memos
- Classify tasks by status
- Generate daily task list
- Suggest updates (complete / follow-up / remove)

## Prohibited Actions

- No automatic modification of memo content
- No automatic tag changes
- No bulk updates without confirmation

## Write Policy

Default behavior:

- Read-only
- Suggest changes
- Wait for user confirmation before updating tags or status

## Workflow Steps

1. Read flomo rules and tag system
2. Read recent memos (default: last 7 days)
3. Identify todos and follow-ups
4. Generate today's todo list
5. Ask user for confirmation on updates

## Output Format

- Today's Todo List
- Follow-up Items
- Suggested Status Changes
- Optional Cleanup Suggestions

## Example Usage

- "Generate today's todo list from my memos"
- "Review my todos and suggest updates"
- "Check if any todos are outdated"

## Notes

This system is designed to stay lightweight.

Do not convert all memos into todos.

Only extract actionable and meaningful tasks.

---

## One Sentence

This skill helps manage daily todos from flomo while keeping the system simple and controlled.