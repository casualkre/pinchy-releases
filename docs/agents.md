---
title: "Agents: coworkers with a standing job"
description: "An agent is a coworker you give a job to once. It works on its own, on a schedule or when something happens, and writes to you only when it is done, has an update, or needs your help or approval. You do not manage it step by step."
keywords: "agent, agents, coworker, command, commands, custom command, slash command, scheduled task, routine, reminder, automation, every morning, every day, watch, monitor, keep an eye, heartbeat, background, standing job, recurring, attach, file, files, folder, zip, download, preview, description, colleagues, message between agents, sub-swarm, helper, stop job, needs you, mark done, dismiss, computer, vm, screen mouse keyboard, take control, move agent, delete agent, specialists"
permalink: /agents/
---
# Agents: coworkers with a standing job

An agent is a coworker you give a job to once. It works on its own, on a schedule or when something happens, and writes to you only when it is done, has an update, or needs your help or approval. You do not manage it step by step.

## What to ask for
- "Every morning at 8, send me five lines on what changed and what needs me." A morning brief, delivered where you want it.
- "Translate every new document that lands in this folder, and check each page before you give it to me." A translator that proofreads itself.
- "Keep my project moving: every evening, do the next thing on the list and tell me what you did." A project coworker.
- "Tell me when this page changes, and what the change means for me." A watcher with judgement.
- "Remind me in ten minutes to call Ada." A one-off reminder, the smallest kind of agent: it costs nothing to run.
- "What are my agents doing?" He lists them, their last runs and anything waiting for you.
- In an agent's chat: "Here are the three invoices, put the totals in a sheet." Attach the files and it works on them.
- In an agent's chat: "Move the news agent to the away server" or "Delete the old copy of Scout." It does it for you.

## How it works
- You describe the job in a chat, or pick an example card in the Agents window and fill in its fields. He shows you the agent and asks before it starts.
- An agent wakes on a schedule, or on a wake-up that costs nothing to check: a file or folder changed, a website value, a new email, a calendar entry, a variable.
- It keeps its own memory in its own folder, so it remembers what it did last time.
- Results go where you choose: a notification, a note on the desktop, the phone app, Telegram, email, or a saved place such as a Discord channel.
- "Keep an eye on…" requests with nothing to do on a schedule go on the heartbeat list: a small, cheap model checks the list regularly and wakes the big one only when something is worth acting on.
- With an away server, your agents keep running while this computer is off.
- There are no separate "scheduled tasks" any more: a task is an agent with a time or a wake-up. The tasks you had before were turned into agents the first time this version started, with the same words, times and way of telling you; a copy of the old list is kept.
- An agent can have conditions: only on certain days, only while you are away from the computer or only while you are at it, not on battery, only while a variable says so. If a condition (or a broken wake-up) keeps an agent from running, he tells you once, with the reason, instead of skipping silently.
- An agent made from a task without a time (a folder watch, or one you started by hand) runs only when its wake-up fires or you start it.
- When you write to an agent, it reads your message right away, even if it was asleep. Resume on one agent runs it now, even in its quiet hours; un-pausing Pinchy wakes your agents at their normal times.

### Files in its chat
- Attach any file, a whole folder or a .zip with the paperclip in its chat ("Attach files or a folder (or drop them here)"), or drop them on the message box. They are copied into the agent's own folder, so it can open them with its own tools; this works for agents on the away server too.
- The files an agent makes show as tiles under its message: Preview, Download, Show in folder and Save to cloud. A file of an agent on the away server is fetched to this computer the first time you open it.
- An agent can also send files to another agent with a message, from its own folder or the folder it works in (never hidden files, keys or Pinchy's own data).
- Pinchy can pass files on too: in your chat with him, "send this PDF to Scout" — he hands the agent your attachment (or a file he made) with his message, on this computer or the away server. Hidden files, key folders and Pinchy's own data never go.

### Its own commands
- An agent can have commands: instructions saved under a short name, such as /weekly. Type "/weekly" in its chat and it does what the command says. Anything you type after the name goes where the instruction says {{text}}, or at the end if it has none.
- You make them on the agent's page, under **Commands**: the **+** button, a name, a few words on what it does and the instruction. Click a command to read it in full, **Edit** it or **Delete** it. In its chat, typing "/" lists its commands.
- The agent can make commands for itself when it notices a job it does again and again. Each command says who made it: "made by you", "made by him" (the agent) or "set by Pinchy". The agent can use yours but never change or delete them; you can change or delete any of them.
- When you run a command the agent wrote, it is told the instruction is its own text, not your words. An agent never makes or changes a command in a round where it read a web page or a message from someone else.

### Agents know each other
- Every agent has a description: what it does and what the others may send it. You write it in the agent's form ("What the other agents read about him"); leave it empty and the agent writes one itself, and keeps it up to date. It shows on the agent's info panel with its id.
- Each agent sees its colleagues by name, id, where they run and their description, so it knows whom to send work to.
- Agents write to each other with no length limit; a very long message is saved as a file in the receiver's folder and its chat shows the start and the file.

### Jobs it starts
- An agent can hand a big job to Pinchy's engines: a Code or Work run, deep research, a code review, or a whole swarm (a sub-swarm runs as a hive like any other swarm), and it can start helpers that work in the background while it goes on.
- Everything it started shows live above its chat under "Working for him": what each job is doing, what it has spent of its limit, and anything that waits for you first. **Open** opens the run or the swarm's board, **Tell** passes a line to a job while it works, **Stop** stops it. The agent hears what you did in its next round. When nothing is running, the strip folds to one line ("His jobs").
- A swarm it starts belongs to it: when the crew has a question, the agent answers what its job and notes settle and sends you only what it cannot decide. When the job is finished the agent gets the real files and a plain statement of what is still open, so it can check the work before it tells you.

### Its own computer, and yours
- Every agent has its own computer, on by default: on the away server that is the server's own desktop ("His screen, mouse and keyboard"), on this computer it is Pinchy's VM ("His own computer (a VM): screen, mouse and keyboard"). It shows beside its chat, and you can take control.
- **Your** screen, mouse and keyboard is a separate box, "Your screen, mouse and keyboard", only while you are away. It is off unless you tick it.
- An agent can also make calls to this computer while it is switched on: run a command, read or write a file, look in a folder. Each call asks you first with **Allow once**, **Always** (for that kind of call, for that agent) or **No**, on the desktop, the phone or Telegram. Calls from the away server can be allowed "Always" only for reading and looking in folders.

### When it needs you
- When an agent needs you, it asks: a question, a step only a person can do on its screen (a captcha, a sign-in), or an OK before something risky (a command, root on the away server, a call to this computer).
- Clicking a "needs you" item, or **See it** on its notification, opens that item's own card: what it is, which agent, when, and its buttons. You answer there, in its chat, on the phone or in Telegram.
- **Mark done** on any card: you do not need to answer it, and the agent is told and carries on without it. The agent can close something it asked too, once it no longer needs you; it then disappears everywhere you saw it.

### Agents managing agents
- In an agent's chat you can ask it to move one of your other agents (to the away server or back to this computer), create one, or delete one. With full autonomy it does it at once when your message names the agent; otherwise you get one Yes/No. It never acts on another agent's message or a web page, and never on itself or the agent that created it.
- A delete made by an agent keeps a copy for 7 days: the chat line "Deleted …" has **Undo**, which brings the agent back paused.

### Specialists on an agent
- A specialist (for example a fact checker) reads along while an agent works and leaves it notes. In the agent's form, under "Specialists watching him", tick one for this agent only; a specialist set to watch every agent is shown there already. "Open Specialists" opens the Specialists window to make one or change what it watches.

## Settings
- Settings → Agents & automation → Agents: Open Agents, let agents run, let Pinchy create agents when you ask, how many helpers an agent may make, how many agents at most and at the same time, how often a scheduled agent may run, the older "Pause watches and routines" switch.
- Settings → Agents & automation → Away server: the machine that keeps them working while this computer is off, with root approvals for agents there.
- Settings → Pinchy → Notifications: where results are sent (under "Results from agents"): your email, quiet hours, saved places.
- Settings → Agents & automation → Heartbeat: the list he keeps an eye on, how often it is checked, how often the big model may be woken.
- Settings → Agents & automation → Variables: live values agents can react to without using your plan.
- Settings → Agents & automation → Telegram & chat apps and Settings → Agents & automation → Phone: reach and answer your agents away from the desk.
- Settings → Workspace → Specialists: the watchers that read along.
- Per agent, in its form in the Agents window: its description, what it may use (its own computer, your screen, mouse and keyboard, browser, wallet …), how free it is, and its specialists.

## Limits
- Every scheduled run is a Claude round and uses your plan. A run every minute uses it fast; wake-ups are checked without Claude.
- What an agent may do without asking is set per agent. Sending, deleting, paying and admin commands ask you first unless you allowed them for that agent.
- A swarm or job an agent starts spends from that agent's daily budget, and never more than your cost cap per swarm. Putting a result into a git project (Apply), raising a limit and permissions are always your decision, never the agent's.
- While this computer is off, agents run only if you set up an away server; calls to this computer wait until it is on.
- An agent made by another agent never gets more than its creator: the same switches, rules and budget (at most the creator's), and no helpers of its own unless you give it some.

## Creatures: five kinds of agent

When you create an agent you pick what **kind** it is. Every kind is a whole agent: each one can plan, go on by itself, hand big jobs to Code, Work or a swarm, start helpers and use every tool you allow. A kind adds what it is best at and starts from different defaults — nothing is taken away, and whatever you set yourself on the agent wins. If you are unsure, pick the lobster; every agent you already have is one.

| Creature | Best at | What it adds or starts from |
|---|---|---|
| **Lobster** | Anything — the all-rounder. | Plans its work, shows the plan, asks when it must. |
| **Shrimp** | Quick questions and small jobs. | Starts every round on the light model and in a fresh, short conversation, so answers come fast and use little. Give it a model or an effort of its own and it uses that. |
| **Pistol shrimp** | Waiting for something, then acting at once. | While it waits for its watch it costs nothing; when the watch fires it acts at once. A hit always reaches you, a false alarm stays quiet (it is in its chat, without a notification), and it keeps score of how often each watch fired and how often that mattered — a watch that keeps firing for nothing is narrowed by the shrimp itself, and named to you if that does not help. Firings close together count as one: three minutes between two strikes by default; ask Pinchy for another gap, or none. |
| **Mantis shrimp** | Things that must be right. | Thinks harder (high effort on every round), and under each result you see what it really looked at — files, pages, screens — recorded by Pinchy, not claimed by the agent. A result with nothing opened behind it is sent back to look, once, before you get it. The second reader is on by default; tell Pinchy to switch it off for an agent and it is off (that also switches the look-again off). |
| **Crayfish** | Long digging in the background. | Rounds of up to 90 minutes in one kept conversation, an extra round each day just to tidy its notes and memory, and each new day starts from what it did and planned yesterday. |

You can change an agent's creature at any time: ask Pinchy ("make the news agent a pistol shrimp") or change it in Agents.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
