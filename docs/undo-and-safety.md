---
title: "Undo, pause and permissions"
description: "You stay in charge of what Pinchy does on your computer. You can pause him at once, see everything he changed and undo it, and decide what he may do without asking."
keywords: "undo, revert, history, timeline, what did you do, pause, stop, stop for a while, stop doing anything, panic, permission, approve, allow, safety, activity log"
permalink: /undo-and-safety/
---
# Undo, pause and permissions

You stay in charge of what Pinchy does on your computer. You can pause him at once, see everything he changed and undo it, and decide what he may do without asking.

## What to ask for
- "What did you change today?" He lists the files he edited or created and the commands he ran.
- "Undo that." or "Put my file back." He restores the file as it was before he changed it.
- "Stop." or the panic shortcut: he stops and stays paused until you unpause him.
- "Ask me before you run commands." He changes how much he may do without asking.

## How it works
- Pause: while paused, Pinchy and his tasks cannot act on your computer, and waiting permission requests are denied. The panic shortcut pauses him from anywhere.
- Permissions: before something that cannot be taken back (deleting, sending, buying, system settings) he asks, and the app shows a dialog. An unanswered request is denied after two minutes. "Always allow" answers are remembered and you can remove them.
- Admin commands: for a command that needs root he shows a password dialog that only you answer. He never types your password.
- Undo: with the timeline on, a copy of every file is kept on this computer before he changes it. The timeline window lists each step with an Undo button.
- The activity log records what he did, including what was auto-approved.

## Settings
- Settings → Pinchy → General: Pause Pinchy, and the panic shortcut.
- Settings → Brain → Claude: how much he may do without asking (the permission mode).
- Settings → Safety & data → Safety: the note for auto-approved actions, how long a request waits, remembered permissions, the activity log.
- Settings → Safety & data → Undo & history: keep a timeline with Undo (off by default), how many days and how much space copies may use, and "Open the timeline".
- Settings → Safety & data → Check everything: one button that tests Claude, the microphone, shortcuts, screenshots and clicks, with a fix for anything that does not work.

## Limits
- The timeline is off until you turn it on, and it covers chats started after that.
- Undo restores files. It cannot unsend a message or undo something done on a website.
- Copies are removed after 7 days or when they use more than 200 MB (both can be changed); those steps can then no longer be undone.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
