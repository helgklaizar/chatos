<div align="center">

# ChatOS

### The chat-first GUI for Linux. Your desktop becomes a conversation.

> 🔓 **The source code will be open to the community soon.** Star ⭐ and watch the repo to get notified.

[Website](https://chatos.dev) · [Join the whitelist](https://chatos.dev) · [Discussions](../../discussions)

</div>

---

## Why

Desktop GUIs haven't really changed since Xerox PARC in the 1970s: a desk, folders, icons, windows and a trash can. That design assumed a person who does everything by hand, moving between apps and carrying data from one to the next.

That isn't how we work anymore. With AI agents (Claude Code, Antigravity, Codex and others) most of the day happens **in one chat window**. You describe what you need and the agent does it: code, files, servers, deploys, email, messengers.

Everything around that window (docks, taskbars, start menus, piles of windows) is a leftover from the old way.

**ChatOS removes it.** You boot straight into an agent manager that acts as your shell, launcher and desktop at the same time.

## How it works

| Layer | In a classic desktop | In ChatOS |
|---|---|---|
| **Core interface** | Desktop, windows, app icons | A chat with your AI agent |
| **Apps & services** | Separate apps with their own windows | **MCP connectors**: WhatsApp, Telegram, email, calendar, Git, servers, CRM… |
| **System info** | Tray icons, widgets, task manager | Built into the chat UI: clock, CPU/RAM, network, battery, **model limits & token usage**, background agents |
| **Visual content** | Every app opens its own window | Rendered **on demand** inline (documents, previews, charts) and dismissed by the agent |

```
┌──────────────────────────────────────────────────────────┐
│ ● agent online   cpu 12%   ram 41%   tokens 84%   14:32  │  ← system bar inside the chat
├──────────────────────────────────────────────────────────┤
│                                                          │
│  you ▸ deploy the landing to prod and reply to Dan on    │
│        WhatsApp that it's live                           │
│                                                          │
│  agent ▸ ✓ built & deployed → https://chatos.dev         │
│          ✓ WhatsApp → Dan: "It's live 🚀"                │
│                                                          │
│  ┌ preview ───────────────────────┐                      │  ← inline, on-demand UI
│  │  [ rendered page screenshot ]  │                      │
│  └────────────────────────────────┘                      │
├──────────────────────────────────────────────────────────┤
│ ▸ type a task…                              [mcp: 7 on]  │
└──────────────────────────────────────────────────────────┘
```

## Principles

- **Chat is the shell.** One place for intent, execution and results.
- **Apps become capabilities.** Every service is a connector (MCP) the agent can use, not a window you have to manage.
- **System status in context.** Hardware, network and AI quota live where you work.
- **Windows only when needed.** Visual UI is generated on demand, not left open all day.
- **Linux underneath.** A stable, open base. ChatOS replaces the desktop environment, not the kernel.
- **Model-agnostic.** Bring your own agent and models, cloud or local.

## Status

🚧 **Early development.** A working prototype runs on top of Linux. We're preparing the first public release.

- [x] Concept & architecture
- [x] Prototype shell on Linux
- [ ] Connector SDK (MCP)
- [ ] System widgets (CPU, RAM, network, model limits)
- [ ] Closed beta for whitelist testers
- [ ] Public open-source release

## Early access

We're picking the first testers now. **[Join the whitelist →](https://chatos.dev)**

## License

To be announced with the open-source release.
