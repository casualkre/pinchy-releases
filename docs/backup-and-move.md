---
title: "Backup and moving to a new computer"
description: "You can save all of Pinchy into one file and bring him back from it, on this computer or a new one. You can also keep encrypted backups in your own cloud storage."
keywords: "backup, back up, restore, move, new computer, migrate, export, import, cloud backup, bucket, S3"
permalink: /backup-and-move/
---
# Backup and moving to a new computer

You can save all of Pinchy into one file and bring him back from it, on this computer or a new one. You can also keep encrypted backups in your own cloud storage.

## What to ask for
- "Make a backup of yourself." He saves one file and tells you where it is.
- "I got a new laptop, how do I take you with me?" He explains the two steps: save a backup here, restore it there.
- "Back yourself up to my cloud storage now." He starts an encrypted backup into your own bucket and tells you when it is done.
- "When was your last backup?" He tells you when the last cloud backup ran and whether it worked.

## What is in a backup
- His memory (the second brain), skills, extensions, artifacts, tasks and agents, variables and settings.
- Not in it: passwords and other secrets. You sign in and reconnect accounts again after a restore.
- Never restored: what you allowed on a computer (remembered permissions, full autonomy, extension rights, paired phones, chat apps). You switch those on again yourself.
- Restoring a backup FILE also leaves this computer's set-up as it is: the away server, connectors, where results are sent, cloud storage, folders and spending caps. A backup someone hands you can then not connect you to their server or run their commands. Your own cloud backup does bring your set-up along.

## How it works
- A backup is one file you can copy anywhere.
- Cloud backups are encrypted on your computer, with a recovery key, before they are uploaded. How often they run is set in the Cloud storage window. The bucket is yours: Backblaze B2, Cloudflare R2, Oracle Cloud, Amazon S3 or any S3-compatible storage. Pinchy has no server of his own that sees your files.
- The working files of swarms (big outputs, videos) are left out of backups above a size cap, so a backup stays small.

## Settings
- Settings → Safety & data → Backup & move: save Pinchy into one file, restore from a file.
- Settings → Safety & data → Backup & move → Open Cloud storage: connect your bucket, back up now, see and restore earlier backups. Cloud storage can also sit in his right-click menu (Customize → Add).

## Limits
- Restoring is done by you in Settings, not by Pinchy in a chat. A restore replaces what is on this computer with what is in the backup.
- Without the recovery key nobody can open a cloud backup, including you. The Cloud storage window shows the key; keep a copy somewhere safe.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
