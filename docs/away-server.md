---
title: "Away server: Pinchy keeps going while your computer is off"
description: "An away server is a second Pinchy without a screen, on a small machine that is always on: a home server, a mini PC or a rented server. It shares Pinchy's memory. While your computer is asleep or off, it keeps your agents' schedules going, runs your server agents, and answers your Telegram bot and yo"
keywords: "away server, away mode, server, change server, move agents, another machine, only this computer, vps, home server, raspberry pi, docker, headless, computer off, pc off, laptop closed, asleep, keeps running, runs while I sleep, claude login, second pinchy, takeover, hand over, sudo on the server, root on the server, administrator, passwordless root, root approvals, allow root command"
permalink: /away-server/
---
# Away server: Pinchy keeps going while your computer is off

An away server is a second Pinchy without a screen, on a small machine that is always on: a home server, a mini PC or a rented server. It shares Pinchy's memory. While your computer is asleep or off, it keeps your agents' schedules going, runs your server agents, and answers your Telegram bot and your phone.

## What to ask for
- "Set up an away server." Pinchy walks you through it: one line to paste on the other machine.
- "Move my agents to another machine" or "bring my agents back to this computer." That is "Change…" on the same card.
- "Is the away server working?" He tells you whether it answers, when it last synced and what runs there.
- "Run my price watcher on the server." An agent can live on the server so it works while this computer is off.
- "What happened while I was away?" He shows what the server did and what it wants to tell you.

## What works while your computer is off
- The scheduled runs of your agents and the heartbeat this computer would have run. They never run twice: the server only takes them over when this computer has been away for a few minutes.
- Agents that live on the server keep working all the time, also while this computer is on.
- Telegram: with "Keep answering while this PC is off" switched on, Pinchy on the server answers your messages. See the page "Telegram".
- The phone app shows the server's agents and what is waiting for you, and lets you answer them.
- A swarm working on the server is not interrupted by the server updating itself; after a restart it carries on by itself.

## What waits for your computer
- Anything that needs this computer's screen, mouse, files or apps.
- Your wallet and your passwords never go to the server.
- Voice notes: speech is turned into text on your computer.

## Setting it up
- Settings → Agents & automation → Away server → "Keep working while this computer is off?" → Yes. The same question is at the top of the Agents window, in the form when you create an agent, and in the welcome.
- Pinchy asks which machine: a computer at home that stays on, or a free cloud server. Then he shows ONE line. Paste it in that machine's terminal: it installs him there, and this computer finds and connects it by itself. No address to type.
- "This machine is only for Pinchy" gives him his own screen and browser there, so a sign-in or a captcha can be finished from your phone. Without it he works in a closed box with text and files only.
- If his brain is not signed in there yet, the card shows the one command for it. Without a sign-in the other machine can receive a message but cannot think, and it tells you so.
- If the machine sits on your home network, your phone only reaches it at home. The Phone screen (Settings → Agents & automation → Phone) says in words whether your phone reaches Pinchy away from home and what the next step is.

## Changing it later
- On the same card, once a machine is set: "Runs on a computer at home / a cloud server · Change…".
- "Another machine" runs the same short setup and moves your agents there, with their notebooks. "Only this computer" brings them back here; they then work only while this computer is on.
- While you set up the new machine your agents wait on this computer. Nothing runs twice, and nothing is deleted on this computer.
- At the end you choose what happens to the old machine: "Clean it" (everything of Pinchy's is deleted from it; you get one line to remove the program itself) or "Leave it as it is" (he stops working there, its copy of his memory stays on its disk).
- An agent that comes back to this computer loses the powers only you can give (working without asking, the wallet); the card names them.

## How it works
- The brain folder (memory, skills, tasks, what he made) is synced to the server every few minutes.
- This computer tells the server it is awake. When that stops, the server waits a minute or two and then takes over the scheduled work and the Telegram bot. When this computer is back, it hands them back.
- On the other machine Pinchy lives in a closed box, unless you gave him the whole machine. What he may do there is your choice: work freely in his own space, or skip anything risky and tell you.
- When something on the server needs you (a question, a captcha, a sign-in), it reaches your phone and your Telegram chat. A screen step is opened from the phone app.
- What an agent on the server wants to tell you (a result, a question): while this computer is on, it asks the server every few seconds and shows it at once here, on your phone and in your chat apps. While it is off, the server's own bot sends it, if "Keep answering while this PC is off" is on; without that switch you find it under "While you were away" when the computer is back.
- Restarting or updating the server only cuts the round that is running; the agents start again by themselves.
- What it keeps: its files, the agents' notebooks and its browser logins stay across restarts and updates — also sites you signed into without "remember me". Its desktop and its agents use the same browser, so a sign-in you finish there is the agents' sign-in too.
- Each agent on the server has the server's screen, mouse and keyboard as its own computer (on by default). You watch it on the right of the agent's chat in the Agents window and can take control there.
- Updating it: Settings → Agents & automation → Away server → Update now (only releases signed by Pinchy's key; if the new one does not start, it goes back by itself). Most fixes for away agents run on the server, so update it after this computer updates — or switch on "Keep Pinchy there up to date".

## Root (administrator) on the server, without a password
- Only on a machine you gave him ("This machine is only for Pinchy"). Turn it on once: Settings → Agents & automation → Away server → "Root commands: off" → Turn on. You type that machine's sudo password one last time.
- After that, when Pinchy or an agent there needs root (installing a program, a system service) — at any autonomy level, whether it uses its root tool or types sudo in its own shell — you get the exact command, and where it runs, on this computer (a notification and the Agents window), on your phone, or in Telegram. You press Allow or Refuse. No password to remember.
- It runs only after your Allow, and exactly the command you were shown: the server checks your computer's or your phone's signature for that one command. Nothing on that machine can run root without it, not even an agent that tries.
- Your phone can allow it while this computer is off (fingerprint or screen lock). Telegram can refuse it any time; it can allow it only while this computer is on and "Approve everything from a chat" is switched on.
- If the command runs a script or a build in a folder your agents can change, the card says so.
- Telegram gets each root request once, as its own card with Allow and Refuse. The agent that asked gets the command's output after your Allow, or your Refuse.
- The page shows whether root approvals are on as they are right now: it checks again when the server reconnects, after it updates and right after you turn them on.
- To turn it off, on the server: sudo pinchy-away root-setup --off

## Settings
- Settings → Agents & automation → Away server (its own page since 2.6.1): at the top how it is right now (connected, which Pinchy it runs + Update, root approvals, its desktop, what it keeps, cloud storage and Telegram from the server), then the question (No / Yes) and "Runs on … · Change…"; under it What he may do there, Sync the brain every, Keep Pinchy there up to date.
- Settings → Agents & automation → Telegram & chat apps: Keep answering while this PC is off.
- Settings → Agents & automation → Phone: whether the phone reaches Pinchy away from home.

## Limits
- The server uses your Claude plan like this computer does.
- A server on your home network is not reachable from outside unless you add a way in (Tailscale, or Pinchy's own encrypted link when it is switched on).
- After this computer goes to sleep there can be a pause of a few minutes before the server takes over.
- If your server agents show "Stopped" after updating to 2.5, resume them once. Older versions stopped them on every server restart; that is fixed.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
