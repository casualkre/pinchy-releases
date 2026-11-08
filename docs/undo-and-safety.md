---
title: "Undo, pause and permissions"
description: "You stay in charge of what Pinchy, your agents and krill do on your computer. You can pause him at once, see everything any of them changed and undo it, and decide what he may do without asking."
keywords: "undo, revert, history, timeline, what happened, what did you do, what did my agent do, krill changed, put it back, undo the agent, pause, stop, stop for a while, stop doing anything, panic, permission, approve, allow, safety, activity log"
permalink: /undo-and-safety/
---
# Undo, pause and permissions

You stay in charge of what Pinchy, your agents and krill do on your computer. You can pause him at once, see everything any of them changed and undo it, and decide what he may do without asking.

## What to ask for
- "What did you change today?" or "What did my agents do this morning?" He reads the one timeline: files, settings, space items and agent changes, by Pinchy, agents, krill and you.
- "Undo that." or "Put my file back." He restores it as it was before the change.
- "Scout broke my shopping list, put it back." He finds that step in the timeline and undoes it. Because it is someone else's change, he asks you first.
- "Stop." or the panic shortcut: he stops and stays paused until you unpause him.
- "Ask me before you run commands." He changes how much he may do without asking.

## How it works
- Pause: while paused, Pinchy and his tasks cannot act on your computer, and waiting permission requests are denied. The panic shortcut pauses him from anywhere.
- Permissions: before something that cannot be taken back (deleting, sending, buying, system settings) he asks, and the app shows a dialog. An unanswered request is denied after two minutes. "Always allow" answers are remembered and you can remove them.
- Admin commands: for a command that needs root he shows a password dialog that only you answer. He never types your password.
- Admin commands on your away server: once root approvals are on, every root command there waits for your Allow or Refuse — from this computer, your phone or Telegram — at any autonomy level. It runs exactly the command you were shown, and only after your Allow. See the page "Away server".
- Your screen, mouse and keyboard: an agent may use them only if you ticked that for the agent. Its own computer (Pinchy's VM, or the away server's desktop) is a different box and is on by default.
- **What happened** (the timeline, on the computer and the phone): one list of every change — files, settings, space items and agents — by Pinchy, your agents (here and on your away server), krill and you, newest first, with who did it and an **Undo** button where there is one. Open it from his menu or the tray, or on your phone (open its Settings and tap "What happened").
- Undo of files: a copy of a file is kept on this computer before it changes (on by default). This works for every engine: Claude Code, and krill on Cursor, Codex, opencode, pi or a local model.
- Undo of settings, space items and agents: always there; a space item comes back as a new version, so nothing is lost.
- Who may undo: you can undo anything. An agent or krill can undo its own step; undoing anyone else's step asks you first, saying who wants to undo what and why. On your away server nobody can undo someone else's step without you: you do it from this computer or your phone.
- The activity log records what he did, including what was auto-approved.
- **Actual full autonomy on everything** (Settings → Experimental, off by default, only switched on in this Settings window): while it is on, nothing above asks you — no permission dialogs for Pinchy, his agents (here and on your away server), swarms or add-ons, and root commands on the away server run without your Allow while this computer is on (it approves them for you; while it is off they wait for your phone). Two things stay: the password dialog for admin commands on this computer, and a short list that is always refused (wiping the system or your home folder, formatting a disk, and turning his own permissions up). Pause and the agents' kill switch still stop everything, and the activity log still records it all.

## Settings
- Settings → Pinchy → General: Pause Pinchy, and the panic shortcut.
- Settings → Brain → Chat: how much he may do without asking (the permission mode).
- Settings → Safety & data → Safety: the note for auto-approved actions, how long a request waits, remembered permissions, the activity log.
- Settings → Safety & data → Undo & history: keep copies so file changes can be undone (on by default), how many days and how much space copies may use, and "Open the timeline".
- Settings → Safety & data → Check everything: one button that tests Claude, the microphone, shortcuts, screenshots and clicks, with a fix for anything that does not work.
- "Pinchy froze" in Check everything: how often Pinchy froze or its background work got stuck in the last 24 hours, the longest one, when, and what was running then. Short pauses under 3 seconds are not counted.

## Limits
- If you switch copies off, settings, space items and agents can still be undone, files cannot.
- A krill that works in your whole home folder gets no file copies (too many files to copy each turn).
- A space item changed outside Pinchy (a tool rewriting its file directly) shows the change but has no Undo step.
- Undo cannot unsend a message or undo something done on a website.
- Copies are removed after 7 days or when they use more than 200 MB (both can be changed); those steps can then no longer be undone.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
