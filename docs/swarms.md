---
title: "Swarms: a crew of Pinchys on one big job"
description: "A swarm is a crew of equal Pinchys that takes one big job and works on it at the same time, deciding as they go on a shared board: each one takes the next useful piece, finishes it, puts it in and takes the next. Use it when a job is too big for one chat: building something with several pieces, a la"
keywords: "swarm, swarms, crew, team of agents, lobsters, lobsters message each other, multi-agent, parallel agents, board, direct message, DM, parked, resume, cost cap, hive, claim, land, idle, resting, go, start, plan first, plan, review, attach, folder, files, sub-swarm, work together"
permalink: /swarms/
---
# Swarms: a crew of Pinchys on one big job

A swarm is a crew of equal Pinchys that takes one big job and works on it at the same time, deciding as they go on a shared board: each one takes the next useful piece, finishes it, puts it in and takes the next. Use it when a job is too big for one chat: building something with several pieces, a large refactor, research with many sources, an audit, a pile of files to process. For a small job a normal chat (or Code and Work mode) is cheaper and faster.

## What to ask for
- "Use a swarm to build a small command line tool in ~/code/notes that syncs my notes to a git repo, with tests and a README." He sets up the swarm and asks you once: "Start this swarm?" with the crew size, the cost cap and the folder. Say go and the crew gets to work at once; there is no plan to wait for. You can switch this question off in Settings.
- "Here is the brief" with a file, a .zip or a whole folder attached: the crew gets them in its board folder and opens them before it starts.
- "Start a swarm to review ~/work/api for security problems. I want a findings list with file, line and severity." A crew reads the code in parallel and one part puts the list together.
- "How is the swarm doing?" He tells you which parts are done, who is working on what and what it has cost so far.
- "Tell the crew to use Postgres, not SQLite." The message goes on the swarm's board for everyone.
- "Ask Coral why the tests are slow." A private message to one member of the crew; only that one gets it.

You can also start one yourself: open the Workspace window, pick Swarm, then New swarm. There you write the goal, attach files or folders (paperclip or drop them), and choose a kind of job, a crew size (Auto is fine), a time limit, a cost cap, connectors and the folder for the results. **Start** starts the crew right away (this button is your go, nothing asks again). **Plan it first** runs a crew with a planner instead: one Pinchy writes the parts and you check and edit them before you press Start the crew.

## The swarm window
Open it from the Workspace window (Swarm tab) or by clicking a crew member on your desktop. It is laid out like a chat app:
- **Left: the conversations.** Board (the whole crew), Files (the board folder), a thread for each part that has a discussion, then the crew: one row per member with what it is doing right now. A member with nothing to do has a hollow dot and says "resting — nothing to do", "resting until "<part>" lands" or "thinks the goal is done". A row is also your private line to that member. "Between lobsters" lists what members wrote to each other in private; you can read every thread.
- **Middle: the conversation you picked**, with one message box under it. The small "To" label above the box says where your message goes: the Board, a part's thread, or one member only. Type @ and a name to get one member's attention on the board. Attach files or a whole folder with the paperclip, drop them on the box, or paste a screenshot; they are put in the board folder (a folder keeps its sub-folders) and the crew can open them. Code in a message has its own Copy button.
- **Interrupt the crew**: a board message normally interrupts nobody (the crew reads it at their next step). Press "Interrupt the crew" before sending when everyone must read it now; it costs one turn per member.
- **Questions for you** are pinned above the message box wherever you are, with buttons when the asker offered choices. Each answer goes to that one question only.
- **Right: details.** Where the run is (Work · Check · Done for a hive; a crew with a plan also has Planning), the parts, the newest files, what it costs and what the crew carries. With a member selected it shows that member instead: its part, Pause, Restart, Remove, its model, and what it did. The button with the sliders at the top right shows or hides this pane; on a small window it starts hidden.
- **Top row:** the swarm's state, cost and time, Pause, and a menu (…) with Add workers, More time or money, Open the results folder and Stop. A thin line across the top shows how many parts are done. The switch next to it changes the middle: Chat, Parts (the board of parts; click a part for who is on it, its proof and its changes), Files, Timeline, and Result once there is one. While a plan waits for your OK there is also Plan.
- **New swarm** shows example cards ("What a crew is good at"). Open one, fill in its fields and press "Use this": it fills in the goal, the folder and a crew size. Nothing starts until you press Start (or Plan it first).
- A finished swarm opens on its Result, with a box under it to ask for a follow-up round in the same folder.

## How it works
- By default a crew works as a **hive**: there is no planner and no plan to wait for. The first member puts the first pieces of the job on the board and starts one; the others join at once. Every member reads the board, **claims** the next useful piece nobody holds (or adds one it sees is missing), builds it, checks it and **lands** it, then takes the next one in the same go. Nobody waits for a teammate: a member that needs something from another asks it in a message and works on something else meanwhile.
- A member that sees nothing useful left for itself **rests**: it has no open session and costs nothing until something wakes it (a message, a new open piece, the piece it waits for landing). When everyone rests and nothing is open, the member who landed last checks the whole job against what you asked for, fixes or puts up what is missing, and then you get the result.
- A piece its member could not finish goes back on the board with a note for whoever can; the same piece stuck twice comes to you.
- Prefer the old way? Settings → Workspace → Swarms → How a crew works → "With a plan first": a planner reads the job and the folder and writes the parts first, and (if you want) you see that plan before any work starts.
- Each member of the crew works in its own copy of the folder, so nobody overwrites anybody. A finished part is merged into the swarm's shared result.
- A part is done when it is checked, not when its maker says so. Checks that are commands (tests, a build) are run by Pinchy himself. In a hive the crew looks at each other's landed work by choice (and fixes what it finds); with a plan first, a part Pinchy could not check himself is looked at by another member, who may improve it directly; you can change this to only the risky parts, every part or none.
- The crew has a board: a shared folder for anything they want to show each other (screenshots, drafts, outputs) and a board chat everyone can read. A message on the board does not interrupt anybody.
- Private messages go to one member only. A member that is in the middle of work reads the message at its next step; it does not have to stop.
- When the crew needs you (a question, a choice, a part that is stuck) you get one question with buttons: in the swarm view, in the phone app, and in Telegram if you connected it. The others keep working on what they can.
- An agent can start its own sub-swarm for a job; it runs as a hive too, with the crew the agent picked (each member with its role), and its card shows in the agent's chat.
- A swarm that one of your agents started belongs to that agent. Its questions go to the agent first; what the agent cannot decide, or does not answer within 15 minutes, comes to you. More money, Apply and permissions always come to you.
- If nothing can move without you, the swarm is parked: every session is closed, the clock stops, and waiting costs nothing. It carries on the moment you answer.
- At the end you get the result with its files. In a git project the changes wait on a branch until you press Apply; in a normal folder the files are put in place for you.

## When Pinchy closes, restarts or updates
- An update waits while a swarm is working. A parked swarm does not hold an update back.
- If Pinchy is closed, crashes or restarts in the middle of a part, nothing is lost: each member continues its own conversation where it stopped instead of starting the part again.
- After an update or a crash the swarm carries on by itself. If you closed Pinchy yourself, he asks first. You can change this.
- A swarm you stopped yourself, one at its cost cap, or one that keeps getting cut off is never restarted without you.

## Settings
- Settings → Workspace → Swarms → How a crew works: "As a hive — they decide as they go" (the default) or "With a plan first — a planner splits the job into parts".
- Settings → Workspace → Swarms → Show me the plan before a swarm I start gets to work: on by default. For a hive it is the one "Start this swarm?" question (no plan); with a plan first you check the parts. It applies to swarms you start from the chat; the Start button in New swarm is already your go, and swarms an agent, a task or the phone starts don't wait.
- Settings → Workspace → Swarms, the rest: how many agents a swarm may have and how many work at the same moment, how many swarms may run at once, which finished parts get a second look, where the agents work (own copy or the same folder), what each agent carries (tools and connectors), the models, the cost cap per swarm and the room in a swarm's board folder.
- Settings → Workspace → Swarms → Carry on with a swarm that was cut off: after an update or a crash (ask me if I quit), always, ask me first, or never.
- Settings → Workspace → Swarms → Show swarm helpers on screen as little Pinchys: the crew walking around on your desktop while they work.
- A project can have its own rules in a file `.pinchy/swarm.json` (which commands check a part, the final check, heavy jobs, house rules for the crew). Pinchy shows you what the file asks for and uses it only after you approved it; if the file changes later, he asks again.

## Limits
- A swarm uses your Claude plan much faster than one chat: every member is its own Claude session. The cost cap per swarm (20 US dollars of usage by default) stops it when reached, and it stops by itself when your plan's usage is nearly used up. Both can be resumed.
- How many members work at the same moment depends on your computer's free memory. On a small machine they take turns; a member that rests frees its place for one with work.
- Files you give a swarm: up to 10 files or folders per message (and with the goal); a folder brings up to 300 of its files (.git, node_modules and links are skipped); one file up to 200 MB; the whole board folder up to its room in Settings (2000 MB by default).
- Builds, emulators and other heavy jobs from all swarms wait in one line so they do not exhaust the computer's memory.
- With the default toolbox ("Focused") the crew works on files, commands and web pages for the job. It does not use your mouse and keyboard, your wallet or admin (sudo) commands, and it cannot change Pinchy's settings.
- Anything that needs your OK still comes to you; the crew cannot approve it for itself.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
