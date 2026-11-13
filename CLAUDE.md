## Cross-session messages
- When a message from another session arrives, hand it to the `peer-router` agent first.
- If the router says "sync", hand the work to the `peer-sync-editor` agent.
- Send messages to other sessions with SendMessage as short plain text. Don't paste
  conversation history, file dumps or tool output. Just say what changed and where.
- Before any commit, the main session (Opus) reviews the diff and gives final sign-off.
  It also decides whether another session's request is allowed at all.
