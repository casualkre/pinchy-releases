---
title: "Second brain: what Pinchy remembers"
description: "Pinchy's memory is a plain folder of markdown files on your computer, called his second brain. He reads a short part of it at the start of every chat and looks the rest up when a question needs it. You can open, read and edit every file yourself."
keywords: "memory, remember, forget, notes, brain folder, USER.md, AGENTS.md, journal, recap, second brain, saved work, project notes, finished jobs, what did the agent find"
permalink: /second-brain/
---
# Second brain: what Pinchy remembers

Pinchy's memory is a plain folder of markdown files on your computer, called his second brain. He reads a short part of it at the start of every chat and looks the rest up when a question needs it. You can open, read and edit every file yourself.

## What to ask for
- "Remember that my sister's birthday is 14 March." He writes a note and adds it to his index.
- "From now on, always answer in British English." He writes it into his standing instructions.
- "What did we decide about the Plantpal database?" He searches his notes and past chats.
- "What do you know about me?" He reads it back from USER.md.
- "Forget what I told you about my old job." He finds the note and removes it (and says what he removed).
- "What did the swarm build for the Acme report last week?" He looks it up in the note he keeps for that project.

## What is in the folder
- `USER.md`: who you are and what you like. Read at the start of every chat.
- `AGENTS.md`: your standing instructions for him. Read at the start of every chat.
- `MEMORY.md`: the index, one line per note. The notes themselves are in `notes/` (by topic: people, projects, howto, decisions).
- `IMPULSIVE.md`: the key points of your last few chats, so a new chat is not confused.
- `PLACES.md`: folders and files he learned where to find.
- `journal/`: one file per day with what was talked about and done.
- `notes/projects/`, `notes/agents/`, `notes/research/`: what finished jobs found out, one note per project, per agent and per research question (see the next section).
- `CAPTURED.md`: the list of what was saved from finished jobs, newest last.

## Saving finished work
- When a Work or Code job, a swarm, an agent run or a deep research finishes, Pinchy files its own summary in the brain: what was made, where the files are, what is still open.
- Few notes that grow, not one note per job: everything done in one project folder goes into that project's note with the newest entry first, an agent's results go into that agent's note, a research answer into a note named after the question.
- The same job finishing again replaces its entry. A run that found nothing new is not saved.
- These notes are not read at the start of a chat. He finds them when he looks something up, so they cost nothing until they are needed.
- A line that looks like a password or a key is left out, and the entry says so.
- Each entry is marked as saved from a finished job: it is information he can read, not instructions to follow.

## How it works
- A small model looks at the chat every few messages and notes what is worth keeping. When it saves something you see a small "Noted" message with Undo.
- When you tell him to remember something, he saves it in the same turn.
- Before answering a question that may have come up before, he searches his notes; when the notes have little on it, the search also brings back matching lines from past chats.
- Claude Code keeps its own notes for a folder you also use with Claude Code. Those are not Pinchy's memory and are never loaded into his chats. When his own notes have nothing on a question, his search also looks there and tells him whose notes they are.

## Settings
- Settings → Brain → Memory: switch memory on or off, pick the brain folder (any visible folder works, for example `~/Pinchy Brain`), how often he updates his notes, the "Noted" message, recent chats, the daily recap, and how much memory is read at the start of a chat.
- Settings → Brain → Memory → Saving finished work: one switch for all of it ("Save what finished jobs found out"), and one each for Work jobs, Code jobs, Swarms, Agent results and Research.
- Settings → Brain → Memory → Open brain folder: opens the folder in your file manager.
- Settings → Brain → Instructions: your standing instructions (the same text as AGENTS.md).
- Settings → Safety & data → Backup & move: save the whole brain (with skills, tasks and settings) into one file.

## Limits
- Passwords and other secrets do not belong in notes. His own accounts are kept in a separate `secrets` folder inside the brain.
- Only a capped part of the brain is read at the start of a chat (12,000 characters by default). Everything else is found by searching, so long notes cost nothing until they are needed.
- An agent keeps its own memory in its own folder inside the brain; it does not write into the main Pinchy's notes. What an agent REPORTS when a run ends is saved under `notes/agents/` by Pinchy, not by the agent.
- At most 40 finished jobs are saved per day, and a project's note keeps its newest 30 entries.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
