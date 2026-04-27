# Memo Todo Loop Skill

## Purpose

Manage a lightweight todo system based on flomo memos.

## Entry

User triggers using natural language.

## Intent Routing

If user intent matches:

- 今日待办 → detect + morning
- 今天要做什么 → detect + morning
- 有哪些待办 → detect only
- 今天做完了吗 → review

## Workflow

1. Read flomo tag system
2. Read recent memos
3. Route intent
4. Execute steps
5. Output result
6. Suggest changes (no write)

## Write Policy

- Read-only by default
- All updates require confirmation

## Steps

- detect.md
- morning.md
- review.md

## One Sentence

Lightweight todo workflow driven by flomo and user intent.