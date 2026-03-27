---
description: How to run the dev server (npm run dev) without hanging
---
To run the dev server without hanging the AI agent:
1. Use the `run_command` tool.
2. Set `CommandLine` to `npm run dev`.
3. Set `Cwd` to the project root directory.
4. Set `WaitMsBeforeAsync` to `2000` (or another small value like 3000) so the process transitions to the background.
5. Do NOT wait for it to finish synchronously. Use `command_status` via the returned `CommandId` if you need to check its output later.
