---
title: "API keys and local models"
description: "Pinchy can think with any API key or a model running on your own computer, next to Claude Code or instead of it. Everything you connect shows up in every model menu."
keywords: "api key, api keys, openai, gemini, openrouter, anthropic api, deepseek, local model, local models, ollama, lm studio, llama.cpp, lean mode, fast mode, context size, own model, other model, no claude, grok"
permalink: /api-keys-and-local-models/
---
# API keys and local models

Pinchy can think with any API key or a model running on your own computer, next to Claude Code or instead of it. Everything you connect shows up in every model menu.

## What to ask for
- "Which models do I have connected?" He lists them by source.
- "Use my Ollama model for this chat." Say the model and he switches, if it is connected.
- "Why is my local model slow?" He looks at its size and the context size you gave it.

## How it works
- Settings → Brain → Models → Where your models come from. Pick a provider and paste a key, or pick a running local server and press Use it. Anything not listed works through Something else: paste any OpenAI-style or Anthropic-style address.
- Local tab: Pinchy looks for Ollama, LM Studio, llama.cpp, Jan and others on this computer. A server on another computer works too.
- API keys are sealed by your system keyring and never appear in a chat, a log or a transcript. Pinchy and his agents can't read a key or change where it is sent; only you can, in Settings. If your computer has no keyring the page says so and the key sits in a private file instead.
- Lean mode: a small model gets a short prompt and a few tools, and finds the rest by searching. It is on for local models because Pinchy's full first turn is too much for them: on a test model it took about 900 tokens instead of 7,500. His memory stays reachable through his tools.
- Context size (local models): how much the model can hold in mind. Bigger uses more memory.
- Fast mode (Anthropic key only): the same model, faster, at twice the price per token. It works on Opus 5.5, Opus 5 and Opus 4.8. When fast mode is rate limited, that request runs at normal speed and the chat says so.
- On my away server: copies that key to your away server so agents there can use those models. It shows once a server is paired. The key is hidden from the agents, but it does leave this computer.

## Good to know
- The models Pinchy can use depend on what the provider gives your key; new ones appear by themselves within a day.
- With a router like OpenRouter some models can reach companies Pinchy doesn't allow, so those are filtered out, and a run stops if a router lands on one anyway.
- On an Anthropic key, if a safety check refuses a request on Fable 5.1, Opus 5.5, Opus 5 or Sonnet 5.5, Anthropic reruns it on another model and the chat says which.
- Spending numbers come from each provider's price list. A model with no known price shows as price unknown, not as free.
- Grok is banned. No Grok models, no xAI or SpaceX AI keys or addresses, through any road.
- Limits, spending caps and fallbacks are on the Delegation page: see Delegation.

## Settings
Settings → Brain → Models.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
