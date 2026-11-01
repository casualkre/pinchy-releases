---
title: "Talking while he works: add a note without stopping the job"
description: "You can type and send messages while Pinchy is working on a job. Your message joins the job he is doing: he reads it at his next step, answers it and carries on. Nothing he has done so far is thrown away."
keywords: "type while he is working, typing, write, send a message while busy, interrupt, mid task, add something, added, You added, change my mind, forgot to say, cancel, stop, stop him, steer, correct him, queue, wait, take back, waiting, overloaded, retrying, trying again, closed before he answered, lost answer, try again, draft, not sent"
permalink: /chat-while-he-works/
---
# Talking while he works: add a note without stopping the job

You can type and send messages while Pinchy is working on a job. Your message joins the job he is doing: he reads it at his next step, answers it and carries on. Nothing he has done so far is thrown away.

## What to ask for
- "Also make the title blue." Sent while he works: he reads it between two steps and does it as part of the same job.
- "Use the 2024 numbers, not 2023." A correction reaches him before he finishes, so he does not finish the wrong thing first.
- "How far are you?" He answers in the same reply and keeps going.
- "Stop, I changed my mind." He reads it and stops or changes course.
- `/stop` Stops what he is doing right now, without a note.

## How it works
- A job is many small steps (read a file, run a command, look at a page). Your message is handed to him while the job runs, and he reads it as soon as the step he is in has finished.
- He answers in the reply he is already writing: one job, one reply.
- "You added: …" under his reply means: these are the messages you sent while he was working on this job. A ✓ after a message means he has read it.
- When he is inside one long step and cannot read anything (a long command, a slow download), Pinchy waits 20 seconds, then stops that step once and gives him your note. He carries on with the job with your note in mind.
- A message sent from the phone app or from Telegram while he works is handled the same way.
- If his turn breaks before he read your note (Claude can't be reached, or Claude Code stopped), your note is not lost: it goes out by itself as the next message and he answers it.
- Stop greys out ("Stopping…") the moment you press it; one press is enough. It also closes a permission window that was waiting for that job.

## Settings
- Settings → Brain → Chat → "Messages while he works change the job": on by default. Off: a message sent while he works waits, and he answers it after the job is finished. It shows under his reply as "Waiting: …"; **Take back** puts its words back in your box. If you press Stop, a waiting message is not sent, and the chat says so.

## When something goes wrong
- "Claude is overloaded — trying again (2/10) in 8 s" (or "Can't reach Claude"): Claude Code tries again by itself, a few times. You don't need to do anything; Stop ends it.
- "Pinchy was closed before he could answer this": Pinchy was closed or restarted while he answered. **Try again** asks him once more in the same conversation (he checks first what he had already done); **Dismiss** leaves it. Sending a new message also clears it.
- A message that could not be sent (an add-on stopped it, a question card is waiting for your answer, Claude Code is missing) stays in your box, with a line saying why.
- What you were typing is kept if Pinchy restarts or crashes, and comes back in the box.
- While a question card is open, what you type answers it — also something that starts with "/", like a folder path. Only Pinchy's own /commands run as commands.

## Limits
- He reads a note between steps, not in the middle of one.
- A note belongs to the job that is running. It does not start a second job next to it; for separate work at the same time, use an agent or a swarm.
- `/stop` and "stop" end the job. What he already changed stays as it is; see the page about undo for taking things back.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
