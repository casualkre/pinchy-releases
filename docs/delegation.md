---
title: "Delegation: which model does what, what takes over, what a model may do"
description: "Pinchy can hand work to cheaper models and keep the strongest for what needs it. You pick how in a delegation profile. Fallbacks say who takes over when a model can't run, caps stop a paid key at a monthly amount, and limits take tools away from a model."
keywords: "delegation, delegate, profile, balanced, smartest, saver, fallback, usage ran out, plan used up, monthly cap, spending, budget, limits, no cli, no browser, no vault, which model, cheaper model, api key, local model"
permalink: /delegation/
---
# Delegation: which model does what, what takes over, what a model may do

Pinchy can hand work to cheaper models and keep the strongest for what needs it. You pick how in a delegation profile. Fallbacks say who takes over when a model can't run, caps stop a paid key at a monthly amount, and limits take tools away from a model.

## What to ask for
- "Who takes over when my plan runs out?" He reads you the fallback list.
- "Use the strongest model for everything." Pick the profile Smartest always in Settings.
- "Which delegation profile is on?" He tells you and what it does.
- "How much did my OpenAI key cost this month?" He reads you the month so far.

## How it works
- Profiles: Balanced is the default. Planning, checking and hard parts go to a strong model, normal building to a mid model, short messages and lookups to a small one, and anything that failed once to a strong one. Smartest always runs everything on your own model. Saver uses the smallest model that can do the job. You can write your own, with a description the model reads, and pick a model per kind of work. An agent can have its own profile.
- Your pick wins. The chat stays on the model you chose. A model you pick for one job or agent stays that model. A live conversation is never moved down to a smaller model, that would cost more than it saves.
- A profile never moves work onto a paid API key by itself. It stays on the road you are on, or a free one.
- Fallbacks: when a model can't run (the plan is used up, a login stopped working, a model was refused, a monthly cap is reached, a server stays down) the next one in your list takes over with a short recap of the chat. A busy server is waited out first. With no list set, your other CLIs and your local models take over, automatically. You see a notice each time, and the chat goes back to its first model as soon as that one can run again.
- With no list set, a local model only falls back to other local models, so nothing leaves your machine by itself, and a CLI that can't stop and ask you first is left out. Add them to your list if you want them.
- A model you pick yourself always gets to try, even if it failed a while ago.
- Paid fallback is off until you turn it on. Then every switch to a paid model shows a notice.
- A CLI fallback runs on whatever that CLI is set up with. If that is a paid key, it is charged there, and Pinchy's cap can't see it.
- Monthly caps: one dollar amount per provider. You get a notice at 80%. At 100% that provider stops and a fallback takes over. The laptop and the away server count towards the same cap. A model with no known price is counted as a call that couldn't be priced, the cap can't see those.
- Limits: take categories away from a model, a provider or a kind, for example all local models no terminal commands and no vault, or all OpenAI models no browser, also through a router. A krill or swarm a limited model starts keeps its limits.

## Settings
- Settings → Brain → Models: profiles, fallbacks, paid fallback, monthly caps, limits, and a test that shows where a kind of work would go.
- Pinchy and agents can't change these. Only your Settings window can.

## Limits
- Limits are enforced for local models and API keys. A CLI harness (Claude Code, Codex and others) runs its own tools, so there a limit is only an instruction in its system prompt. The vault is the exception: it refuses a blocked model on every engine.
- When an engine changes, the new model gets a recap of the chat, not the whole conversation.
- Background chores such as memory notes and the regular check keep their own model settings.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
