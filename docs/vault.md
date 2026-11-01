---
title: "The vault"
description: "The vault is where you keep your passwords, logins, cards, API keys and secret notes. Pinchy and your agents never see what is in it. They only know a name like vault:hetzner, and when one is needed the vault fills it in after you approve."
keywords: "vault, keep passwords, keep my passwords, password, passwords, logins, login, sign in, card, credit card, api key, key, secret, secrets, passphrase, recovery code, keyring, approve, fill, autofill, 2fa, one time code, lost passphrase, forgot passphrase, import secrets"
permalink: /vault/
---
# The vault

The vault is where you keep your passwords, logins, cards, API keys and secret notes. Pinchy and your agents never see what is in it. They only know a name like vault:hetzner, and when one is needed the vault fills it in after you approve.

## What to ask for
- "What's in the vault?" He lists the names and sites, never a value.
- "Sign in to Hetzner." He opens the site and asks to use the saved login. You press Approve in the vault's own window.
- "Save my GitHub login." He opens the vault's window, and you type it there, never in the chat.
- "Check my Hetzner servers with the API key." The vault makes the call itself, sends the key only to the saved site, and gives him the answer with the key taken out.

## How it works
- A separate program: the vault runs on its own, apart from Pinchy. Pinchy can only ask it to do something. There is no way to ask it for a value.
- Two locks: opening the vault takes your passphrase and your system keyring together (KWallet or GNOME Keyring, Windows, macOS Keychain). One without the other opens nothing. With no keyring it runs on the passphrase alone, and the vault says so.
- Its own window: the passphrase, every value and every Approve go through a small window that belongs to the vault, not to Pinchy. Pinchy's own windows only show names.
- Auto lock: it locks after 15 minutes without use (you can change that), when your screen locks, when the computer sleeps and when Pinchy quits.
- Approve: every use asks you. You see who asks, for which item and on which site. Full autonomy doesn't skip this. A card, or an item you mark, also asks for your passphrase or your phone's fingerprint, because a plain button could be pressed by an agent that controls your mouse.
- Fills stay on the saved site: a value only goes to the exact site it was saved for, into the right kind of field. While a secret is on a page he can't read that page, take a screenshot of it or run code in it, until a new page loads or he clears it.
- API keys: he can't put a key in a command, because he never has it. The vault sends it in the one header you saved for it. It follows no redirects.
- Your phone: Approve works with your fingerprint in the Pinchy app, once you add the phone in the vault's window. Cards stay PC only unless you turn that on. The vault must be unlocked on your PC.
- Agents on the away server: off for each item until you turn it on. Each use needs your Approve, the value is sent encrypted for that one fill, and it is wiped after. Your PC has to be on, since the vault stays on it.
- Limits: a limit that says "no vault" holds for every model, CLI harnesses too. Lifting one asks for your passphrase.
- Activity: the vault's window lists every use: when, who, which site, what you answered. Never a value.

## Forgot the passphrase
When you make the vault it shows a recovery code once. Write it down. It opens the vault and lets you set a new passphrase, also if your keyring is gone. Without the passphrase and the code, nobody can open the vault, not even Pinchy's makers.

## Moving your old secret files in
If you have plain files in Pinchy's secrets folder, the vault offers to import them. It reads them itself and shows you only what it found: the file name, the fields, a site. You give each login its site. If a file holds more than fits one item, such as backup codes or a second account, the whole file goes in as well, as a note you can open with your passphrase. The plain files are deleted only when you say so, with your passphrase, and only those that went in unchanged. Change a password that matters afterwards if you want to be sure no copy is left on the disk.

## What the vault can't promise
- It keeps saved values away from Pinchy and his agents: they only ever hold a name. It can't fully guard against a program running as you, and an agent with a terminal is one, as is a virus you installed. Such a program could show a fake vault window.
- On Windows a program running as you could read the vault's memory while it is unlocked, so keep the auto lock short. On Linux the vault's own process is closed to other programs, but the window's page, where you type, relies on a kernel setting (`ptrace_scope`). The window warns you when that setting leaves it open.
- On Linux without Wayland (an X11 session), any program of yours can listen to what you type into the vault window and read what it shows. On Wayland it can't: the window runs natively there. Windows and macOS keep the window out of screen captures; Linux can't.
- A program running as you could draw a window that looks like the vault's. Only type your passphrase when you opened the vault yourself or Pinchy just asked for a saved login.
- An agent that controls your screen can press a plain Approve. It gets a sign-in on the saved site, never the value. Cards, and items set to ask for your passphrase, need the passphrase or your phone.
- A site you saved sees what you fill in, as with any password manager.
- Copying an old vault file back undoes later changes to it, like a deleted item or a limit. That needs no passphrase. Change the password of something you deleted because it leaked.
- On the away server a value exists in memory for a moment during the fill.
- A fill happens only in Pinchy's own browser, here or on an away server that has one. An agent's virtual machine gets no fills: the model has full control inside it, so nothing could keep it from reading the field. Use Pinchy's browser for the sign-in.

## Settings
- Right-click Pinchy → Vault: what is in it, Lock now, activity. Add, Edit and Delete open the vault's window.
- In the vault's window: Auto lock, Cards from the phone, Limits, and for each item: its site, Ask for my passphrase every time, Allow on the away server.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
