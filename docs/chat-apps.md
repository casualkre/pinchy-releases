---
title: "Discord, Slack and Matrix: Pinchy in the chat apps you already use"
description: "Besides Telegram, Pinchy can answer in Discord, Slack and Matrix (Element and other Matrix apps). In each one you make a bot of your own, connect your chat to it once, and then write to him there: he answers, asks his questions and tells you when something needs you. It works the same way in all of"
keywords: "discord, slack, matrix, element, whatsapp, chat app, messaging app, messenger, other chat apps, bot, direct message, dm, connect discord, connect slack, connect matrix, one-time code, start code, approve from discord, approve from slack, answer with a number, numbered choices, manifest, app token, access token, homeserver"
permalink: /chat-apps/
---
# Discord, Slack and Matrix: Pinchy in the chat apps you already use

Besides Telegram, Pinchy can answer in Discord, Slack and Matrix (Element and other Matrix apps). In each one you make a bot of your own, connect your chat to it once, and then write to him there: he answers, asks his questions and tells you when something needs you. It works the same way in all of them. Telegram has its own page ("Telegram").

## What to ask for
- Just write to the bot: "what is my backup agent doing?" He answers in that chat.
- "status" shows what Pinchy is doing. "needs" lists what is waiting for you. "agents" shows your agents.
- "/to Translator say this in French: good morning" talks to one agent, and the chat stays with it until you write "/pinchy". In Slack write "!to Translator …" and "pinchy". If two agents fit the name, you pick one: a button in Discord and Slack, a number in Matrix.
- "/code fix the login redirect" starts a Code job and "/work …" a Work job, as in Telegram. It writes when it needs you and when it is done; reply to its message to talk to it; "/jobs" lists them. In Slack write "!code", "!work" and "jobs".
- An agent's message is an ordinary message that starts with "from" and its name. Reply to it to talk to that agent.
- When he asks for your OK, press Approve or Deny in Discord and Slack. In Matrix the choices are numbered: reply to his message with the number.
- Send a file or a picture with a question and he reads it.
- "Set up Discord for me" or "why does my Slack bot not answer?" He opens the right Settings page and tells you the next step. He cannot paste tokens or connect a chat himself.

## Setting it up
- Open Settings → Agents & automation → Telegram & chat apps and scroll to "Other chat apps".
- Press "Set up" on the app you want. The card lists the steps for that app and opens its developer page for you.
- Discord: make an application, copy its bot token, add the app to your own account or to a server you own.
- Slack: create an app "From a manifest" (the card has a "Copy manifest" button), then copy the app-level token and the bot token.
- Matrix: make a second account for Pinchy, copy its access token from Element, and give the server address.
- Paste the values into the card and press Connect. Pinchy checks them with the service before saving.
- Press "Connect my Discord" (or Slack, or Matrix). The card shows a code that works once, for 10 minutes. Send that line to the bot from your own account. That chat is now connected.

## What is different per app
- Discord: you write to the bot in a direct message. It never reads a server's channels. Commands also work with a slash, like "/status".
- Slack: you write in the app's Messages tab. Slack keeps the slash for itself, so write "status" or "!status".
- Matrix: there are no buttons, so every choice is a numbered line. For anything that allows or starts something, reply to his message with the number; a bare number only counts right after he asked. Start the chat with encryption turned off: Pinchy cannot read encrypted rooms and says so once if you try.
- Voice notes are answered by voice only where the app supports them.

## How it works
- Each bot is yours. Its tokens are locked with the system keyring on your computer and never shown again, not to Pinchy either.
- Only chats you connected with the one-time code can talk to him. Anyone else who writes to the bot gets no answer.
- A forwarded or shared message is shown to Pinchy as someone else's words. He does not follow instructions inside it.
- A message that waited more than two minutes while Pinchy was off is not acted on. He tells you, and you send it again.
- Admin (sudo) commands, payments and "always ask" requests are shown with what they are and can be denied here. With "Approve everything from a chat" switched on (Settings → Agents & automation → Telegram & chat apps) payments and "always ask" requests can be approved here too.
- An admin password is never typed into Discord, Slack or Matrix: these apps do not let Pinchy delete your message again. Approve admin commands on the computer, in the phone app or in Telegram.
- Nothing on your computer is opened to the internet: Pinchy connects out to the service and listens there.

## Settings
- Settings → Agents & automation → Telegram & chat apps: under "Other chat apps", one card per app with Set up, the switch "Pinchy answers in …", Connect, Connected chats (and what each chat is told about), Remove.

## Limits
- These three answer only while this computer is on. With the computer off, your away server keeps answering Telegram, not the other apps.
- WhatsApp is not supported. Its official way in needs a business account and a public web address, and the unofficial ways break WhatsApp's rules.
- What you write while this computer is off is not picked up when it starts again (Telegram does keep it): write it again.
- Matrix: Pinchy's account accepts an invitation to a chat only while a connect code is open on its card, so strangers cannot pull it into their rooms.
- Up to 5 chats per app. Groups and channels are not supported: Pinchy leaves or ignores them.
- Messages go through the servers of the app you use. Do not send secrets you would not put in that app.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
