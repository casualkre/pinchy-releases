---
title: "Krill: workers that do one job"
description: "A krill is a worker that does one job with every tool Pinchy has: the shell, files, the web, a browser, your connectors. You give it a goal and maybe some files, it works beside the chat, hands over the result and is done. You can watch it, steer it and send a follow-up. An agent is different: an ag"
keywords: "krill, job, job doer, code krill, plain krill, custom loop, loops, start a krill, now working, stop, stopping, cancel, side chat, ask about it, project notes, notes, made here, project library, step time limit, paused, trying again, overloaded, web check, static check, projects, project, start in a project, work mode, code mode, workspace, word, excel, powerpoint, pdf, docx, xlsx, pptx, chart, sources, citations, draft, compare drafts, tidy files, example cards, attached file, progress bar, diff, wrap, revert file, apply as one commit, checkpoint, roll back, run, runs, job, task, edit my project, project folder, my code, document, report, spreadsheet, slides, programming, repository, repo, branch, review, apply, progress, plan, deliverable, code agent, his own branch, his branch, see the changes, throw away, agent branch, attach, attach a folder, zip, pdf attachment, paperclip, files in code mode, project jobs, new work, new code"
permalink: /krill/
---
# Krill: workers that do one job

A krill is a worker that does one job with every tool Pinchy has: the shell, files, the web, a browser, your connectors. You give it a goal and maybe some files, it works beside the chat, hands over the result and is done. You can watch it, steer it and send a follow-up. An agent is different: an agent stays, keeps a memory, and messages you. A swarm is many krill on one board for a big job.

Krill replaced Work mode and Code mode. Old Work and Code jobs are still there, on the same list.

## What to ask for
- "Write me a two-page comparison of password managers for a family of four, with prices." A krill: you get the document as a file.
- "Turn these notes into a 10-slide presentation." A real PowerPoint file, or a deck you can edit in a space.
- "Summarise this bank export by month and category, with a chart." A spreadsheet with the totals, a chart and the odd rows on their own sheet.
- "Tidy my Downloads folder." It shows the full list of moves first and waits for your OK.
- "Rate-limit the login endpoint to five tries a minute per IP." A code krill, in your repository.
- "Customers are sometimes charged twice. Find out why and fix it." A code krill: it proves the bug with a failing test first, then fixes it.
- "How is the krill doing?" or "Tell it to also update the README." Ask about one or steer it from the chat.

## Where they are
- Agents window → **Workspace** tab: every krill and swarm, here or on your cloud server. The list shows what needs you first, then what is working, then what is finished. Search and filters are at the top.
- **New krill** starts one. Pick its type on the form (plain, code, code review, research, swarm of krill), say the goal, add files or a folder, pick where it runs and with which model.
- Right click a row for what you can do with it.
- Pinchy starts them for you when you ask in the chat, and so do agents, your phone and scheduled tasks. The list says who started each one.
- Each kind of krill can run on any model you have connected: Claude Code, another CLI, an API key or a local model. A model that can't do tools well will do the job worse, it won't change the rules below.

## Kinds of krill
- **Krill** (plain): any job. It works until it's done, and its files land in a folder for that krill. What it can make: Word documents, Excel spreadsheets with formulas, PowerPoint slides, PDF, web pages, Markdown and CSV, with charts where there are numbers.
- **Code**: works on its own git branch, runs your project's checks, gets an independent review, and one click applies it. See below.
- **Code review**: finds real problems in a folder or a change. See the Code review page.
- **Research**: sources, fact checks and a report with citations. See the Research page.
- **Swarm**: many krill on one board. See the Swarms page.

## How a krill works
- There are no stages to wait through: it starts on your message. For a job with several steps it writes a short plan and changes it as it goes. It asks you only when it can't go on.
- A plain krill checks its own file before handing it over: that it opens, has the sections and length you asked for, has no leftover placeholder text, no empty slide and no broken formula. What it couldn't confirm is said in the hand-over, not hidden.
- Tidying files: nothing is moved until you approve the list, nothing is ever deleted, and you can undo the moves.
- Attach with the paperclip: **Files…** and **A folder…**, at the start and in every later message. You can drop them on the page too. On the cloud server the files travel with the krill and the results come back.
- **Stop** stops at once. **Ask about it** is a small side chat about what the krill is doing and why; your question never reaches the krill and never changes it.
- When a model is busy or overloaded the line says so and it tries again, it doesn't look stuck.

## Code krill
- In a git repository it never edits your project folder directly. It works on a separate copy, and the first time it changes a file the work goes onto a branch called `pinchy/…`. It runs your project's checks itself.
- In a plain folder (no git) it works in the folder and keeps checkpoints outside it, so you can see each change, revert one file, or undo everything.
- A separate session that didn't write the code reviews it. If a check still fails, **Keep fixing** is offered.
- You can just talk to it: "hi" or a question about the code gets a plain answer, nothing changes and no branch appears.
- The changed files open as tabs beside the chat. **Apply** is one click. The ⋯ beside it has Apply as one commit, Keep branch, Pull request and Discard; in a plain folder it is Undo all changes.

## Custom loops
- A loop tells a krill how to work: do the job, have a fresh session judge it, run a check, ask you, repeat until done. The built-in ones are plain, checked (do, then fresh eyes), ralph (repeat until it says DONE) and tdd (do, run the test, fix).
- Make your own on the **Loops** page of the Workspace tab, or ask Pinchy to write one. A loop an agent or Pinchy wrote runs its check commands in the sandbox, and the first time you see the command and approve it.

## A krill in a space
- Start a krill from a space and its results land in that space, where you can edit them like a document.

## A Code agent on his own branch
- A Code agent (Agents → New → Code agent) is an agent, not a krill: it looks after one repository and keeps working on it by itself, on its own copy and its own `pinchy/agent-…` branch. Its card has **His branch**: commits ahead, each check, the files it changed. You apply from there.

## Settings
- Settings → Workspace → All krill: stop a krill after a time or a cost, thinking effort, reviewers, a step's time limit.
- Settings → Workspace → Code krill: rounds of fixing failed checks, time for the project checks, prove a bug before fixing it.
- Settings → Workspace → Plain krill: the folder for finished work, the permission mode.
- Settings → Brain → Models: which model does which part of a job.

## Limits
- A krill uses more than a quick answer, because it checks what it made before it tells you it is done. "hi" or a small question costs one short reply.
- A krill stops after 2 hours by default; you can change that. A step's time limit counts silence, not work: a step with no sign of life for that long is paused with a sentence saying so, and Go on carries on. A busy step is never cut off.
- In a git repository your branch is untouched until you press Apply. In a plain folder the changes are already there, use the checkpoints to go back. In a very large folder it works in place without step checkpoints and says so at the start.
- A code krill can move to your cloud server with **Move to away server** when the server can take it. The conversation goes with it, on Claude Code and on Pinchy's own engine. A model only you have connected on this computer has to be shared with the server too.
- A Word, Excel or PowerPoint file is checked by its content, not by how its pages look. To have the layout looked at page by page, ask for a PDF as well.
- On a CLI other than Claude Code, or a model with no tool calling, some kinds of check are weaker. Model limits are only enforced for API keys and local models; on a CLI they are words in its instructions.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
