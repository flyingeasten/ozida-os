# Memo Todo Loop Trigger

## Purpose

Provide a simple entry point to run the memo-todo-loop skill using natural language.

This file is not the skill itself.

It tells an agent how to recognize user intent and route the request to the correct memo-todo-loop step.

## User Trigger Examples

The user may say:

- 今日待办
- 今天要做什么
- 最近有哪些待办
- 帮我整理这些 memo
- 这些需要我做吗
- 今天做完了吗
- 收尾一下

## Instruction to Agent

When the user input matches todo-related intent:

1. Read the skill entry:
   - skills/memo-todo-loop/SKILL.md

2. Read the needed step file:
   - skills/memo-todo-loop/detect.md
   - skills/memo-todo-loop/morning.md
   - skills/memo-todo-loop/review.md

3. Route by intent:
   - 今日待办 / 今天要做什么 → detect + morning
   - 最近有哪些待办 / 帮我整理这些 memo → detect
   - 今天做完了吗 / 收尾一下 → review

4. Follow the global write policy:
   - principles/write-confirmation-policy.md

## Rules

- Read flomo tag rules first when available
- Default to read-only analysis
- Do not modify memo content or tags without confirmation
- Keep output concise and actionable
- Do not expose internal reasoning

## One Line

Natural language → intent routing → memo-todo-loop skill → correct step execution.