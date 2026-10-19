---
title: "Telegram: talk to Pinchy from a chat app"
description: "Pinchy can live in a Telegram chat. You write to your own bot, Pinchy answers there, and he tells you when something needs you: an approval, a question, an agent that is done, a swarm that finished. It works from anywhere your phone has internet, without the Pinchy phone app."
keywords: "telegram, messenger, code job from telegram, work job from telegram, /code, /work, /jobs, approve from a chat, admin password from telegram, sudo from telegram, from tag, messaging app, bot, botfather, chat from my phone, text pinchy, message pinchy, approve from telegram, notifications, away, pc off, computer closed, voice note, send a photo, send a file, board, dm, swarm from telegram"
permalink: /telegram/
---
# Telegram: talk to Pinchy from a chat app

Pinchy can live in a Telegram chat. You write to your own bot, Pinchy answers there, and he tells you when something needs you: an approval, a question, an agent that is done, a swarm that finished. It works from anywhere your phone has internet, without the Pinchy phone app.

## What to ask for
- Just write: "are the backups done?" He answers in the chat, like in the chat bubble on your computer.
- Send a voice note. He turns it into text on your computer and answers (by voice too, if you like).
- Send a photo with a question: "what is wrong with this error?" Send a file and he saves it and reads it.
- "/agents" shows your agents with Run and Pause buttons. Reply to an agent's message to talk to that agent.
- "/to Price watcher how much is it today?" talks to one agent. The chat then stays with that agent: what you write next goes to it too. "/pinchy" brings you back to Pinchy.
- "/code fix the login redirect" starts a Code job, "/work write a one-page summary of this month's invoices" starts a Work job. The chat tells you when the job needs you and when it is done.
- "/swarm compare five note apps for a small team" starts a crew. When they finish, the result and its files arrive in the chat.

## Setting it up
- Open Settings → Agents & automation → Telegram & chat apps.
- Make a bot: open BotFather in Telegram, pick a name and a username. BotFather answers with a token that looks like 123456789:ABC…
- Paste the token into Settings.
- Press "Connect my Telegram". It makes a link that works once, for 10 minutes. Open it on the phone that has your Telegram and press Start.
- That chat is now connected. Up to 5 private chats can be connected; groups are not supported.

## What arrives in the chat
- Approvals, with what is asked, why, and Approve and Deny buttons.
- Pinchy's questions, with the choices as buttons when he offers some.
- What an agent says: an ordinary message whose first line is "from" and the agent's name. Reply to it to steer that agent. Run and Pause are in "/agents".
- A Code or Work job that waits for you: what it wants and why. A command has Approve and Deny, a plan has Start and Cancel the job; anything else you answer with a reply.
- One message for each finished round of an agent, however many places it is delivered to.
- "/needs" lists everything that is waiting for you.
- "/made" lists what he made lately (reports, tables, write-ups). Tap one to get it as a file.
- Each connected chat can switch kinds of messages off in Settings → Agents & automation → Telegram & chat apps → Connected chats.

## Talking to one agent
- "/to <name> <message>" sends your message to that agent, and the chat stays with it until you write "/pinchy". "@name <message>" does the same.
- You do not have to type the whole name: the start of it is enough. If two agents fit, the chat asks which one you mean.
- "/to <name>" with no message only switches the chat to that agent.
- A reply to an agent's message goes to that agent for that one message. It does not switch the chat. That is also true for its messages from your away server and from before Pinchy restarted. If two agents have the same name, the reply goes to Pinchy (rename one, or use /to).
- An agent's messages start with "from" and its name, so you always see who is speaking.
- A chat you leave alone for six hours is with Pinchy again.
- This works for agents and tasks, on your computer and on your away server. Swarms have their own commands (below).

## Code and Work jobs
- "/code <what you want>" starts a Code job in the project you used last. "/code in ~/projects/site: <what you want>" names the folder. The first message says which folder it works in.
- "/work <what you want>" starts a Work job: a document, a table, a write-up.
- While a job works, its first message shows the step it is on.
- A small job just starts. A bigger one shows its plan first when you asked for that (Settings → Workspace → Runs, "Plan first and wait for my OK"): the plan with Start and Cancel the job. Reply to the message to say what to change.
- When one of its commands needs your OK, the chat shows the command and what it is for, with Approve and Deny.
- When it needs something else from you, the message says what. Reply to answer.
- A finished Code job says what it changed, with Apply, Keep as a branch and Discard. Nothing is in your folder until you tap Apply. A finished Work job has a button that sends you its file.
- A reply to any message of a job talks to that job: it steers it while it works and goes on with it after it is done.
- "/jobs" lists your jobs. A job you start here is also a conversation in the Code or Work window on your computer.

## Approving from the chat
- Every request says what it is and why. For an admin (sudo) command that is the computer, the exact command and the folder.
- Ordinary requests have Approve and Deny.
- Admin commands, payments and "always ask" requests can only be denied from a chat until you switch on "Approve everything from a chat" (Settings → Agents & automation → Telegram & chat apps). It is off when Pinchy is new.
- With the switch on, they get Approve too. After Approve on an admin command the chat asks for your admin password: you send it as your next message, and Pinchy deletes that message at once. The password does pass through Telegram's servers.
- "/cancel" instead of the password leaves the request waiting, and Deny ends it. A password that starts with "/" or "!" has to be typed at the computer.
- An agent that parked a command that needs root: with the switch on, "Run it" shows you the exact command and asks for the password in the same way.
- On your away server with root approvals turned on (see the page "Away server"), there is no password: each root request comes once, as its own card with the exact command, Allow and Refuse. Refuse works any time; Allow works while your computer is on and "Approve everything from a chat" is switched on (your computer signs it). With the computer off, allow it from the phone app.

## Swarms in Telegram
- "/swarms" shows your crews and how far they are. "/swarm <goal>" starts one.
- A crew member's question arrives as its own message. Tap an answer or reply in your own words. Your answer goes only to the one who asked; the others keep working.
- When the crew itself is stuck or reaches its cost cap, the message has buttons such as Try again, Skip it or Stop here.
- A crew member can send you a message with a picture or a file. Reply to it and only that crew member gets your reply.
- "/board" shows what the crew wrote on its board lately. "/board <message>" writes on it without interrupting anyone; start the message with @Name to reach one of them at once.
- "/dm <name> <message>" writes to one crew member privately.
- When the crew is done you get what they made in a few sentences, what is still open, and the first result files as real files. A button sends the rest.

## When your computer is off
- With an away server (see the page "Away server") and "Keep answering while this PC is off" switched on, the server answers your bot while your computer is asleep or off.
- Pinchy on the server answers your messages himself, with the same memory. Photos and files work. Voice notes do not: speech is turned into text on your computer.
- "/agents", "/run <name>", "/needs", "/status", "/pause", "/resume", "/stop" and "/new" work there. Swarms, "/code", "/work", "/made" and anything that needs your computer's screen or files wait until it is back on.
- If an agent on the server meets a captcha or a sign-in, the chat tells you. You open the screen in the Pinchy phone app and then tap "I'm done" in either place.
- If the server cannot answer, the chat says why, for example that the server has no Claude sign-in yet.

## How it works
- The bot is yours: only Telegram and your own Pinchy see the token. On your computer the token is locked with the system keyring.
- Only chats you connected with the one-time link can talk to him. Anyone else who finds the bot gets no answer at all.
- A message Telegram held back while Pinchy was off for more than two minutes is not acted on. He tells you, and you send it again if you still want it.
- A forwarded message is shown to Pinchy as someone else's words. He does not follow instructions inside it.
- Raising a crew's cost cap, putting results into your files, or allowing a risky step from Telegram follows the same switches as the phone app (Settings → Agents & automation → Phone). When a switch is off, your computer asks you instead.
- Payments, admin (sudo) commands and "always ask" requests are shown in the chat with their details. They can be approved there only after you switched on "Approve everything from a chat" on the computer (see "Approving from the chat").

## Settings
- Settings → Agents & automation → Telegram & chat apps: the bot token, Connect my Telegram, Connected chats (per chat: which kinds of messages it gets, and whether voice notes are answered by voice), Approve everything from a chat, Keep answering while this PC is off, Remove the bot.
- Settings → Agents & automation → Away server: pair the server that answers while this computer is off.

## Limits
- Telegram lets a bot receive files up to 20 MB and send files up to 50 MB. Bigger result files are named in the chat and stay on your computer.
- "Keep answering while this PC is off" stores the bot token on your away server, where the agents running there could read it. Only use a server you run yourself.
- When the server takes over after your computer goes to sleep, there can be a pause of a few minutes before it starts answering. Nothing is lost: Telegram keeps your messages.
- Messages go through Telegram's servers. Do not send secrets you would not put in a Telegram chat. With "Approve everything from a chat" on, anyone who can open your Telegram can approve in your name.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
