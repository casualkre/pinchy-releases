---
title: "Backup and moving"
description: "You can save all of Pinchy into one file and bring him back from it, on this computer or a new one. With a Lobster Network profile he can also keep his own backups in your account: 10 GB that is yours alone, locked on this computer before anything leaves."
keywords: "backup, back up, restore, move, new computer, migrate, export, import, backups, lobster network backup, 10 GB, recovery code, encrypted, vault backup, spaces backup, cloud storage, bucket, Backblaze, R2, S3, where did cloud storage go, from cloud storage"
permalink: /backup-and-move/
---
# Backup and moving

You can save all of Pinchy into one file and bring him back from it, on this computer or a new one. With a Lobster Network profile he can also keep his own backups in your account: 10 GB that is yours alone, locked on this computer before anything leaves.

## What to ask for
- "Make a backup of yourself." He saves one file and tells you where it is.
- "I got a new laptop, how do I take you with me?" He explains it: sign in to the Lobster Network there with your recovery code, then open Backups and restore.
- "Back yourself up now." He starts a backup into your account and tells you when it is done.
- "When was your last backup?" He says when the last one ran and whether it worked.
- "Where did Cloud storage go?" It is gone since 2.7.5. Your bucket is still there and still yours; what Pinchy kept in it was copied to this computer (see below).

## Backups in your Lobster Network account
- Open Backups from his right-click menu, or ask him. You need a Lobster Network profile; it is free.
- Every account gets 10 GB for its own backups (2 GB in a new account's first week). That is apart from what you publish, which keeps its own limits.
- What goes in: his memory (the second brain), skills, extensions, agents, tasks, variables and settings, and your chats unless you switch them off. Your Spaces go up as their own backup.
- Your vault only if you turn it on (Backups → Your vault too). It goes up still locked by your vault passphrase, then locked again.
- Daily or weekly, while this computer is on. The last 4 of each kind are kept: Pinchy, Spaces and Vault are counted apart.
- Off until you turn it on. If you had Cloud storage backups on, they carry on here by themselves after the move.

## Who can read them
- Nobody but you. Every backup is locked on this computer before it leaves, with a key that comes from your Lobster Network account. The network gets locked bytes: not your files, not their names, not which computer they came from.
- That key comes from your account's recovery code, so the same code is what opens your backups on a new computer. It never leaves your computers. Without it nobody can open them, and nobody can give it back to you.
- The network does see that you have backups, of which kind (Pinchy, Spaces or Vault), how big they are and when they were made.
- A backup changed on the network, or swapped, cut short or put together from two others, does not restore: it says so and leaves nothing half done.
- The network could hold back your newest backup or show an older one. Pinchy can't prove from the outside that the list is the newest; look at the dates.

## Restoring
- Backups → a row → Restore asks first, in place. Only you can do it, in that window. Not Pinchy in a chat, not an agent, not your phone.
- A Pinchy backup puts his memory, skills, agents and settings back as they were then. What is here now is kept next to it.
- A Spaces backup brings back the spaces and items you no longer have. Anything you still have stays as it is.
- A Vault backup is only put back on a computer without a vault, so it can never undo changes you made since. On a new computer the vault opens with its own recovery code, because that computer's keyring is not the one it was locked with.

## Moving off Cloud storage (2.7.5)
- Cloud storage is gone from Pinchy. Pinchy never deletes or changes anything in your bucket: not in the move, not ever.
- Backups → Moving off Cloud storage → Copy brings what Pinchy kept there to this computer, into Pinchy / From Cloud storage in your home folder. From then on that folder is in your backups.
- Your old encrypted backups stay in your bucket, as does anything outside Pinchy's folder there. Delete the bucket yourself when you no longer want it.
- If the copy stops (no connection, a locked keyring), what came over stays and Copy again picks up where it was.

## A backup file
- Settings → Safety & data → Backup & move: save Pinchy into one file, restore from a file. You can copy that file anywhere.
- Not in it: passwords and other secrets. You sign in and reconnect accounts again after a restore.
- Never restored: what you allowed on a computer (remembered permissions, full autonomy, extension rights, paired phones, chat apps). You switch those on again yourself.
- Restoring a file someone hands you leaves this computer's set-up as it is (away server, connectors, where results are sent, folders, spending caps), so it can't connect you to their server or run their commands.
- Left out so a backup stays small and always finishes: a krill's copy of your project and its scratch files, node_modules and Python environments that agents made, big swarm outputs above a size cap, and anything a link inside Pinchy's folders points to.

## Settings
- Backups (right-click menu, or ask him): on or off, how often, chats, the vault, the list, restore, the move off Cloud storage.
- Settings → Safety & data → Backup & move: a backup file.
- Lobster Network → You: your recovery code.

## Limits
- 10 GB per account. When the network itself is short of space, a backup is refused before anything is sent, with a sentence that says so; nothing half-made is kept.
- A restore is yours, on this computer, never a chat's or an agent's.
- On the phone you can see when the last backup ran; turning backups on or off, backing up now and restoring are done on the computer.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
