---
title: "Updates: getting a newer Pinchy"
description: "Pinchy updates himself. He checks for a new version a few times a day, tells you when there is one, and installs it when you say so. You do not download an installer again."
keywords: "update, upgrade, new version, latest version, release, roll back, rollback, auto update, what's new, update the away server, update the server, phone app update, new apk"
permalink: /updates/
---
# Updates: getting a newer Pinchy

Pinchy updates himself. He checks for a new version a few times a day, tells you when there is one, and installs it when you say so. You do not download an installer again.

## What to ask for
- "Is there a newer version of you?" He checks right now and tells you which version you have and which is the newest.
- "Update yourself." He downloads the new version and asks before he restarts.
- "What changed in this version?" He shows the release notes.
- "How do I go back to the version before?" He points you to the roll back button (he cannot roll himself back; that button is yours).

## How it works
- About every six hours he asks the download server which version is the newest. Nothing about you or your computer is sent.
- A new version is only accepted when it is signed with Pinchy's release key, so a tampered download is refused.
- By default he tells you and waits for your click. If you allow him to install by himself, he does it only when nothing is running and you have been away from the keyboard for five minutes, or when you quit Pinchy.
- An update never restarts Pinchy under a working swarm or agent. It waits until they are done.
- After an update he tells you what is new. The version before stays on your computer, so you can roll back.
- Your away server updates separately: Settings → Agents & automation → Away server → Update now, or switch on "Keep Pinchy there up to date" and it follows this computer by itself when it is idle. It also accepts only signed versions and goes back by itself if a new one does not start. Fixes for agents on the server only arrive there with its update.
- The phone app does not update itself: install the new APK from the release page (the download table at the top of each release).

## Settings
- Settings → Safety & data → Updates: look for updates by himself (on by default), install updates by himself (off by default), "Check now", and after an update the buttons to roll back or to skip a version.
- Settings → Safety & data → About & quit: the version you are running.

## Limits
- Rolling back keeps your memory, settings and agents as they are; only the app goes back.
- Rolling back and skipping a version are buttons for you; Pinchy cannot press them.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
