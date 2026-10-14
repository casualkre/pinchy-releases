---
title: "Add-ons: connectors, skills and extensions"
description: "Three ways to give Pinchy more: connectors link him to the apps and services you use, skills are know-how he loads when a task needs it, and extensions add new looks, tricks, tools and panels."
keywords: "connector, connect, integration, MCP, plugin, extension, add-on, skill, install, library, github, gmail, calendar, notion, slack, google, google drive, google docs, google sheets, zapier, client id, manifest, super extension, super extensions, experimental, deep sea, hide a page, replace a page, engine, drift, extension theme"
permalink: /add-ons/
---
# Add-ons: connectors, skills and extensions

Three ways to give Pinchy more: connectors link him to the apps and services you use, skills are know-how he loads when a task needs it, and extensions add new looks, tricks, tools and panels.

## What to ask for
- "Connect to my GitHub." He opens the connector with one sign-in or one key; no config files.
- "Which connectors do I have switched on?" He lists them.
- "Find a skill for making PowerPoint files." He searches the skill libraries and opens the one that fits for you to read and install.
- "Is there an extension that plays music?" He looks in the extensions library.
- "Write me an extension that shows the weather on your shell." He writes one; you review what it may do before it is switched on.
- "Make me a colour theme in deep greens." He writes an extension that only holds the theme; it shows up with the other themes.

## How it works
- Connectors: each one is a tool server Pinchy can call. You switch on only the ones you want; their tools load when he needs them, so a connector you never use costs nothing in a chat.
- Skills: a skill is a folder with instructions (and sometimes scripts). A switched-on skill loads by itself when a task matches. Skills you taught by showing are here too.
- Extensions: an extension says what it wants to do (show a panel, add a tool, add a colour theme, run on a schedule, reach the internet). You see that list and say yes before it runs, and it runs in a sandbox with only those rights.

## Super extensions (experimental)
A normal extension only adds things. A super extension may also change Pinchy himself:
- hide a part of the app (for example a page in Settings) or show its own page in that place,
- answer one of Pinchy's own tools in his place,
- add an engine: another way of working through a job, which Pinchy uses when you ask for it by name.

How to try it:
1. Settings → Experimental: switch on **Super extensions** and read the warning.
2. Open the Extensions window and pick **Deep Sea**, the example that ships with Pinchy.
3. Before it goes on, the window lists in plain words everything it will touch. Say yes.
4. The app changes at once: a deep-sea colour theme, the Tricks page is gone from Settings, the Focus mode page is Deep Sea's own page, Pinchy's speech bubble no longer shouts, and there is an engine called Drift ("use the Drift engine to plan my move").
5. Switch Deep Sea off, or press "Put everything back" in the Extensions window, and everything is as it was, including the theme you had before.

What a super extension can never touch: the windows where you decide (approvals, the administrator password, the wallet, the consent window), the Extensions window and the Experimental page (your way back), Safety, pause and the kill switch, and the tools behind them. A tool it answers still asks you exactly as the built-in one did. Only your own click switches a super extension on; Pinchy, an agent or a chat app cannot.

## Gmail, Google Calendar, Drive and Slack
- The quick way for a normal Google account: in Settings → Add-ons → Connectors, search "gmail" (or "google calendar") and connect Zapier, Pipedream or Make. One sign-in, no setup on Google's side; you pick there which Google apps Pinchy may use.
- Google's own servers (the cards named Gmail, Google Calendar, Google Drive, Google Docs, Google Sheets, Google Slides, marked "Setup · preview"): Google only lets an app you registered yourself sign in, and your account must be in Google's Workspace Developer Preview Program. The card lists the five steps with a link for each; you paste a Client ID and a Client secret once and all six cards share them.
- Slack (marked "Setup · preview"): Slack's own server works with a small private app in your workspace. The card has the three steps and a "Copy the manifest" button; you paste the app's Client ID, press Sign in and allow it in the browser. In some workspaces an admin must approve the app first. Pinchy then reads and writes Slack as you.
- "Setup · preview" means: new in 2.5 and not yet tried against every kind of account. If sign-in fails, the sentence under the button says why.
- Talking TO Pinchy from a chat app is a different thing, not a connector: see Settings → Agents & automation → Telegram & chat apps (Telegram, Discord, Slack, Matrix).

## Settings
- Settings → Add-ons → Connectors: the library, sign in or paste a key, switch a connector on or off.
- Settings → Add-ons → Skills: Pinchy's skills, also use my own Claude Code skills (on by default), install from the libraries.
- Settings → Add-ons → Extensions: installed extensions, what each may do, the library.
- Settings → Experimental: the **Super extensions** switch, off by default. Off (or Experimental locked) stops every super extension at once.
- Settings → Brain → Claude → Claude Code on this computer: also load the tool servers you use in Claude Code (off by default).

## Limits
- Super extensions are experimental. A super extension can hide something you rely on; if anything looks wrong, switch it off and it is back.
- Engines from extensions run when you ask for one by name. Work and Code keep their own engine, unless a super extension you switched on says it runs them; the list you read before switching it on says so.
- A connector acts with your account: what he does there is done in your name. Sending and deleting ask first.
- Some services need a key or a one-time setup on their side; the connector's card walks you through it.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
