---
title: "Code review: find what is wrong in a project"
description: "Code review reads a project for real problems (crashes, wrong results, lost data, security holes), runs the project's own checks, tries the app itself on Pinchy's own desk, and shows you what he found. You decide what gets fixed: he only shows, lets you pick, or fixes the sure ones on a branch of th"
keywords: "code review, my repositories, private repo, github connector, the app itself, website, appimage, exe, test the website, test my program, review my code, review this project, review a repo, review a repository, github repo, git url, pull request from a review, patch, find bugs, find errors, check my code, audit, bug hunt, security review, lint, failing tests, test the app, try the app, desk tester, findings, fix the findings, fix selected, not a problem, dismiss, report, REPORT.md, review window, review job, agent review"
permalink: /code-review/
---
# Code review: find what is wrong in a project

Code review reads a project for real problems (crashes, wrong results, lost data, security holes), runs the project's own checks, tries the app itself on Pinchy's own desk, and shows you what he found. You decide what gets fixed: he only shows, lets you pick, or fixes the sure ones on a branch of their own. It has its own window, separate from the Workspace.

## What to ask for
- "Review my notes app for bugs." He opens a review of that folder.
- "Check only what I changed on this branch." A review of the changes, not the whole project.
- "Look especially at the login flow." What you say goes to every reader as the focus.
- "Review https://github.com/owner/name." A repository by its address, without cloning it yourself.
- "Review my lobster repo and test it at https://my-site.example.com." The source from GitHub, the running website tried on his desk.
- "Fix the two high ones from the review." One Code job fixes exactly those, on its own branch.
- "Have the Coder agent review the api-server every Friday." Agents can start review jobs too; their reviews show in the same window, tagged with the agent's name.

## How it works
- Where: the Code review window. Open it from the tray menu (Code review), from the Workspace sidebar, from his right-click menu (add the Code review tile when you customise it), or just ask him.
- The start page: pick a folder on this computer (recent folders are offered) or a repository (pick one of your own from the list, or type its address: https://, ssh:// or git@host:path, an optional branch), the whole project or only what changed, what happens when he finds something (Just show me, Let me pick, Fix them too), whether he tries the app, and how deep he reads (Quick reads the riskiest parts, Deep uses several readers and desks at once). An optional line says what to look at especially.
- The stages show at the top while it runs: Looking around, Running its checks, Reading the code, Double-checking, Trying the app, Writing it up, and Fixing when you chose Fix them too. The bar under them is how much of the code has been read.
- Its checks: your project's own test, lint, type check or build run in a throwaway copy of the project. Your folder is never touched, and uncommitted changes are part of what is reviewed. A failing check is a finding.
- Double-checking: a second reader tries to prove each finding wrong before you see it. What it disproves moves to Dropped; what it could not prove but thinks likely is marked Likely.
- Your repositories: with GitHub connected (Settings → Add-ons → Connectors → GitHub, or `gh auth login`), the start page lists your repositories, newest first, private ones marked with a lock; type to search, click one to pick it. A private one is copied with your GitHub login, which is never written into the copy, the address, the report or the log.
- The app itself (optional): next to the source, give the app to try — "Find it in the code" (he starts it from the project), "A website" (its address; he opens it in a fresh browser on his desk) or "A program file" (an .AppImage, or a Windows .exe that runs through Wine on his desk). When you give the app, it is always tried, even for a repository he only reads, because nothing from the repository runs. On his desk a program can see your files and go online (not your browser, mail or chat data), and what it writes is thrown away — pick only a program you would run yourself. The program file has to be in your home folder, and only you can pick one in this window — an agent's review can give a website, never a program. The review's header shows what was tried. A Windows .exe needs Wine on this computer (without it the review says so), and where his desk can't run (your away server, Windows, macOS, Linux without KDE Plasma 6) Pinchy's VM can only try a website.
- Trying the app: when the project has a window or a web page, he starts it on his own hidden desk (several desks when the review is Deep) and clicks through it. You can watch each desk live in the review window and click one to open it big and take over its mouse and keyboard. Whatever the app writes there is thrown away when the review ends.
- The findings: sorted by how bad they are (High, Medium, Low), or by file. Each one says what is wrong and how it fails, with the code or output as evidence and, for the app, the screenshot. Click the file and line to open it in your editor.
- Fixing: tick findings and press Fix selected (or Fix this on one). That starts one normal Code job on its own branch. When it is done the finding says Fix ready, and the bottom of the window has Apply, Keep as a branch and Throw away. Nothing reaches your branch until you press Apply.
- Not a problem: dismiss a finding and say why if you like. It moves to Dropped, and the next review of the same project is told, so the same thing is not raised again.
- A repository: he copies it just for the review (a shallow copy inside the review's own folder) and throws the copy away with the review. By default he only reads it — it is someone else's code. Tick "Run its tests and app" on the start page to let him install it in the copy (install scripts off), run its tests and try the app on his own desk.
- Running a repository's code is sealed off: its install and tests run in a box that sees only the copy — your home folder, your keys, Pinchy's data and your tokens are out of reach, and nothing it writes outside the copy is kept. That box needs Linux with bubblewrap (bwrap); on Windows, macOS or a Linux without it the review reads the code only and says why.
- Only your own tick runs a repository's code. When Pinchy or an agent starts a review of a repository address ("Review https://github.com/…"), it is always a read-only review; tick the box in the window yourself if you want its tests run. A fix of a repository is written but not run or tested (it is someone else's code) and leaves as a draft pull request (GitHub signed in, gh auth login, and push rights) or a .patch file you save. A private repository works when GitHub is connected or your own git already knows the login.
- The report: every review writes a REPORT.md with all findings, the checks and what was read. Report in the window opens it.

## Settings
- The model that does the review is the one for Code mode: Settings → Workspace → Code mode.
- Trying the app needs Pinchy's own desk: Settings → Computer → Pinchy's own desk. When it is off or cannot run on this computer, the review says so and reviews the code only.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
