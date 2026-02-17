# Gemini CLI Reference

## Core Syntax
- `@<path>`: Attach files or directories to the context (e.g., `@src/index.ts`).
- `!<command>`: Shell execution mode (e.g., `!npm test`).

## Slash Commands
### 1. Project & Context
- `/init`: Analyzes the project and creates a tailored `GEMINI.md` file. (Run this first!)
- `/directory`: Manage workspace directories.
    - `add`: Add directories (comma-separated).
    - `show`: Show active directories.
- `/memory`: Interact with long-term memory and `GEMINI.md` inputs.
    - `show`: Show memory contents.
    - `add`: Add content to memory.
    - `refresh`: Refresh from source.
    - `list`: Show paths of `GEMINI.md` files in use.

### 2. Tools & MCP & Skills
- `/tools [desc]`: List available Gemini CLI tools.
- `/mcp`: Model Context Protocol management.
    - `list / desc / schema`: List servers with varying detail.
    - `refresh`: Restart MCP servers.
    - `enable / disable`: Toggle servers.
- `/skills`: Manage agent skills.
    - `list / enable / disable / reload`.

### 3. Session & Performance
- `/compress`: **Essential!** Replaces context with a summary to save tokens.
- `/stats [session|model|tools]`: Check usage statistics.
- `/chat`: Manage checkpoints.
    - `save <tag> / resume <tag> / list / delete`.
    - `share <file>`: Export to markdown/json.
- `/copy`: Copy last result/code to clipboard.
- `/rewind`: Jump back to a specific message and restart.
- `/clear`: Clear screen and history.
- `/quit`: Exit the CLI.

### 4. System & Dev
- `/auth [login|logout]`: Manage credentials.
- `/config`: Open model configuration dialog.
- `/settings`: View and edit CLI settings.
- `/doctor`: Check installation.
- `/update`: Manage extensions.

## Keyboard Shortcuts
- **Ctrl+Y**: Toggle **YOLO Mode** (No confirmation for tool execution).
- **Shift+Tab**: Toggle **Auto-accept** edits.
- **Ctrl+J**: New line in prompt.
- **Ctrl+L**: Clear screen.
- **Ctrl+X**: Open input in external editor.
- **Ctrl+S**: Selection mode (copy text).
- **Page Up/Down**: Scroll.
- **Up/Down**: Command history.
- **Esc**: Cancel operation (double press to clear input).
