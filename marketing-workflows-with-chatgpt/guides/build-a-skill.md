# Turning a successful chat into a skill

Use a successful task and its corrections as the starting evidence. A skill describes a repeatable procedure. A brief supplies the changing facts. A Project stores ongoing context. An agent or automation additionally needs execution logic and access to tools.

## A prompt to use in chat

> Review this completed task and my corrections. Draft a skill folder with a SKILL.md for repeating this task on a different campaign. Include a clear name and description, required inputs, workflow, output format, and quality checks. Preserve my intent and current authorization. Separate campaign facts from reusable rules. Do not turn incidental choices into permanent requirements. Identify what we have not tested, and propose normal, missing-input, and changed-direction test cases. Show the draft for review.

## File structure

```text
my-skill/
  SKILL.md
```

```yaml
---
name: my-skill
description: Describe the specific task and when this skill applies.
---
```

Add supporting references or scripts only when they make the work more reliable. An instruction-only file is often enough.

## Use and installation

For a manual chat workflow, provide the SKILL.md and explicitly ask ChatGPT to follow it for that task. This is not the same as installation. On supported ChatGPT surfaces use the skill creator and installer options available to your account. In supported Codex repositories, a skill folder under `.agents/skills/` enables repository discovery. Check the [official guide](https://learn.chatgpt.com/docs/build-skills) for current surface-specific behavior and plugin distribution. This educational repository does not create or publish a plugin.

## Test before calling it dependable

Run the same cases with the previous and revised versions. Preserve inputs, outputs, tool access, and version labels. Check whether the instructions help on a new brief and whether they fail gracefully when data is missing. Use the rubric in `templates/skill-evaluation.md`. A metadata validator can check file structure, not creative judgment or statistical correctness.
