# Memo Todo Loop Skill

## Skill Name

memo-todo-loop

## Positioning

Memo Todo Loop is one complete skill with three internal steps.

It is not three separate skills.

- detect.md: identify todo and follow-up items
- morning.md: generate the daily lightweight list
- review.md: close the loop and prepare status updates

## Purpose

Manage a lightweight daily todo loop based on flomo memos and the existing flomo tag system.

The goal is not to turn flomo into a full project management system.

The goal is to help the user see what needs attention today, follow up on unfinished items, and clean up status tags after confirmation.

## Entry

The user triggers this skill with natural language.

Examples:

- 今日待办
- 今天要做什么
- 最近有哪些待办
- 帮我整理这些 memo
- 今天做完了吗
- 收尾一下

## Intent Routing

Route by user intent:

1. Triage / detect intent
   - User asks: 哪些是待办 / 帮我整理这些 memo / 这些需要我做吗
   - Run: detect.md

2. Morning list intent
   - User asks: 今日待办 / 今天要做什么 / 帮我生成今天清单
   - Run: detect.md + morning.md

3. Closeout / review intent
   - User asks: 今天做完了吗 / 收尾一下 / 更新今日状态
   - Run: review.md

4. Unclear intent
   - Ask a short clarification or default to read-only detect.

## Required Rule Sources

Before running this skill, read the relevant flomo rule memos when available:

- 状态标签规则
- Memo Todo Loop 工作流说明
- AI 识别待办 / 待跟进规则
- Memo Todo Loop 早晨清单生成规则
- Memo Todo Loop 收尾确认与状态回写规则
- Memo Todo Loop 预约型待办规则

## Core Principles

- flomo keeps the original record.
- AI organizes and suggests, but does not silently rewrite.
- Not every memo becomes a todo.
- Status tags are temporary and should be cleaned regularly.
- The daily list should stay small: usually 3 to 7 items.
- Use existing tags before creating new ones.
- Keep the system lightweight.

## Write Policy

Default mode is read-only.

Allowed without confirmation:

- Read memos
- Analyze memos
- Generate lists
- Suggest tags
- Suggest status changes

Requires explicit confirmation:

- Edit memo content
- Add or remove tags
- Change status tags
- Save a daily list back to flomo
- Bulk update any memo

## Output Requirements

For morning list:

- Item
- Source
- Current status
- Next action
- Priority
- Need confirmation: yes / no

For review:

- Item
- Current status
- Suggested new status
- Reason
- Need confirmation: yes / no

## File Responsibilities

README.md is for human understanding.

SKILL.md is the routing and operating entry for AI.

detect.md, morning.md, and review.md are step files.

## One Sentence

Memo Todo Loop is a lightweight flomo-based todo loop: detect, plan, review, and update only after confirmation.
