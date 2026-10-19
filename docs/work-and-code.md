---
title: "Work and Code: real jobs done beside the chat"
description: "Work and Code are conversations with Pinchy for real jobs. You write what you want; he answers, or does the work right there and tells you what he made, and you keep talking in the same conversation. Work mode makes finished work products; Code mode changes a codebase."
keywords: "projects, project, start in a project, work mode, code mode, workspace, word, excel, powerpoint, pdf, docx, xlsx, pptx, chart, sources, citations, draft, compare drafts, tidy files, example cards, attached file, progress bar, diff, wrap, revert file, apply as one commit, checkpoint, roll back, run, runs, job, task, edit my project, project folder, my code, document, report, spreadsheet, slides, programming, repository, repo, branch, review, apply, progress, plan, deliverable, code agent, his own branch, his branch, see the changes, throw away, agent branch, attach, attach a folder, zip, pdf attachment, paperclip, files in code mode, project jobs, new work, new code"
permalink: /work-and-code/
---
# Work and Code: real jobs done beside the chat

Work and Code are conversations with Pinchy for real jobs. You write what you want; he answers, or does the work right there and tells you what he made, and you keep talking in the same conversation. Work mode makes finished work products; Code mode changes a codebase.

## What to ask for
- "Write me a two-page comparison of password managers for a family of four, with prices." Work mode: you get the document as a file, attached in the chat.
- "Turn these notes into a 10-slide presentation." Work mode: a real PowerPoint file.
- "Summarise this bank export by month and category, with a chart." Work mode: a spreadsheet with the totals, a chart and the odd rows on their own sheet.
- "Tidy my Downloads folder." Work mode: he shows the full list of moves first and waits for your OK.
- "Rate-limit the login endpoint to five tries a minute per IP." Code mode, in your repository.
- "Customers are sometimes charged twice. Find out why and fix it." Code mode: he proves the bug with a failing test first, then fixes it.
- "How is the run doing?" or "Tell it to also update the README." You can ask about a run or steer it from the chat.

## How it works
- Where: in the Workspace — the grid button first beside Pinchy's chat box, or Workspace in his right-click menu. It opens on what you used last. Pinchy's chat itself has no Work or Code switch any more; a Work or Code conversation you pick in Recent chats opens in the Workspace.
- There are no stages to wait through: he starts on your message. For a job with several steps he writes a short plan in the conversation and changes it as he goes. He asks you only when he cannot go on.
- Work mode: the result is one or more files in a folder for that run, with a short report. The finished files are attached in the chat when the run ends.
- What Work mode can make: Word documents, Excel spreadsheets (with formulas), PowerPoint slides, PDF, web pages, Markdown and CSV, with charts where there are numbers. For research he lists his sources and opens each one again to check that the number he quotes is really on the page.
- Work mode checks its own file before handing it over: that it opens, has the sections and length you asked for, has no leftover placeholder text, no empty slide and no broken formula. What he could not confirm is said in the hand-over, not hidden.
- Tidying files: nothing is moved until you approve the list, nothing is ever deleted (what he would throw away goes into a `.pinchy-trash` folder in the same place), and "Put every file back" undoes the whole job.
- Code mode in a git repository: he never edits your project folder directly. He works on a separate copy; the first time he changes a file there, the work goes onto a git branch called `pinchy/…`. He runs your project's checks himself after a change. When you are happy you press Apply.
- Code mode in a plain folder (no git): he works in the folder itself and keeps checkpoints outside it, so you can see each change, revert one file, or undo everything the conversation changed.
- Before the hand-over, a separate session tries each "done means" point for real (runs the code, opens the document), and reviewers look for problems. Findings are confirmed before time is spent fixing them. If something is still failing after the allowed rounds, he says so instead of calling it finished.
- The Code view is a chat with the code beside it. Your messages and his are bubbles, and the text box is at the bottom; a new Code chat is the same page, empty. Just talk: "hi" or a question about the code gets a plain answer in a few seconds, with no plan and nothing changed. Say what to change and he answers with one line, then does it. While he works, the last bubble shows what he is doing right now and what he says as he goes; for a bigger job he keeps a short checklist there, and it changes as he goes. What he did for an answer is folded on that answer ("What he did"); a check that failed shows the end of its output there. You can type at any time: he reads a message at his next step. While he works and the box is empty, the send button is Stop.
- The code is in the middle. The files he changes open there by themselves as tabs (All changes, then one tab per file), with the whole path on the line under the tabs. A changed file shows its diff (Wrap, Unified or Side by side, Revert file, and Revert for one part of it) or the whole file. The folder button opens the project's files, so you can read any of them. In a narrow window you see the chat first; the Code button at the top swaps to the code and back.
- Apply is on the line under the tabs, next to how many files changed. The ⋯ beside it has Apply as one commit, Keep branch, Pull request and Discard; in a plain folder it is Undo all changes instead. If a check still fails, Keep fixing is under his answer. The next message goes on in the same conversation, and the conversation is named after the first thing he makes in it.
- The Work view is a chat. Your messages and his are bubbles, and the text box is at the bottom. A new Work chat is the same page, empty: say what you want in your own words (or just ask him something) and attach what he should read with the paperclip, a drop, or a pasted screenshot. While he works, the last bubble shows what he is doing right now; what he did for an answer is folded on that answer ("What he did"), and you can open it. When the job has more than one step he shows a short plan, and the plan changes as he goes. You can keep typing at any time: an answer to his question, a change while he works, a follow-up after he is done. The file he makes opens beside the chat (the draft or the result with its outline; Details has the plan, sources, checks and brief). Select a sentence in the draft to leave a comment; your comments become the next draft, and Compare shows what changed between two drafts. His last message has the finished files with Open, Show in folder and More (save as artifact, export, send, do this regularly).
- Attaching works the same in every Workspace mode (Work, Code, Swarm and Research), at the start and in every later message: the paperclip in the text box has **Files…** and **A folder…**, you can drop files or a folder on the page, or paste a screenshot. Any kind of file goes: a PDF, a .zip, pictures, a whole folder. Each one shows as a tile with its size; click it to preview it (see Notes and artifacts).
- The empty start page shows example jobs as cards ("Ready to go"). Open one to see how he would work, fill in its one or two fields and press Use this: it sets the kind of result and the format and puts the request in the box, so you only change the details. If you had already typed something, he asks before replacing it.

## Projects
- Workspace → Projects keeps a project's instructions, its files and its chats together. Open a project and pick New Work, New Code, New Swarm or New Research: the normal page of that mode opens, with "in <project>" next to its name at the top. Everything you start there belongs to the project: it follows the instructions and can read the files. The × next to the project name starts the chat outside the project instead.
- The project page lists every chat started in it, in any mode, newest first.

## A Code agent on his own branch
- A Code agent (Agents hub → New → Code agent) looks after one repository and keeps working on it by himself. **Repository folder** has a **Choose…** button; for an agent on the away server you type the folder on the server.
- **How he changes code**: **Works himself on his own branch** (what a new Code agent does) or **Hands each change to the Code engine** (every change is a separate Code job with its own branch, checks and review; agents made before 2.6 keep this).
- Working himself: he has his own copy of the repository, outside your folder, on a branch called `pinchy/agent-<his name>-…`. He edits, runs the tests and commits there. After every round that changed something, Pinchy commits what he left and runs the project's checks on his branch (the ones under **Checks that must pass**, else the project's own test / lint / build). Your checkout is never touched.
- His card in the Agents hub has **His branch**: how many commits he is ahead of your branch, each check by name (click it for its output), the files he changed, and a note when your repository's commit hook refused a commit or a round was not checked. **See the changes** shows the whole diff. **Apply** brings his branch into your checkout: it refuses while you have uncommitted changes or when it would conflict, and when a check still fails it asks once more (**Sure? Apply anyway**). **Throw away** (it asks once) puts his branch back to yours.
- After you apply, his copy starts again from where your branch is. A Code job he hands on starts on his branch, and its work comes back onto his branch. He can also start a Code review of the project and fix what it confirms (see Code review).

## Settings
- **The Workspace has its own Settings:** ⚙ Settings at the bottom of the Workspace sidebar opens them inside the Workspace, on the tab of the mode you are in — General · Work · Code · Swarm · Research. Each mode starts with its **permission mode** (how much Pinchy may do there without asking you: Read-only, Ask first, Edits allowed, Auto, Full autonomy), then what matters for that mode. Making a mode looser (more autonomy, a higher or no cost limit, no plan first, checks without asking) asks you to confirm in a dialog; making it stricter is saved at once. Research has no permission mode: it only reads the web. "All Pinchy settings" opens the big Settings window, which shows the same settings.
- Settings → Workspace → Runs: "Plan first and wait for my OK" (No, just start · Yes, every time), stop a run after a time or a cost, thinking effort, reviewers. "Show more settings" has the rest: questions first, prove every point before hand-over, runs at the same time, the models.
- Settings → Workspace → Work mode: the folder for finished work, the permission mode.
- Settings → Workspace → Code mode: check the project before changing it, rounds of fixing failed checks, time for the project checks, reuse installed dependencies, prove a bug before fixing it, let him run the project's checks without asking, the coding buddy that reviews your commits (off by default).

## Limits
- A job uses more of your plan than a quick answer, because he checks what he made before he tells you it is done. "hi" or a small question costs one short reply.
- In a git repository your branch is untouched until you press Apply. In a plain folder the changes are already there; use the checkpoints to go back. In a very large folder he works in place without step checkpoints and says so at the start; the timeline can still undo his edits.
- A run stops after 2 hours by default; you can change that.
- A Code agent that works himself keeps his copy of the repository in `~/.cache/pinchy/agents/`; it takes the space of one more checkout. His installed dependencies are copied only where the disk can copy them for free; otherwise he installs them in his copy.
- A Word, Excel or PowerPoint file is checked by its content, not by how its pages look. To have the layout looked at page by page, ask for a PDF as well.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
