# Skill Template

Use this template to create reusable skills in ozida OS.

---

## Skill Name

(Example: flomo-tag-health-check)

## Purpose

What problem does this skill solve?

## Scope

What is included?
What is not included?

## Inputs

What data does the skill read?

- flomo
- Airtable
- GitHub
- Other

## Capabilities

What can the skill do?

- Analyze
- Summarize
- Compare
- Suggest
- Draft

## Prohibited Actions

What must the skill never do?

- No automatic write
- No data deletion
- No large-scale modification

## Write Policy

Does this skill allow write actions?

Default:

- Read-only
- Write only after confirmation

## Workflow Steps

Describe step-by-step execution:

1. Read rules
2. Read data
3. Analyze
4. Generate output
5. Wait for confirmation if needed

## Output Format

Define how results should be structured.

Example:

- Summary
- Key findings
- Suggestions
- Risks

## Example Usage

User prompt examples:

- "Run this skill on recent data"
- "Analyze and suggest improvements"

## Notes

Additional constraints or context.

---

## One Sentence

This skill helps with ______ while staying within read-first and confirm-before-write principles.