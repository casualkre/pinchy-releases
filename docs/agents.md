---
title: "Agents: coworkers with a standing job"
description: "An agent is a coworker you give a job to once. It works on its own, on a schedule or when something happens, and writes to you only when it is done, has an update, or needs your help or approval. You do not manage it step by step."
keywords: "agent, agents, coworker, scheduled task, routine, reminder, automation, every morning, every day, watch, monitor, keep an eye, heartbeat, background, standing job, recurring"
permalink: /agents/
---
# Agents: coworkers with a standing job

An agent is a coworker you give a job to once. It works on its own, on a schedule or when something happens, and writes to you only when it is done, has an update, or needs your help or approval. You do not manage it step by step.

## What to ask for
- "Every morning at 8, send me five lines on what changed and what needs me." A morning brief, delivered where you want it.
- "Translate every new document that lands in this folder, and check each page before you give it to me." A translator that proofreads itself.
- "Keep my project moving: every evening, do the next thing on the list and tell me what you did." A project coworker.
- "Tell me when this page changes, and what the change means for me." A watcher with judgement.
- "Remind me in ten minutes to call Ada." A one-off reminder, the smallest kind of agent: it costs nothing to run.
- "What are my agents doing?" He lists them, their last runs and anything waiting for you.

## How it works
- You describe the job in a chat, or pick an example card in the Agents window and fill in its fields. He shows you the agent and asks before it starts.
- An agent wakes on a schedule, or on a wake-up that costs nothing to check: a file or folder changed, a website value, a new email, a calendar entry, a variable.
- It keeps its own memory in its own folder, so it remembers what it did last time.
- Results go where you choose: a notification, a note on the desktop, the phone app, Telegram, email, or a saved place such as a Discord channel.
- When an agent needs you, it asks. You answer in the Agents window, on the phone or in Telegram.
- "Keep an eye on…" requests with nothing to do on a schedule go on the heartbeat list: a small, cheap model checks the list regularly and wakes the big one only when something is worth acting on.
- An agent can hand a big job to Pinchy's engines: a Code or Work run, or a whole swarm. A swarm it starts belongs to it. When the crew has a question, the agent answers what its job description and its notes settle, and sends you only what it cannot decide, with its reason. When the swarm is finished the agent gets the real files and a plain statement of what is still open, so it can check the work before it tells you.
- With an away server, your agents keep running while this computer is off.
- There are no separate "scheduled tasks" any more: a task is an agent with a time or a wake-up. The tasks you had before this version were turned into agents the first time it started, with the same words, times and way of telling you; a copy of the old list is kept. One message told you how many moved and anything that could not be carried over exactly.
- An agent can have conditions: only on certain days, only while you are away from the computer or only while you are at it, not on battery, only while a variable says so. If a condition (or a broken wake-up) keeps an agent from running, he tells you once, with the reason, instead of skipping silently.
- An agent made from a task without a time (a folder watch, or one you started by hand) runs only when its wake-up fires or you start it.

## Settings
- Settings → Agents & automation → Agents: open the Agents window, pause scheduled tasks, how many may run at once, let agents run, let Pinchy create agents when you ask, how often a scheduled agent may run, away mode.
- Settings → Pinchy → Notifications: where results are sent (under "Results from agents"): your email, quiet hours, saved places.
- Settings → Agents & automation → Heartbeat: the list he keeps an eye on, how often it is checked, how often the big model may be woken.
- Settings → Agents & automation → Variables: live values agents can react to without using your plan.
- Settings → Agents & automation → Telegram & chat apps and Settings → Agents & automation → Phone: reach and answer your agents away from the desk.

## Limits
- Every scheduled run is a Claude round and uses your plan. A run every minute uses it fast; wake-ups are checked without Claude.
- What an agent may do without asking is set per agent. Sending, deleting, paying and admin commands ask you first unless you allowed them for that agent.
- A swarm an agent starts spends from that agent's daily budget, and never more than your cost cap per swarm. Putting a swarm's result into a git project (Apply), raising a limit and permissions are always your decision, never the agent's.
- While this computer is off, agents run only if you set up an away server.

## Creatures: five kinds of agent

When you create an agent you pick what **kind** it is. Every kind is a whole agent: each one can plan, go on by itself, hand big jobs to Code, Work or a swarm, start helpers and use every tool you allow. A kind adds what it is best at and starts from different defaults — nothing is taken away, and whatever you set yourself on the agent wins. If you are unsure, pick the lobster; every agent you already have is one.

| Creature | Best at | What it adds or starts from |
|---|---|---|
| **Lobster** | Anything — the all-rounder. | Plans its work, shows the plan, asks when it must. |
| **Shrimp** | Quick questions and small jobs. | Starts every round on the light model and in a fresh, short conversation, so answers come fast and use little. Give it a model or an effort of its own and it uses that. |
| **Pistol shrimp** | Waiting for something, then acting at once. | While it waits for its watch it costs nothing; when the watch fires it acts at once. A hit always reaches you, a false alarm stays quiet (it is in its chat, without a notification), and it keeps score of how often each watch fired and how often that mattered — a watch that keeps firing for nothing is narrowed by the shrimp itself, and named to you if that does not help. Firings close together count as one: three minutes between two strikes by default; ask Pinchy for another gap, or none. |
| **Mantis shrimp** | Things that must be right. | Thinks harder (high effort on every round), and under each result you see what it really looked at — files, pages, screens — recorded by Pinchy, not claimed by the agent. A result with nothing opened behind it is sent back to look, once, before you get it. The second reader is on by default; tell Pinchy to switch it off for an agent and it is off (that also switches the look-again off). |
| **Crayfish** | Long digging in the background. | Rounds of up to 90 minutes in one kept conversation, an extra round each day just to tidy its notes and memory, and each new day starts from what it did and planned yesterday. |

You can change an agent's creature at any time: ask Pinchy ("make the news agent a pistol shrimp") or change it in Agents.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
