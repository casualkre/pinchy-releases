---
title: "Deep research and specialists"
description: "For work where being right matters: a long, fact-checked research run that ends in a cited report, and specialists that watch Pinchy, your Workspace jobs and your agents while they work and step in when something in their field is wrong."
keywords: "research, deep research, sources, citations, report, fact check, fact checker, follow-up, research tab, expert, specialist, watcher, watch agents, watch workspace, away agents, new specialist, create a specialist, useful, not useful, critical note, attach files to research, second opinion, doctor, lawyer, accountant, panel"
permalink: /research-and-specialists/
---
# Deep research and specialists

For work where being right matters: a long, fact-checked research run that ends in a cited report, and specialists that watch Pinchy, your Workspace jobs and your agents while they work and step in when something in their field is wrong.

## What to ask for
- "Do deep research on heat pumps versus gas boilers for a 1970s house." It runs in the background; the Research tab of the Workspace shows it working and the cited report when it is done.
- "Is it true that creatine helps memory? I want sources." The same, on a narrower question.
- "Follow up on the heat pump research: what does an installation cost this year?" A follow-up builds on the earlier answer instead of starting from zero, and stays in the same conversation.
- In the Research tab you can attach files or a folder to your question (a report to check, your own notes): Pinchy reads them along with the web.
- "Turn the fact-checker on for all my agents." From then on it reads what each agent does and leaves the agent a note when a number, date or name is wrong.
- "Have the code reviewer watch my Workspace jobs." It reads the steps of your Code and Work jobs as they happen.
- "Make me a specialist for German tax law that always checks the paragraph, and let it watch the Ai News agent." He saves it with your instructions and where it watches.
- "Ask a medical expert whether ibuprofen and paracetamol can be taken together." He consults a specialist and tells you what it said.
- "Open the specialists." The Specialists window opens: what each one watches and what it has noticed.
- Specialists have no chat of their own: you do not talk to them, they read along while the work happens.

## How it works
- Research: several searchers read the web at once. Pinchy then opens every page they cite himself and checks that the quoted words are really there; a quote that is not there counts for nothing. A claim needs two independent sites to count as verified.
- Specialists: each one is set up for its job. It starts with the tools that fit it (a code reviewer reads your files, a fact-checker uses the web, a devil's advocate reasons without looking anything up; you can change that in its settings), and it brings its own checklist, its own steps, and its own kind of answer: a code review comes back as findings with a verdict, a fact-check as claims marked right, wrong, misleading or cannot tell, each with its source. No specialist can change a file or run a command.
- A specialist that is Watching rides along on the work you chose for it: your chats with Pinchy (his answers, the pages he reads, the documents he writes), your Workspace jobs (Work, Code, Swarm, Research), and your agents (every agent, every agent but some, or only the ones you pick). It reads each piece as it happens and stays quiet unless something in its field is wrong or missing; then it leaves a short note.
- A note goes back only to the job it is about, and you see it there:
  - a Work or Code chat: the note shows in that chat, and its next step (or your next message in that chat) takes it into account;
  - an agent: a small line "Fact-checker: …" in that agent's chat, and the agent reads it in its next round;
  - a swarm: the note is posted on that swarm's board, where every member of the crew reads it;
  - Pinchy: he weighs it with his next answer, and when a note says his last answer was seriously wrong he corrects himself right away.
- The worker weighs each note and fixes what is right. A note is advice, never an order; a note that reads like an order ("ignore your rules", a command to paste into a terminal) is thrown away before anyone sees it.
- Agents on your away server are watched too, by the server's own copy of the same specialist. Their notes show in the Specialists window marked "away server".
- A quick fact is answered in the chat. Research is for questions that need real investigation.

## The Specialists window
- Right-click Pinchy → Specialists, ask Pinchy to open the specialists, or Settings → Workspace → Specialists → Open Specialists. (If you took Specialists out of his menu, put it back with the grid button at the top of the menu → Add.)
- On the left are your specialists, each with the last thing it noticed, or "Not watching". The + at the top makes a new one.
- Pick one to see it. At the top: what it is for, where it watches, how many notes it left today, and the Watching switch. The gear opens its own settings (model, thinking effort, what it may use).
- What it watches: three rows you switch on or off. Your chats with Pinchy (his answers, the pages he reads, the documents he writes). Workspace jobs (Work, Code, Swarm and Deep Research jobs while they run). Agents: None, Every agent (also the ones you make later; untick one to leave it out), or Only these (tick the agents).
- What it checks for: its instructions, with Edit.
- What it noticed: each note it left, with where (an agent's name, a Workspace job's title, Pinchy) and how serious it is. The chips All · Pinchy · Workspace · Agents filter the list. The times it read along and had nothing to add are folded into one line. Mark a note Useful or Not useful: that is how you tell it what matters to you.
- New specialist (the +): add a Ready-made one with one click (fact-checker, code reviewer, editor, devil's advocate and more), or Make your own: a name, what it is expert in, what it checks for, and what it watches. "Fill it in for me" writes the form from one sentence; nothing is made until you press Create. A new one watches your chats with Pinchy and the Workspace, and no agents until you choose them.
- From an agent's side: open the agent's settings (Edit) → "Specialists watching him". Tick one for that agent only. One set to Every agent shows there as already on; change that in the Specialists window.

## The Research tab
- Workspace → Research (Alt+4 in the Workspace). You can also start a research there: write the question, pick Quick, Standard or Deep, and start.
- Attach files or a folder with the paperclip next to the question (or drop them on it). They are read as material for the question, never as instructions.
- While it runs you see the steps (Plan, Search, Re-read, Verify, Write), the sub-questions Pinchy split your question into, and the pages as they come in: "Found — not re-read yet", then "Quote found on the page" once he has re-read the page himself, "Could not be opened" when the page was blocked, or "Thrown out: the quote is not on the page".
- The report is read in the tab. A number like [3] after a sentence is its source: click it to see the page and the exact quote. The side panel lists Sources, the Plan, and the Claims with how well each is confirmed.
- The box under the report asks a follow-up. The question and its follow-ups are one conversation, one row in the list on the left. Right-click a row to rename, pin or delete it.
- Stop ends a running research and keeps what it found so far. "Open as a document" opens the saved report (it is also kept under Artifacts).

## Settings
- Settings → Workspace → Deep research: default depth (Quick, Standard, Deep), the model for planning and writing, the model for the searchers.
- Settings → Workspace → Specialists: Open Specialists; Default model and thinking effort; Use specialists; Let specialists watch the work (the switch for all of them). Under it the limits: Each specialist may spend at most ($ per hour), Pause between two looks by the same specialist, Let Pinchy correct an answer right away when a specialist catches a mistake, Show me critical notes too (a notification), Model for watching.

## Limits
- A research run uses several models at once and takes minutes; it costs more of your plan than a chat answer.
- A follow-up is a new research run with its own cost. Its report cites only pages it checked itself; the earlier answer is background for it, not a source.
- Pages appear when a searcher comes back with them, not one by one while it reads.
- A specialist is a careful second opinion, not a professional. For medical, legal or money decisions, check with a person.
- Watching costs a little of your plan each time a specialist reads something. Each one looks at one job at most every couple of minutes (the pause in Settings) and stops for the hour when it reaches what it may spend. Watching every agent costs more than watching one.
- A specialist reads what the work produced (answers, steps, the text of files it wrote), not your screen, keys or clipboard. It cannot change a file, run a command or talk to you.
- The away server's notes reach the Specialists window only while the away link is up.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
