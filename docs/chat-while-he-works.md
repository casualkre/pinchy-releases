---
title: "Talking while he works: add a note without stopping the job"
description: "You can type and send messages while Pinchy is working on a job. Your message joins the job he is doing: he reads it at his next step, answers it and carries on. Nothing he has done so far is thrown away."
keywords: "type while he is working, typing, write, send a message while busy, interrupt, mid task, add something, added, You added, change my mind, forgot to say, cancel, stop, stop him, steer, correct him, queue, wait"
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

## Settings
- Settings → Brain → Claude → "Messages while he works change the job": on by default. Off: a message sent while he works waits, and he answers it after the job is finished.

## Limits
- He reads a note between steps, not in the middle of one.
- A note belongs to the job that is running. It does not start a second job next to it; for separate work at the same time, use an agent or a swarm.
- `/stop` and "stop" end the job. What he already changed stays as it is; see the page about undo for taking things back.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
