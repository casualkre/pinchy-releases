---
title: "Your other agents: Claude Code, Cursor, opencode, pi and Hermes"
description: "If you run coding agents yourself in your terminals, Pinchy can look after them: he tells you how they are doing, answers their harmless permission questions, asks you about the risky ones and passes messages between them. It is off until you switch it on."
keywords: "other agents, your other agents, manage my agents, coding agents, claude code, cursor, cursor-agent, opencode, pi, hermes, terminal, herdr, green dot, icons beside pinchy, needs you, approve, permission, smart approvals, always allow, hook, connect, disconnect, pinchy-say, talk to each other, message another agent"
permalink: /your-other-agents/
---
# Your other agents: Claude Code, Cursor, opencode, pi and Hermes

If you run coding agents yourself in your terminals, Pinchy can look after them: he tells you how they are doing, answers their harmless permission questions, asks you about the risky ones and passes messages between them. It is off until you switch it on.

## What to ask for
- "What are my coding agents doing?" He lists every one he sees, what it is doing and its last line.
- "What did Claude Code in my frontend folder say last?" He reads that one agent for you.
- "Tell my Claude Code in the frontend folder to also run the end-to-end tests before it finishes." He passes the message on; it reaches the agent between its steps.
- "Tell the backend agent what the frontend one found." He carries it over in its own words.

## How it works
- **Icons beside Pinchy.** Every agent he sees gets a small icon next to him with a dot: green when he manages it, a green ring when it is open but not managed, amber and pulsing when it needs you, red when it failed, grey when it finished or closed. The ones that need you come first; with many open you see six and a "+N".
- **The card.** Click an icon: you see its name, its folder, what it is doing, its last line and any request waiting for you with **Allow** and **Refuse**. **Manage** / **Managing** switches Pinchy on or off for that one agent, **Say…** sends it a message, **Open** brings its terminal to the front (in herdr) or opens its folder.
- **He keeps you posted** in his chat: when one finishes ("Claude Code in ~/app finished: …"), when one needs you, when one failed. Things he allowed on his own are folded into one short line now and then, not one line each.
- **Smart approvals.** When a managed agent asks for permission, Pinchy decides:
  - He allows reading and searching (not files that can hold passwords or keys), editing files inside the agent's own project, and harmless commands such as `ls`, `git status` or `git diff`.
  - Running code (a script, the project's build or its tests) passes without asking only when that code is exactly what the project's last commit holds. Code that is new or changed since then comes to you.
  - Anything risky comes to you in his normal approval window, on your phone or in Telegram: pushing, deleting, root, the internet, a file outside the project, anything he does not know.
  - Some things he always refuses: touching Pinchy's own data or keys, changing an agent tool's own permission settings, wiping a home folder or a disk.
  - Nobody answers within the time set in Settings → Safety & data → Safety ("Auto-deny permission requests after")? Then the tool simply asks in its own window, as it would without Pinchy.
- **"Always allow"** is offered for a run of code or tests: it covers that one tool, in that one project, for that exact command only. `npm test` never covers `npm test; curl …`. The window says what it will cover before you press it. Your remembered answers are listed under **Remembered permissions** in Settings → Safety & data → Safety.
- **They can talk to each other.** A managed agent learns its own id and who else is open, and can write to another one with the small `pinchy-say` command Pinchy gives it. The message reaches the other agent between its steps, or when it stops; it can answer the same way. One agent can send at most 30 messages an hour, and an idle agent in a herdr pane is woken at most once a minute. Messages from you or from Pinchy are never limited.
- **Connect.** For each tool Pinchy adds a small hook to that tool's own settings, so he hears from it and can answer it. Disconnect takes out only his part and leaves your own hooks alone. While Pinchy is closed, every tool works exactly as it does without him.
- **Pinchy's own sessions** (his chat, his agents, Workspace jobs, swarms) are never listed here, not even one of his conversations you reopen in a terminal; this is only about the agents you run yourself.

## Settings
Settings → Agents & automation → Your other agents:
- **Let Pinchy manage your other agents**: off by default. While it is off he does not look at them at all.
- **When one of them asks for permission**: **Smart** (the rules above), **Ask me** (every request comes to you), or **Never answer** (he only watches and passes messages; each tool asks in its own window).
- **Open now**: every agent he sees, its state and last line, with **Manage** and a button to show its terminal.
- **On this computer**: each tool, whether it is installed, whether Pinchy is connected to it, and a **Connect** / **Disconnect** button with one line on what he can do with that tool.

## Limits
- **Claude Code** and **opencode**: everything above.
- **Cursor**: he answers its shell and connector questions with Allow or Refuse and sees when it starts and ends. A message reaches it when it stops in its own window; a one-off `cursor-agent -p` run cannot be reached.
- **pi** never asks permission itself, so Pinchy only stops the things on his never-list there; he sees what it is doing and can send it messages, even when it is idle.
- **Hermes** keeps asking its own dangerous-command questions (Pinchy shows you when one waits); he stops the never-list and passes messages at its next turn. Connect also switches Pinchy's plugin on in Hermes.
- pi and Hermes were tested against their plugin interfaces, not with a full model run on our side.
- An agent that is open but whose tool is not connected shows with a green ring only: Pinchy sees it but cannot answer it or send it messages.
- On Windows the Cursor hook and `pinchy-say` run through Pinchy's own program; Claude Code's hooks need `curl`, which comes with Git Bash.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
