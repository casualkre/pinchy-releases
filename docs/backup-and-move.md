---
title: "Backup, moving and cloud storage"
description: "You can save all of Pinchy into one file and bring him back from it, on this computer or a new one. You can also connect your own cloud storage: keep encrypted backups there, drop files and folders into it, and let Pinchy and your agents save their work there."
keywords: "backup, back up, restore, move, new computer, migrate, export, import, cloud backup, bucket, S3, cloud storage, upload, drag and drop, save to cloud, share link, Backblaze, R2, away server"
permalink: /backup-and-move/
---
# Backup, moving and cloud storage

You can save all of Pinchy into one file and bring him back from it, on this computer or a new one. You can also connect your own cloud storage: keep encrypted backups there, drop files and folders into it, and let Pinchy and your agents save their work there.

## What to ask for
- "Make a backup of yourself." He saves one file and tells you where it is.
- "I got a new laptop, how do I take you with me?" He explains the two steps: save a backup here, restore it there.
- "Back yourself up to my cloud storage now." He starts an encrypted backup into your own bucket and tells you when it is done.
- "When was your last backup?" He tells you when the last cloud backup ran and whether it worked.
- "Save the report to my cloud." He (or the agent you ask) puts the file or the whole folder into your cloud storage and tells you where it went.
- "What is in my cloud?" / "Get me invoice.pdf from my cloud." He lists a folder, or downloads the file into your Downloads folder.
- "Make a link to that file so I can send it." Pinchy makes a download link that runs out (a day unless you say otherwise, a week at most).

## What is in a backup
- His memory (the second brain), skills, extensions, artifacts, tasks and agents, variables and settings.
- Not in it: passwords and other secrets. You sign in and reconnect accounts again after a restore.
- Never restored: what you allowed on a computer (remembered permissions, full autonomy, extension rights, paired phones, chat apps). You switch those on again yourself.
- Restoring a backup FILE also leaves this computer's set-up as it is: the away server, connectors, where results are sent, cloud storage, folders and spending caps. A backup someone hands you can then not connect you to their server or run their commands. Your own cloud backup does bring your set-up along.

## How it works
- A backup is one file you can copy anywhere.
- Cloud backups are encrypted on your computer, with a recovery key, before they are uploaded. How often they run is set in the Cloud storage window. The bucket is yours: Backblaze B2, Cloudflare R2, Oracle Cloud, Amazon S3 or any S3-compatible storage. Pinchy has no server of his own that sees your files.
- The working files of swarms (big outputs, videos) are left out of backups above a size cap, so a backup stays small.
- If a scheduled cloud backup fails, you get a notice with the reason your storage provider gave (for example a full account or a spending cap) and a button to open Cloud storage. It tries again later by itself.

## Cloud storage for your files
- Cloud storage is a place in the Workspace sidebar, under Projects and Artifacts. Drop files or whole folders anywhere on that page and they are saved into the folder you have open; folders keep their inside folders. Upload files / Upload a folder do the same through a file picker.
- From there you open folders, preview pictures and text files, download a file or a whole folder (into Downloads, never over an existing file) and copy a share link that works for 24 hours. The arrow button at the top opens the full Cloud storage window for renaming, deleting, backups and the connection.
- The Cloud storage window takes a drop on any of its pages too: it switches to Files and uploads there.
- Every file tile in Pinchy (in an agent's chat, in Work and Code chats) has Save to cloud next to Preview and Download. On the phone, a file's page has Save to cloud storage.
- Pinchy and every agent can save files and folders into your storage, list it and fetch files from it. Saving asks you first (Allow, or Allow always) unless the agent has full autonomy. Only you and Pinchy's own chat make share links; an agent cannot hand a file out to the world.
- Files that hold keys or passwords (.env, ssh keys, Pinchy's own data folder) are never uploaded by Pinchy or an agent. Inside a folder they are skipped, and he says how many he left out.

## Your away server and your bucket
- Off until you switch it on: Cloud storage window → Connection → Your away server can use it too. Pinchy then gives the server your bucket and keys, so agents on the server can save into your storage and fetch from it while this computer is off.
- The keys are stored on the server, outside what it shares back with this computer; agents there cannot read that file. Switching it off (or disconnecting the bucket, or changing keys) reaches the server as well.
- An away server from before 2.6 does not know this yet: the switch says so, and Update now on the away server page fixes it.

## Settings
- Settings → Safety & data → Backup & move: save Pinchy into one file, restore from a file.
- Settings → Safety & data → Backup & move → Open Cloud storage: connect your bucket, back up now, see and restore earlier backups. Cloud storage can also sit in his right-click menu (Customize → Add).
- Workspace → Cloud storage: your files in the bucket, drop to upload.
- Cloud storage window → Backups: on or off, daily or weekly, how many to keep. → Connection: test, change keys or bucket, disconnect, and Your away server can use it too.

## Limits
- Restoring is done by you in Settings, not by Pinchy in a chat. A restore replaces what is on this computer with what is in the backup.
- Without the recovery key nobody can open a cloud backup, including you. The Cloud storage window shows the key; keep a copy somewhere safe.
- Pinchy only ever sees the folder you chose for him in the bucket, never the rest of it. His encrypted backups folder there is managed by Backups only: Pinchy and agents cannot change it.
- One drop or upload takes up to 5000 files. A share link lasts a week at most.
- Cloud storage needs a bucket of your own (an S3-compatible account). Pinchy has no free storage of his own to offer.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
