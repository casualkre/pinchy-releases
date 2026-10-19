---
title: "Using your computer: your screen, his own desk, his browser, his own computer"
description: "Pinchy can do things on a computer the way a person does: look at the screen, click, type, use apps and websites. He has four places to do that, and he picks the one that disturbs you least. His agents have a computer of their own too, and they can ask to use yours."
keywords: "computer use, mouse, keyboard, click, type, screen, screenshot, desk, hidden desktop, virtual machine, VM, browser, website, open app, control my computer, take control, give back, agent computer, his own computer, server desktop, away server screen, pc_call, calls to my computer, run a command on my computer, read a file on my computer, allow once, always for this agent"
permalink: /using-your-computer/
---
# Using your computer: your screen, his own desk, his browser, his own computer

Pinchy can do things on a computer the way a person does: look at the screen, click, type, use apps and websites. He has four places to do that, and he picks the one that disturbs you least. His agents have a computer of their own too, and they can ask to use yours.

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

## An agent's own computer
- Every agent can have a computer of its own, shown live at the top of its right side in the Agents window (**His computer**). An agent on your away server works on the server's own screen; an agent on this computer works in Pinchy's VM — never on your desktop unless you allow that separately (below).
- While he works on it you see **Using it** next to the title. Hover the picture and press **Take control to click and type**: then your clicks, keys and the **Type into his computer…** box go to that computer, and he waits. Press **Give back** when you are done (it also goes back by itself after a minute without input, or when you open another agent).
- **Bigger** widens the side to read the screen; **Open in its own window** shows it full size. The phone app has the same view, with Take control.
- An agent on this computer whose VM is not set up yet shows **Set up his computer** (a one-time download, a few minutes). One whose VM was switched off shows **Give him his own computer**.
- Settings → Agents & automation → Away server → **His agents' computers** shows the server's screen right now (with **Open it**) and the state of Pinchy's VM here, and says in one sentence what is missing when it cannot run.

## What an agent may use: two different switches
In an agent's settings, under **What he may use**:
- An agent on your away server has **His screen, mouse and keyboard** = the server's own desktop. On by default (when the server has a screen).
- An agent on this computer has two boxes:
  - **His own computer (a VM): screen, mouse and keyboard** — on by default.
  - **Your screen, mouse and keyboard** — your own desktop, only while you are away. Off unless you tick it.

## When an agent needs your computer
- An agent (on this computer or on your away server) can ask to run a command, read or write a file, or look in a folder on your computer while it is switched on. You get one notice with what exactly, and why: **Allow once**, **Always for this agent** or **No** — on the desktop, on the phone and in Telegram.
- **Always for this agent** is per agent and per kind (run, write, read, look in folders). From the away server only reading and looking in folders can be allowed always; running and writing are asked every time.
- What an agent may do without asking is listed on its side under **On your computer** (and in its Guardrails), each with a button to take it back.
- Some things are never allowed this way, whatever you answer: Pinchy's own data and keys, startup files, and admin rights (root goes through its own password or Allow/Refuse dialog).

## How it works
- On your screen he looks once, then does as much as he safely can per step; every click comes back with a picture of the result.
- A key he holds for smooth control is always let go on Stop, on pause, when you move the mouse, or after 30 seconds at most.
- Anything that leaves the computer from his desk (an email sent, a form submitted, a purchase) cannot be undone, so opening an app there asks you first unless you allowed him to act without asking.
- While you hold an agent's computer (Take control), the agent cannot click or type there; it may still look.

## Settings
- Settings → Computer → Computer use: let him use the mouse and keyboard without asking each time (off by default), rehearse without touching anything, fast screenshots, show him the screen after every action, keep a key held between steps.
- Settings → Computer → Pinchy's own desk: what his desk can and cannot do, and the Keep / Throw away review.
- Settings → Computer → Pinchy's computer: open it, memory, CPU cores, disk size, shut down after idle. It never gets more than 40 % of this computer's memory, or more CPU cores than it has minus one.
- Settings → Agents & automation → Away server: His agents' computers (the server's screen and Pinchy's VM).
- Settings → Pinchy → General: Pause Pinchy and the panic shortcut stop everything at once.

## Limits
- His own desk needs Linux with KDE Plasma 6 for now. It has no sound and cannot see or type into your screen.
- His own computer will not start when your memory is too low (it needs its own memory plus 1.5 GB free). It needs QEMU and KVM; when something is missing, Pinchy names it and the one command that fixes it. A cloud server without virtualisation cannot run it — an agent there uses the server's own screen instead.
- The away server's screen needs the "this machine is only for Pinchy" setup; the closed-box setup has no screen.
- He never types passwords for you. A command that needs admin rights shows a password dialog that only you answer (on the away server: an Allow / Refuse, no password).

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
