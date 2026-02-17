# Gemini CLI Reference

## Core Syntax
- `@<path>`: Attach files or directories to the context (e.g., `@src/index.ts`).
- `!<command>`: Shell execution mode (e.g., `!npm test`).

## Slash Commands
### 1. Project & Context
- `/init`: Analyze the project and create `GEMINI.md`.
- `/directory add <path>`: Add directories to the workspace.
- `/memory show` / `/memory refresh`: Interact with session memory.

### 2. Tools & MCP
- `/tools`: List internal tools.
- `/mcp list` / `/mcp refresh`: Manage Model Context Protocol servers.
- `/skills list` / `/skills enable <name>`: Management of agent skills.

### 3. Session Control
- `/compress`: Essential! Use this and save tokens by summarizing the session history.
- `/stats session`: Check current token usage.
- `/chat save <tag>` / `/chat resume <tag>`: Save/Load session states.
- `/clear`: Clear terminal display.
- `/quit`: Exit terminal session.

## Shortcuts (Terminal Emulation)
- `Ctrl+Y`: Toggle **YOLO Mode** (No confirmation required for commands).
- `Shift+Tab`: Toggle auto-accept for code edits.
- `Ctrl+J`: Add newline without sending.
- `Ctrl+L`: Clear screen.
