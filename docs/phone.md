---
title: "Phone: Pinchy in your pocket"
description: "The Android app talks to the Pinchy on your computer. You chat with him, follow your agents, runs and swarms, answer his questions and allow or refuse what he wants to do, with notifications. At home it uses your Wi-Fi. Away from home it needs one way in, and Pinchy has his own: an encrypted link yo"
keywords: "phone, android app, mobile, pair, pairing, qr code, away from home, outside, mobile data, not connecting, can't connect, cannot reach, reconnect, tailscale, vpn, link, tunnel, cloudflare, fingerprint, approve on phone, sudo on phone, admin password, payment on phone, see my screen, notifications, lost phone, unpair, answer an agent on the phone, question from an agent, keep talking to a finished job, continue a run from the phone, creature on the phone, shrimp, lower autonomy from the phone"
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
- An agent's question is a message in his chat. Tap one of his answers or type your own. If he asked without waiting ("He asked — and carries on meanwhile"), he keeps working and takes your answer when it comes; that kind never raises the "needs you" alarm.
- A Code or Work job that has finished can still be talked to: write the next thing in its box and he goes on in the same conversation.
- New agent: the form has one row "Which creature" (lobster, shrimp, pistol shrimp, mantis shrimp, crayfish) with one sentence on what each is best at. Every picture of an agent in the app shows his creature and colour.
- "How free he is" shows his level. From the phone you can only give him less freedom. More freedom, and "Real full autonomy", are given on the computer.
- If you change the machine that keeps Pinchy working while your computer is off, the phone follows by itself the next time it reaches your computer.

## Settings
- Settings → Agents & automation → Phone: pairing code, paired phones, whether the phone works away from home, "Reach Pinchy from anywhere" with "Reconnect now", and what the phone may do (see my screen, deliver Work/Code results, raise swarm cost caps, switch on Careful skills, allow payments).
- In the app, under its own settings, the Connection page: the addresses the phone tries, which one answers now, and "Away from home".

## Limits
- Android only.
- Your computer must be on (or an away server must be running) for the phone to reach anything.
- The live picture of your screen is off until you switch on "Let the phone see my screen".
- Through an away server, big photos and files are cut off at 5 MB. Over the link or at home they are not.
- Pinchy's own link depends on two free outside services: the tunnel and a public notice board for the address note. If either is down, the phone still works at home and over Tailscale.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
