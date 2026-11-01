---
title: "Storage: how much space Pinchy uses"
description: "Pinchy keeps his work on your computer: swarms with their working copies, krill, caches, the agents' computer (a VM disk) and his memory. The Storage page shows how much each of those takes and frees what is safe, and Pinchy tells you when your disk gets almost full."
keywords: "storage, disk, disk space, disk full, free space, free up space, clean up, tidy, cache, how much space, what takes space, old swarms, delete old runs, trash"
permalink: /storage/
---
# Storage: how much space Pinchy uses

Pinchy keeps his work on your computer: swarms with their working copies, krill, caches, the agents' computer (a VM disk) and his memory. The Storage page shows how much each of those takes and frees what is safe, and Pinchy tells you when your disk gets almost full.

## What to ask for
- "How much space do you use?" He reads it out by kind, biggest first.
- "What can I delete?" He tells you what is safe to free and opens the Storage page; he never deletes anything himself.
- "My disk is almost full." He shows what of his takes the space and what can go.

## How it works
- The Storage page (Settings → Safety & data → Storage): it lists swarms, krill and reviews, leftovers and caches, and what Pinchy keeps (the agents' VM disk, his browser's logins, speech models, files, agents, memory), each with its size.
- "Free … now" removes only copies Pinchy can always make again: browser caches (your logins stay), old update downloads, unfinished cloud backup files, and the scratch folder of a run that ended more than 3 days ago.
- A finished swarm or run goes only when you tick it and click twice, and it goes to the Trash, so you can still get it back. Empty the Trash to get that space.
- Anything still running or waiting for you (a swarm, a run, a backup, a swarm waiting for your plan to reset) is shown but can't be picked.
- When the disk under Pinchy's data has less than 5 GB (or 5 %) left, he tells you once a day what he can free, with a "Show me" button.

## Settings
- Settings → Safety & data → Storage: the page itself, "Measure again", and "Tell me when the disk is almost full" (on by default).

## Limits
- Pinchy can read these sizes but cannot remove anything: the Storage page is yours.
- The agents' VM disk, memory, skills and chats are never offered here; remove the VM in Settings → Computer.
- Only this computer: the away server's own disk is not shown.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
