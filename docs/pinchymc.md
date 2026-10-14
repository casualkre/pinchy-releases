---
title: "PinchyMC: Pinchy plays Minecraft with you"
description: "PinchyMC is a small Minecraft mod that lets Pinchy play in your game: walk somewhere, follow you, mine, craft, build, fight, use chests and chat. The mod does the fast part (finding a path, aiming, clicking at a human pace); Pinchy is the brain that decides what to do next. You can take over at any"
keywords: "minecraft, pinchymc, mc, mod, fabric, play minecraft, play with me, server, survival, mine, mining, craft, crafting, smelt, furnace, chest, loot, barrel, build, building, fight, pvp, mobs, follow me, pathfinding, pairing code, pair, prism launcher, mods folder, jar, K key, J key, take control"
permalink: /pinchymc/
---
# PinchyMC: Pinchy plays Minecraft with you

PinchyMC is a small Minecraft mod that lets Pinchy play in your game: walk somewhere, follow you, mine, craft, build, fight, use chests and chat. The mod does the fast part (finding a path, aiming, clicking at a human pace); Pinchy is the brain that decides what to do next. You can take over at any moment by simply playing.

## What to ask for
- "Pair with Minecraft, the code is 482 913."
- "What's in my inventory, and what could I craft with it?"
- "Follow me and fight whatever attacks us."
- "Go to 120 64 -30 and mine the iron ore there."
- "Craft me an iron pickaxe." He works out the steps himself: logs to planks, planks to sticks, raw iron through the furnace, then the pickaxe.
- "Build a 5 by 5 cobblestone hut here with a door."
- "What's in that chest? Take the iron and five bread, and put the cobblestone in."
- "Stop." (or press K in the game)

## Setting it up
1. Open the PinchyMC page in Settings and switch it on.
2. Get the mod: press *Put it here* next to your Fabric instance (Pinchy downloads the mod from his own release page, checks it, and puts it into that mods folder), or save the file and add it yourself. The instance needs Minecraft 26.3, the Fabric loader and Fabric API.
3. Start Minecraft, join a world, and type `/pinchymc pair` in the game chat. It shows a 6-digit code that works once, for five minutes. Only you see it.
4. Type the code into the PinchyMC page, or just tell Pinchy the code. He keeps the connection key encrypted; you never copy or paste anything.

The status pill then says **MC connected**.

## How it works
- The mod runs inside your own Minecraft and listens only on this computer. Nothing is installed on a server, and nothing leaves your computer except what the game itself sends.
- Pinchy sees the game as facts (position, health, inventory, blocks and creatures nearby, chat, what just happened) and gives the mod one job at a time: go there, follow, attack, mine these blocks, build this, craft that, use this item.
- Every job ends with what really happened. A job that did not work says why in plain words, for example "cannot craft 1 x iron pickaxe: missing 2 x raw iron" or "needs a crafting table within reach", so Pinchy can fix it instead of guessing.
- Crafting, smelting and chests go through the game's own inventory slots, not through mouse positions, and the inventory is read again after every step: he tells you what really moved and what did not fit.
- Everything happens at a human pace: turns are smooth, clicks have a human rhythm.

## You stay in control
- **K** stops whatever PinchyMC is doing. **J** pauses it until you press J again. Both keys can be changed in Minecraft under Options, Controls, Key Binds, PinchyMC.
- Moving, clicking, turning the mouse or opening a menu also stops him straight away. He waits a moment before he tries again.
- Saying something in the game chat as you needs your yes first, because everyone on the server reads it.

## Settings
- Settings → Add-ons → PinchyMC: the switch, getting the mod into an instance, the pairing code, unpair.
- Settings → Add-ons → Extensions: the PinchyMC extension's own page (what it may do and why, the bridge port).
- In the game: `/pinchymc pair` (a new code), `/pinchymc pause`, `/pinchymc selftest` (walks you forward for five seconds to show the mod has control), `/pinchymc token reset` (forget every pairing).

## Limits
- Minecraft Java Edition 26.3 with Fabric only. Other versions and Bedrock are not supported.
- PinchyMC is off until you switch it on, and it only plays through your own game while that game is running.
- Use it in your own worlds and on servers that allow helper mods. Many public servers forbid automated play; that is their rule to make, and Pinchy does not hide what he is.
- Crafting knows the survival basics (wood, sticks, tools, torches, chest, furnace, armour, beds, doors, bow and arrows, bread, smelting ores, sand and food). For anything else he says that he knows no recipe for it.
- Crafting does not walk or place blocks by itself: a crafting table or furnace has to be within reach, and Pinchy places one with a build job when he needs it.
- One job runs at a time, and he reacts to what the game reports every moment, not to the picture on the screen.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
