---
title: "Backup, moving and cloud storage"
description: "You can save all of Pinchy into one file and bring him back from it, on this computer or a new one. You can also connect your own cloud storage: keep encrypted backups there, drop files and folders into it, and let Pinchy and your agents save their work there."
keywords: "backup, back up, restore, move, new computer, migrate, export, import, cloud backup, bucket, S3, cloud storage, upload, drag and drop, save to cloud, share link, Backblaze, R2, away server, keep what pinchy makes, made by pinchy, keep copies, automatic copy"
permalink: /backup-and-move/
---
# Backup, moving and cloud storage

You can save all of Pinchy into one file and bring him back from it, on this computer or a new one. You can also connect your own cloud storage: keep encrypted backups there, drop files and folders into it, and let Pinchy and your agents save their work there.

## What to ask for
- "Make a backup of yourself." He saves one file and tells you where it is.
- "I got a new laptop, how do I take you with me?" He explains the two steps: save a backup here, restore it there.
- "Back yourself up to my cloud storage now." He starts an encrypted backup into your own bucket and tells you when it is done.
- "When was your last backup?" He tells you when the last cloud backup ran and whether it worked.
- "Would my backup really come back?" He looks at the last weekly check (see below), or runs one now when you press Check it in Cloud storage → Backups.
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
- Cloud backups only send what changed. A backup is cut into pieces of about 2 MB; a piece your bucket already holds is not sent again. The first backup uploads everything; after that a backup with little changed sends a few pieces instead of the whole thing (on a real Pinchy: 2 pieces of 176). Each piece is locked with your recovery key before it leaves, and its name tells the bucket nothing about what is inside. Pieces no backup uses any more are removed a day later. Backups made before 2.6.5 (one big file each) still restore.
- While a backup runs, the Backups card says what it is doing in numbers: which part it is gathering, how far the packing is, how much it is checking, how many new pieces it sends, and roughly how long is left. Afterwards it says how big the backup is and how much had to be sent, and "What went into the last backup" lists every part with its size and what stayed on this computer.
- Stop works at any moment of a backup, in the Cloud storage window or on the phone: one press, the card says Stopping…, and nothing half-made is kept. A restore can be stopped while it downloads and unlocks, never while it is putting your files back.
- If your bucket is full (a storage cap), the backup removes this computer's oldest backups to make room and tries once more. It never removes this computer's newest backup or another computer's backups; if there is still no room, it says so with your provider's words.
- The working files of swarms (big outputs, videos) are left out of backups above a size cap, so a backup stays small.
- Left out on purpose, so a backup stays small and always finishes: a Work or Code run's own copy of your project and its scratch files (the project itself lives elsewhere), node_modules and Python virtual environments made by agents, runs or swarms (they are rebuilt, not kept), and anything a link inside Pinchy's folders points to. A link is never followed: before 2.6.5 one folder linking back into itself made every backup fail after about 45 minutes. An extension or skill that ships its own node_modules keeps it.
- If a scheduled cloud backup fails, you get a notice with the reason your storage provider gave (for example a full account or a spending cap) and a button to open Cloud storage. It tries again later by itself. The same reason is told once, not every time it tries again.
- A backup that stopped working can't be missed: after 2 days without a good cloud backup, Settings → Safety & data → Check everything and the app's Home screen on your phone show "No good backup for N days" in amber; after 7 days it turns red and Pinchy says so once a day with a Back up now button. A backup you stopped yourself does not count as a failure.
- Once a week, right after a backup worked, Pinchy proves it would come back: he downloads it again, unlocks it with your recovery key and opens every part — nothing on this computer is changed. Each backup in Cloud storage → Backups then shows "Checked: restores OK" or why it would not open, and has a Check it button to do the same now. If the bucket or the internet says no, that counts as "could not check" and is tried again later, never as a broken backup.
- A backup whose name doesn't match what is inside it (a copy put there under another name) is marked on its row and can't be restored by that name.

## Cloud storage for your files
- Cloud storage is a place in the Workspace sidebar, under Projects and Artifacts. Drop files or whole folders anywhere on that page and they are saved into the folder you have open; folders keep their inside folders. Upload files / Upload a folder do the same through a file picker.
- From there you open folders, preview pictures and text files, download a file or a whole folder (into Downloads, never over an existing file) and copy a share link that works for 24 hours. The arrow button at the top opens the full Cloud storage window for renaming, deleting, backups and the connection.
- The Cloud storage window takes a drop on any of its pages too: it switches to Files and uploads there.
- Every file tile in Pinchy (in an agent's chat, in Work and Code chats) has Save to cloud next to Preview and Download. On the phone, a file's page has Save to cloud storage.
- Pinchy and every agent can save files and folders into your storage, list it and fetch files from it. Saving asks you first (Allow, or Allow always) unless the agent has full autonomy. Only you and Pinchy's own chat make share links; an agent cannot hand a file out to the world.
- Files that hold keys or passwords (.env, ssh keys, Pinchy's own data folder) are never uploaded by Pinchy or an agent. Inside a folder they are skipped, and he says how many he left out.
- Keep what Pinchy and agents make: one switch, off until you turn it on (Cloud storage window → Connection, or the Cloud storage place in the Workspace). When it is on, every file a chat, a Work job, a deep research or an agent hands you is also copied into your bucket under "Made by Pinchy", a folder per day and one per hand-over, so two reports with the same name never overwrite each other. Keys, passwords, hidden files and Pinchy's own data never go; a file bigger than 200 MB is left out; a job that failed copies nothing, and the same file is never copied twice. The line under the switch says how many it kept today, or why the last copy failed. Files a swarm hands you are not copied yet.

## Your away server and your bucket
- Off until you switch it on: Cloud storage window → Connection → Your away server can use it too. Pinchy then gives the server your bucket and keys, so agents on the server can save into your storage and fetch from it while this computer is off.
- The keys are stored on the server, outside what it shares back with this computer; agents there cannot read that file. Switching it off (or disconnecting the bucket, or changing keys) reaches the server as well.
- An away server from before 2.6 does not know this yet: the switch says so, and Update now on the away server page fixes it.

## Settings
- Settings → Safety & data → Backup & move: save Pinchy into one file, restore from a file.
- Settings → Safety & data → Backup & move → Open Cloud storage: connect your bucket, back up now, see and restore earlier backups. Cloud storage can also sit in his right-click menu (Customize → Add).
- Workspace → Cloud storage: your files in the bucket, drop to upload.
- Cloud storage window → Backups: on or off, daily or weekly, how many to keep. → Connection: test, change keys or bucket, disconnect, Your away server can use it too, and Keep what Pinchy and agents make (off unless you turn it on).

## Limits
- Restoring is done by you in Settings, not by Pinchy in a chat. A restore replaces what is on this computer with what is in the backup.
- Without the recovery key nobody can open a cloud backup, including you. The Cloud storage window shows the key; keep a copy somewhere safe.
- Pinchy only ever sees the folder you chose for him in the bucket, never the rest of it. His own folders there (pinchy-backups, pinchy-backup-pieces and pinchy-pool, the away server's lease) are managed by Pinchy only: Pinchy's chat and agents can't read, save into, rename or delete them, even by uploading a folder with the same name.
- One drop or upload takes up to 5000 files. A share link lasts a week at most.
- Cloud storage needs a bucket of your own (an S3-compatible account). Pinchy has no free storage of his own to offer.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
