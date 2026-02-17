---
name: gemini-cli
description: Use the Gemini CLI for code analysis, autonomous terminal tasks, and project management. Trigger this skill when the user wants to use Gemini as a sub-agent to handle complex coding tasks via its terminal interface.
---

# Gemini CLI Skill

This skill allows OpenClaw agents to operate the Gemini CLI as an autonomous sub-agent for fullstack development.

## Quick Start Workflow

1. **Enter Project**: `cd /path/to/project`
2. **Launch**: Run `gemini`
3. **Initialize**: Immediately run `/init` to generate the project's `GEMINI.md`.

## Core Operation

### Context Awareness
- Always use `@filename` to load specific file context before executing complex tasks.
- If you need to run terminal commands, use the shell mode prefix `!`.

### Tactical Performance
- **Token Management**: Use `/compress` as soon as the conversation feels long to maintain speed and save costs.
- **YOLO Mode**: Enable `Ctrl+Y` for high-autonomy workflows to bypass confirmation prompts for tools.

## Command Reference
For a complete list of slash commands and shortcuts, see [cli-reference.md](references/cli-reference.md).

## Safety
- **YOLO Warning**: While YOLO mode is efficient, review the content of shell commands (`!`) carefully, as you have full system permissions.
- **Verification**: Use `/stats session` to monitor resource usage.
