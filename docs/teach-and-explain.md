---
title: "Teach by showing, and explain what is on the screen"
description: "Two ways to work with what you see: show Pinchy a task once and he turns it into a skill, or drag a box around anything and he explains it."
keywords: "teach an agent, teach him a task, show him, watch him try it, what he learned, fixes learned, voice note, agent computer, teach, show, watch me, learn, skill, record, demonstrate, explain, region, screenshot, what is this, error on screen"
permalink: /teach-and-explain/
---
# Teach by showing, and explain what is on the screen

Two ways to work with what you see: show Pinchy a task once and he turns it into a skill, or drag a box around anything and he explains it.

## What to ask for
- "Let me show you how I file my invoices." A small bar appears; you do the task once, add notes if you like, and press Finish.
- "Watch how I do this on the website." The same, in his browser.
- "Do the invoice thing again." He runs the skill you taught him.
- "Let me show Scout how to renew the domain." The Agents window opens at that agent with **Teach him a task** ready on its own computer.
- Press the explain shortcut and drag a box around an error message, a chart or a figure in a PDF: he explains it in the chat.

## How it works
- Teaching: he notes which window is in front, the names of the buttons and fields you use, and what you write in the Note box. He never records your keystrokes. A few screenshots of the window help him understand clicks he cannot name; they are deleted as soon as the skill is written, and never taken of password managers or while Private is on.
- When you press Finish he writes a skill draft. You read it, then save or discard it. Saved skills load by themselves when a later task matches.
- You can teach in three places: your own desktop (say "watch what I do", or put Teach me into his right-click menu with Customize), his browser, and his own computer (the Watch me button in each).
- Explain: only the box you drag is sent to him, with an optional standing question such as "what does this error mean".

## Teach one of your agents
- Every agent has its own computer (Pinchy's VM on this computer, the server's desktop for an agent on your away server). Under it in the Agents window: **Teach him a task** → say what you will show (optional) → **Start showing**. You take the mouse and keyboard; the agent waits. Do the task once.
- While you teach: **Note** (type, or press the mic and say it) adds why you do a step; **Private** stops recording what you type (passwords, codes) — login, bank and code windows are treated as private by themselves; **Finish** writes the lesson, **Cancel** throws it away.
- After Finish: **Save for him** (or Discard) right there, then **Watch him try it now** — he does it once by himself while you watch his screen.
- A lesson you show one agent is that agent's own skill: Pinchy's chat and your other agents don't use it. See them all under **What he learned** on the agent's page: Read, Undo last fix, Remove.
- An agent can ask you to show it something: its question then has a **Show him** button that opens the lesson with the task filled in.
- A lesson nobody finishes ends by itself after a while (20 minutes without anything happening on this computer, 30 minutes of recording on the away server), so the agent gets its computer back; on this computer its steps become a draft you can still save.
- You can also teach an agent's computer from the phone (see Phone).

## Settings
- Settings → Computer → Teach by showing: teach in my own apps, look at the app I am showing, read button and field names, let Claude tidy the steps, the model for writing skills, and "Watch me now".
- Settings → Computer → Explain the screen: switch it on (off by default), the shortcut, what to ask about the region.
- Settings → Add-ons → Skills: every skill he has, switch one off or remove it.

## Limits
- Reading button and field names uses the desktop accessibility service (Linux). Password fields are never read.
- A taught skill fixes itself when a button was renamed or moved, or a new dialog appears: the one who repeats it re-finds it by name, finishes, and corrects that one step — never into a different or riskier button, never a new website or a private part. You get a notice with **Undo**; each skill lists its "Fixes learned" (Settings → Add-ons → Skills, or **What he learned** for an agent's). If the app changed a lot, teach it again.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
