---
title: "Phone: Pinchy in your pocket"
description: "The Android app talks to the Pinchy on your computer. You chat with him, follow your agents, runs and swarms, answer his questions and allow or refuse what he wants to do, with notifications. At home it uses your Wi-Fi. Away from home it needs one way in, and Pinchy has his own: an encrypted link yo"
keywords: "phone, android app, mobile, pair, pairing, phone settings, widget, widgets, home screen widget, quick bar, needs you widget, attach file from phone, send photo to agent, send a folder, download a file to my phone, mark done, dismiss, needs you on the phone, root on the phone, root command, allow root, mute an agent, lock screen, enter sends, text size, open on, haptics, diagnostics, agents on the phone, agent profile, his computer on the phone, take control, qr code, away from home, outside, mobile data, not connecting, can't connect, cannot reach, reconnect, tailscale, vpn, link, tunnel, cloudflare, fingerprint, approve on phone, sudo on phone, admin password, payment on phone, see my screen, notifications, lost phone, unpair, answer an agent on the phone, question from an agent, keep talking to a finished job, continue a run from the phone, creature on the phone, shrimp, lower autonomy from the phone"
permalink: /phone/
---
# Phone: Pinchy in your pocket

The Android app talks to the Pinchy on your computer. You chat with him, follow your agents, runs and swarms, answer his questions and allow or refuse what he wants to do, with notifications. At home it uses your Wi-Fi. Away from home it needs one way in, and Pinchy has his own: an encrypted link you switch on once.

## What to ask for
- "Pair my phone." Pinchy opens the Phone settings with the code to scan.
- "Can my phone reach you when I'm not at home?" He says whether it can, how, and what the next step is.
- "My phone can't connect." He checks the addresses, the firewall and the link, and says what is wrong in words.
- "Reconnect my phone." He opens his link again with a fresh address; the phone finds it by itself.
- "Which phones are paired?" He lists them; you can rename or remove one.

## Pairing
- Get the app: open Settings → Agents & automation → Phone. It shows a code that opens the download page on your phone.
- In the app tap "Pair with my PC" and scan the pairing code from the same settings page. The code works once and only for a few minutes.
- The app only trusts this computer's own certificate, which it learns from the code. Removing a phone in the settings locks it out at once.

## Away from home
There are three ways. Any one is enough, and the Phone settings say in words which one is working.
- Pinchy's own link: switch on "Reach Pinchy from anywhere". Pinchy opens a public address and the app talks to it by itself when no home address answers. Everything on it is sealed for this computer with keys only your phone and this computer have, so nobody in between can read or change it. No extra app on the phone.
- Tailscale: install it on the computer and the phone and sign in with the same account. The Phone settings show the steps.
- An away server that can be reached from the internet. See the page "Away server".

About the link:
- It is off until you switch it on. The first time, Pinchy downloads the small free tunnel program it uses (a checked, fixed version).
- A phone must have been on your home Wi-Fi once after it was paired or updated to 2.5. That is when it gets its keys. The app does this by itself and says so under Connection in its settings.
- The link's address changes when it restarts. Pinchy leaves a sealed note with the new address and the app reads it by itself. If it ever hangs: "Reconnect now" in the Phone settings, or tap the red line in the app.
- While the computer is off, the link is off too. An away server keeps going; see its page.

## Allowing things from the phone
- Ordinary requests: Allow or Deny, one tap.
- Admin (sudo) commands and payments are never one tap. The app shows the exact command and the computer, or the amount and who gets it, and asks for your fingerprint or screen lock. Only then does your phone sign the answer, and the computer accepts it only for exactly what you saw.
- An admin request also asks for that computer's admin password. It travels sealed (or over your home Wi-Fi), is used once and is not kept.
- A phone with no screen lock cannot allow these. They stay on the computer.
- Pairing another phone, full autonomy and the kill switch stay on the computer.

## Agents and jobs on the phone
- The Agents tab is laid out like a messenger: search and + on top, a row of big portraits (who needs you, who is working, the ones you pinned), then one row per agent with his last line and unread count, newest first. Hold a row for quick actions (Pin, Do a round now, Pause, Stop, Details).
- Tapping an agent opens his chat: his messages on one side, yours on the other, and a question, an approval, a file or a job he started shows as a card in the flow. The name at the top opens his profile (his description, his job, how free he is, what wakes him; rename, colour, delete); the screen button opens his own computer.
- His own computer: watch it live, tap "Take control" to do one step yourself (a password, a code, a captcha), then "I'm done" hands it back. An agent with no computer yet gets one with one tap.
- Jobs he started (a swarm, a Code or Work run) show as live cards in his chat: watch, tell it something, or stop it.
- An agent's question is a message in his chat. Tap one of his answers or type your own. If he asked without waiting ("He asked — and carries on meanwhile"), he keeps working and takes your answer when it comes; that kind never raises the "needs you" alarm.
- A Code or Work job that has finished can still be talked to: write the next thing in its box and he goes on in the same conversation.
- New agent: the form has one row "Which creature" (lobster, shrimp, pistol shrimp, mantis shrimp, crayfish) with one sentence on what each is best at. Every picture of an agent in the app shows his creature and colour.
- "How free he is" shows his level. From the phone you can only give him less freedom. More freedom, and "Real full autonomy", are given on the computer.
- If you change the machine that keeps Pinchy working while your computer is off, the phone follows by itself the next time it reaches your computer.

## Files and photos
- The + next to the message box attaches things: "Photos and videos", "Files" (PDF, zip, documents, anything) or "A folder" (sent as one .zip). Any file up to 2 GB. It works in an agent's chat, in Pinchy's own chat and when you start a new job.
- A big file over mobile data asks first (you can switch that off, see Settings below).
- A file an agent made or sent opens on the phone: pictures, text, Markdown and the first pages of a PDF show right there; anything else says what it is. "Download" saves it to Downloads › Pinchy (or Downloads, your choice). A folder from your computer comes as one .zip. Files of an agent on your away server open too.

## Needs you on the phone
- Everything waiting for you is in the Inbox. Tap one and it opens: what it is, who asks and when, the whole text, and what you can do about it right there — its answers, Approve, or "Open his screen" for a captcha or sign-in.
- "Mark done" tells the agent he does not need to wait for you on this; it leaves "needs you" on the phone, the computer and in Telegram at once. "Open the chat" is the last row if you would rather answer him there.
- A command an agent wants to run as root on your away server comes as a request with the exact command. "Allow…" shows it, asks for your fingerprint or screen lock and then your phone signs exactly that command; no password is typed. This works with your computer on or off (then the phone talks to the away server). A root request on this computer itself still needs its password at the computer: from the phone you can say no.

## Settings in the app
The app's own Settings start with what belongs to this phone, then your computer, then the rest. On top: three quick switches, Live updates (off = battery saver), Lock and Haptics.
- This phone:
  - General: "Open on" (the tab the app starts on), Haptics, "Keep the screen on while you watch his screen".
  - Notifications: what may notify you, quiet hours, "Show what they say on the lock screen" (off: only who it is from; with Lock on, nothing shows there), and "Mute an agent": a muted agent stays quiet about its news but still rings when it needs you.
  - Chat: "Enter sends" (off: Enter makes a new line), "Chat text size", "His little animations".
  - Files & data: "Save files to", "Ask before sending big files on mobile data", "Load his screen and pictures on mobile data", and the files kept on the phone with "Clear kept files".
  - Widgets, Connection, Privacy & lock, Look.
- Your PC: Pinchy on your PC (his name, usage level, desk, cloud storage, the away server) and Add-ons.
- More: Your Pinchys (switch PCs, pair another) and Help & about, with "Copy a diagnostics report" (versions and how the phone is connected; no keys and no full addresses) for when something is wrong.

## Home-screen widgets
- Five widgets: Pinchy (what he is up to, with Talk and Inbox), Your agents (all of them, or the ones you pick, each with what it is doing), Needs you (how many things wait and the first few), One agent (one you pick, big, with Message) and Quick bar ("Ask Pinchy…" plus up to three buttons you pick).
- Each widget has its own style (Theme, Dark, Light or See-through) and its own choices. You set them when you place it, and later by touching and holding the widget.
- The app's own Widgets page (in its settings, under This phone) shows live previews of all five in every style and adds one to your home screen with a tap (or: touch and hold an empty spot on the home screen → Widgets → Pinchy).
- With Lock on, widgets show names and counts only, never what an agent is doing.

## Settings
- Settings → Agents & automation → Phone: pairing code, paired phones, whether the phone works away from home, "Reach Pinchy from anywhere" with "Reconnect now", and what the phone may do (see my screen, deliver Work/Code results, raise swarm cost caps, switch on Careful skills, allow payments).
- In the app, under its own settings, the Connection page: the addresses the phone tries, which one answers now, and "Away from home".

## Limits
- Android only.
- Your computer must be on (or an away server must be running) for the phone to reach anything.
- The live picture of your screen is off until you switch on "Let the phone see my screen".
- Through an away server, one answer is capped at 5 MB (a full-size picture of your screen, for example). Files go up and come down in pieces, so they are not cut off.
- Pinchy's own link depends on two free outside services: the tunnel and a public notice board for the address note. If either is down, the phone still works at home and over Tailscale.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
