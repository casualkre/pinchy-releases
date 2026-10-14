---
title: "Model and plan usage: which Claude he uses and how much of your plan"
description: "Pinchy runs on your Claude plan. You choose the model he thinks with and how careful he is with your usage."
keywords: "model, opus, sonnet, haiku, fable, plan, usage, quota, limit, tokens, cost, cheaper, faster, slow, new chat, reset chat, usage level, quota saver"
permalink: /model-and-usage/
---
# Model and plan usage: which Claude he uses and how much of your plan

Pinchy runs on your Claude plan. You choose the model he thinks with and how careful he is with your usage.

## What to ask for
- "Use Haiku for chats." He switches the chat model.
- "How much of my plan is left?" He tells you the 5-hour and weekly usage.
- "Use less of my plan." He explains the usage levels and switches when you say which.
- "Why did you just switch models?" When your plan is nearly used up, the quota saver moved the chat to a cheaper model; he says so.

## How it works
- Model: one setting for chats. Work, Code, agents and swarms have their own model settings.
- Usage level: Full quality, Balanced or Saver. Every level loads his rarely used tools only when he needs them. Balanced and Saver also carry less of his memory in every message and look older chats up when they matter.
- Quota saver: when the 5-hour window is nearly used up (85% by default), the chat moves to a cheaper model, answers get shorter and agents that run on a schedule wait. Reminders and anything marked essential still run.
- A new chat starts by itself when the bubble has been closed for a while (2 minutes by default), so an old conversation does not ride along forever. The key points of your last chats are remembered.
- He does not carry a manual of himself in every message. When you ask how something works or where a setting is, he looks it up in these docs.

## Settings
- Settings → Brain → Claude: the model, the usage level, when a fresh chat starts, keep Pinchy ready to answer, messages while he works change the job, the quota saver and its threshold, the chat model while saving quota.
- Settings → Brain → Claude → Permissions: how much he may do in chats and in an agent's scheduled runs without asking.
- Settings → Brain → Claude → Claude Code on this computer: also load the tool servers you use in Claude Code (off by default), where the claude program is.

## Limits
- "Keep Pinchy ready to answer" keeps one Claude process waiting while the chat is open (about 230 MB of memory) so the first answer comes sooner.
- Usage numbers come from your Claude plan and are shared with everything else you do on that plan.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
