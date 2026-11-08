---
title: "Pinchy's browser"
description: "Pinchy and your agents have their own web browser: real Chromium with an ad blocker (uBlock Origin Lite) built in, in your colours. It never touches your normal browser, your mouse or your keyboard. You can open it yourself too: right-click Pinchy → **Browser**."
keywords: "browser, pinchy's browser, chromium, chrome, web, website, ad blocker, ublock, ublock origin lite, ads, open the browser, side panel, macros, record a macro, page script, userscript, tampermonkey, captcha, solve captcha, login, signed in, share login, away agents, cookies, pdf, save as pdf, search the web, read pages, research, extract, scrape, table from a page, network log, console, reverse image search, ocr, theme"
permalink: /browser/
---
# Pinchy's browser

Pinchy and your agents have their own web browser: real Chromium with an ad blocker (uBlock Origin Lite) built in, in your colours. It never touches your normal browser, your mouse or your keyboard. You can open it yourself too: right-click Pinchy → **Browser**.

## Getting it
- The first time, it downloads once (about 210 MB): press **Install** in the setup, in "What's new", or in Settings → Computer → Pinchy's browser. Until it is in, Pinchy uses his basic built-in browser (it works the same, just without the ad blocker and the side panel).

## What to ask for
- "Find the cheapest flight to Izmir next Friday." He searches, reads several pages at once and tells you what he found, with links.
- "Turn this page into a table of names and prices." He reads the page into exactly the columns you want.
- "Save this page as a PDF." It lands in Downloads → BlueLobster.
- "What's in this picture? Where else is it online?" He runs a reverse image search (Google Lens, Bing, Yandex, TinEye).
- "Why does my web app fail to load?" He reads the page's network log and console errors.
- "Read the text in this chart." He reads text that is only in pictures.

## The side panel
Click the lobster icon in the browser's toolbar. It shows who is using this window (Pinchy, an agent or a krill), and has:
- **Stop** and **Take over / Hand back**: take the controls whenever you want; he waits until you hand them back.
- **Needs you**: when a site wants a captcha, a login or a code, he asks you instead of guessing. Your phone gets a "needs you" too. Solve it, press **Done**, and he carries on (he also notices by himself when the captcha is gone).
- **Ask Pinchy about this page**: type a question, and it goes to his chat with the page attached.
- **Macros**: press **Record a macro**, do the steps once, press **Hand back**. Pinchy and your agents can then repeat them quickly. Pinchy asks you before he runs one, because a macro can pay, send or delete. What you type into password or card fields is never recorded.
- **Page scripts**: a few lines of JavaScript that run on every page of one site (hide a banner, add a button). Add your own in Settings. An agent can only suggest one: you see the code and say yes or no.
- **Share this site's login with my away agents**: see below.

## Your agents and their windows
- Each agent and krill gets its own window, so they never get in each other's way, and they all share the browser's logins on this computer. Work nobody needs to watch happens in windows you don't see.
- Research (searching, reading many pages, reverse image search) happens logged out, in a fresh private window each time, and only on public websites. So nobody can quietly read your mail or your router's admin page that way.
- Logins from the vault are filled in after you approve, and Pinchy never sees them.
- Files only leave this computer through the browser when you or an agent upload them on purpose. Key folders, Pinchy's own data, hidden files and password stores are never uploaded.

## Away agents and your logins
Your away agents can use a site you are signed into here, but only one site at a time and only when you say so. Open the site in Pinchy's browser and press **Share this site's login with my away agents** in the side panel. Pinchy's own approval window then asks you, and names exactly what goes (that site and its subdomains). **Stop sharing** (side panel or Settings) removes it from the server again. Vault logins don't need this: they already work on the away server.

## Settings
Settings → Computer → Pinchy's browser: install or check the engine, the sites shared with your away agents (Stop sharing), your macros (rename, delete), your page scripts (on/off, add your own), and an Engine switch to go back to the basic browser.

## Good to know
- The sites you were signed into in the old browser stay signed in: the first time the new one starts, it brings them along.
- Linux, Windows and macOS. On Linux, if your system blocks Chromium's sandbox, Pinchy keeps the basic browser and tells you why. He never turns the sandbox off.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
