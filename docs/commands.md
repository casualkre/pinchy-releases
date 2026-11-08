---
title: "Chat commands: things you type with a /"
description: "Type `/` in the chat box and a list of commands opens. A command does one thing at once, without asking Pinchy to think about it, and many borrow their names from Claude Code. They work the same in the chat on your computer, in the phone app and in Telegram."
keywords: "commands, slash, slash commands, /goal, goal, keep going, keep working until, /btw, side question, /status, /usage, cost, /plan, /loop, /schedule, /remember, /memory, /export, /ask, /call, /voice, /copy, /doctor, /model, /effort, /new, /clear, /stop, /stopall, /jobs, /swarm, /krill, /research, /style, /theme, my own commands, shortcut"
permalink: /commands/
---
# Chat commands: things you type with a /

Type `/` in the chat box and a list of commands opens. A command does one thing at once, without asking Pinchy to think about it, and many borrow their names from Claude Code. They work the same in the chat on your computer, in the phone app and in Telegram.

## What to ask for
- `/goal all tests in ~/proj pass` Pinchy keeps working, turn after turn, until it is true. After each answer a small model checks whether the goal holds; if not, he gets one more round with what is still missing.
- `/btw what was that library called?` A quick side question. He answers from the chat so far without stopping what he is doing.
- `/plan move my notes to Obsidian` He writes the plan first (as a Reef document) and does nothing until you say go.
- `/loop 30m check my inbox for invoices` Runs something again and again. `/schedule 18:30 call the plumber` or `/schedule in 20m …` runs it once, later.
- `/ask Scout what did you find?` Sends one of your agents a note. Its answer comes back to you in the chat.
- `/status` What he is on right now: model, goal, running krill, busy agents, what waits for you.

## All the commands
- **Work:** `/goal`, `/plan`, `/krill`, `/research`, `/swarm`, `/jobs` (what is running), `/stop` (stop his answer; also pauses a goal), `/stopall` (stop every agent run), `/loop`, `/schedule`.
- **The chat:** `/new` or `/clear` (fresh chat), `/chats` (reopen an earlier one), `/btw`, `/export` (this chat as a Reef document), `/copy` (his last answer), `/model`, `/effort`, `/usage` (cost and how much is left).
- **Memory:** `/remember <fact>`, `/memory <words>`, `/recap`.
- **People and helpers:** `/agents`, `/ask <agent> <message>`, `/call [agent]` (rings your phone).
- **Pinchy himself:** `/voice on|off` (the Humotranslator reads his replies), `/theme`, `/style` (the whole look), `/focus`, `/pause`, `/resume`, `/undo`, `/doctor`.
- **Windows:** `/reef`, `/browser [address]`, `/vault`, `/review`.
- `/help` lists the ones that work right now: a command whose feature is switched off or not installed is left out.

## How /goal works
- `/goal <what should be true>` starts it. A chip over the chat box shows the round ("Goal · round 3/25"); ✕ drops it.
- He stops by himself when it is met ("Goal met after N rounds", with the reason), after 25 rounds, when he asks you something (it waits for your answer), on `/stop`, when a turn fails, or while he is paused.
- `/goal` shows where it is, `/goal clear` drops it, `/goal resume` carries on after it stopped.
- The check reads only his last answer. Write the goal so his answer can show it: "the file X exists and has 3 lines" works better than "do a good job".

## Your own commands
- Make one in Settings, or ask him: "make a /standup command that sums up my calendar for today". Anything typed after the name goes where the command says `{{text}}`.
- Agents have their own commands too, on each agent's page.

## Settings
- Settings → Brain → Commands: your own commands (make, edit, delete) and the built-in list.

## Limits
- Only your own words run commands: what you type in the chat, on the phone, in your paired chat app, or say out loud. A `/…` line inside a note, a web page or an agent's message is just text to him.
- `/compact` (shrink the chat's memory) is not there yet.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
