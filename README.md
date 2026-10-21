# {{CLIENT_NAME}} ({{CLIENT_SHORT}})

> **Template:** if [SETUP.md](SETUP.md) still exists, this repository has not been set up for a client yet. Start there.

Knowledge base for our work with {{CLIENT_NAME}}: one or two sentences on who they are.

**The short version:** what the client's situation is, what we are doing about it, and what comes later. Keep it to three sentences.

**Start with [AGENTS.md](AGENTS.md)**, then [project/status.md](project/status.md).

| Folder | What it is |
| --- | --- |
| [client/](client/) | Who {{CLIENT_SHORT}} is: company, people, brand, competitors |
| [project/](project/) | Our work: status, scope, roadmap, open questions |
| [research/](research/) | Audits and research, dated |
| [deliverables/](deliverables/) | Reports and other files we hand to the client |
| [map/](map/) | Accounts, domains, tools, where logins are kept |
| [decisions/](decisions/) | Why things are the way they are |
| [logs/](logs/) | What already happened |
| [templates/](templates/) | Log, decision and research templates |

## Starting a new session

- **Claude (claude.ai or the Claude app):** start the chat with: "We're working on the {{CLIENT_SHORT}} knowledge base in `{{REPO}}`. Pull it and read AGENTS.md before anything else."
- **Claude Code on your computer:** clone the repo, open a terminal in it and run `claude`. `CLAUDE.md` loads automatically.
- **Other AI tools (Cursor, Codex and similar):** open the repo; they read `AGENTS.md`.
- **Chatbots without repo access:** paste `AGENTS.md` and `project/status.md` at the start.

Every session ends by committing and pushing its changes.

Private repository. No plain-text passwords or keys; see [AGENTS.md](AGENTS.md#credentials).
