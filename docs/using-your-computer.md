---
title: "Using your computer: your screen, his own desk, his browser, his own computer"
description: "Pinchy can do things on a computer the way a person does: look at the screen, click, type, use apps and websites. He has four places to do that, and he picks the one that disturbs you least."
keywords: "computer use, mouse, keyboard, click, type, screen, screenshot, desk, hidden desktop, virtual machine, VM, browser, website, open app, control my computer"
permalink: /using-your-computer/
---
# Using your computer: your screen, his own desk, his browser, his own computer

Pinchy can do things on a computer the way a person does: look at the screen, click, type, use apps and websites. He has four places to do that, and he picks the one that disturbs you least.

## What to ask for
- "Open Dolphin and rename every .txt file in my todo folder to .md." He does it on his own desk and shows you the changes to keep.
- "Fill in this form on the website for me." He uses his own browser; your mouse stays yours.
- "Click the blue button in the window I have open." He uses your screen, because the thing is already there.
- "Install this program and see if it works, but not on my system." He uses his own small virtual computer.

## The four places
- **His own browser**: for anything on the web. It never touches your mouse and several jobs can browse at once.
- **His own desk**: a second, hidden desktop where he uses your apps with his own mouse and keyboard. He can read your files there; your files only change when you press Keep, and the old versions go to the Trash first.
- **Your screen**: your real mouse and keyboard, for something already open in front of you or when you ask for it.
- **His own computer**: a small virtual machine (Alpine Linux) that starts only when needed and keeps its files between sessions. Good for risky installs and long jobs.

## How it works
- On your screen he looks once, then does as much as he safely can per step; every click comes back with a picture of the result.
- A key he holds for smooth control is always let go on Stop, on pause, when you move the mouse, or after 30 seconds at most.
- Anything that leaves the computer from his desk (an email sent, a form submitted, a purchase) cannot be undone, so opening an app there asks you first unless you allowed him to act without asking.

## Settings
- Settings → Computer → Computer use: let him use the mouse and keyboard without asking each time (off by default), rehearse without touching anything, fast screenshots, show him the screen after every action, keep a key held between steps.
- Settings → Computer → Pinchy's own desk: what his desk can and cannot do, and the Keep / Throw away review.
- Settings → Computer → Pinchy's computer: open it, memory, CPU cores, disk size, shut down after idle.
- Settings → Pinchy → General: Pause Pinchy and the panic shortcut stop everything at once.

## Limits
- His own desk needs Linux with KDE Plasma 6 for now. It has no sound and cannot see or type into your screen.
- His own computer will not start when your memory is too low (it needs its own memory plus 1.5 GB free).
- He never types passwords for you. A command that needs admin rights shows a password dialog that only you answer.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
