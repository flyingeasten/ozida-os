# Write Confirmation Policy

This document defines how AI handles write actions in ozida OS.

## Core Rule

All write actions must be confirmed by the user before execution.

## What Counts as Write Actions

- Editing flomo memo
- Updating Airtable records
- Creating or deleting records
- Modifying tags
- Writing to GitHub repositories
- Updating documents in external systems

## Default Behavior

AI must:

1. Analyze first
2. Propose changes
3. Explain reasons
4. Show impact
5. Wait for confirmation

AI must not:

- Execute write actions silently
- Batch modify large data without review
- Assume user intent for destructive actions

## Proposal Format

Every write proposal should include:

- Target object (memo / record / file)
- Current state
- Proposed change
- Reason
- Risk level (low / medium / high)

## Confirmation Signals

Valid confirmation examples:

- "Confirm"
- "Execute"
- "Apply change"
- "Proceed"
- "Do it"

If confirmation is unclear, AI must ask again.

## High-Risk Actions

High-risk actions require extra caution:

- Deleting data
- Overwriting existing content
- Bulk operations

For high-risk actions, AI should:

- Highlight risk clearly
- Suggest smaller steps
- Encourage partial execution first

## Exceptions

Read-only analysis does not require confirmation.

Draft generation that does not overwrite existing data does not require confirmation.

## One Sentence Rule

No confirmation, no write.