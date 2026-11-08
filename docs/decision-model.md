---
title: "The decision model"
description: "A small model on your own computer (tev1, through Ollama) that answers quick closed questions in about a tenth of a second, with no usage spent: yes or no, pick one of a few options, or a score. Pinchy, his agents and krill use it where a full model turn would be slow or wasteful. It is fast but not"
keywords: "decision model, tev, tev1, tev_decide, nimble, smart watcher, quick decision, is the page loaded, screen ready, stuck, waiting for input, delegation kind, ollama systemone, opt out"
permalink: /decision-model/
---
# The decision model

A small model on your own computer (tev1, through Ollama) that answers quick closed questions in about a tenth of a second, with no usage spent: yes or no, pick one of a few options, or a score. Pinchy, his agents and krill use it where a full model turn would be slow or wasteful. It is fast but not clever, so it only acts when it is sure. When it isn't, the big model decides as before.

## What to ask for
- "Is the decision model working?" He checks which model answers, how fast, and how often it was sure.
- "Tell me when the build log says it failed." He can set up a smart watch: the decision model reads the log and the watch fires when it is sure it failed, twice in a row. No regex, no usage.
- "Why did my krill go to a smaller model?" When a job's title alone didn't say what kind of work it is, the decision model named it (lookup, docs, building…). It only moves work to a cheaper model when it is very sure.
- "Is that agent stuck?" A run that has printed nothing for 3 minutes is read again: still working (a long download), waiting for an answer in its terminal, or stuck.

## How it works
- It needs Ollama (free, ollama.com). Pinchy never downloads a model without your click. It runs fine on a processor alone, faster with a graphics card.
- Computer use: a chain of clicks can wait for "the screen finished loading" instead of a fixed pause, and the screenshot Pinchy gets back after a page change shows the page, not a spinner.
- Safety: it can only make Pinchy more careful, never less. A risk check can add an ask, never skip one. A call check can add a call, never stop one you have to answer.
- "What it decided lately" in Settings lists its last answers, with how sure it was and how long it took.
- Tool for every model: tev_decide. Give it a piece of text and one short question, and act only on a sure answer.

## How a smart watch is set up (for Pinchy and his agents)
- First a variable that holds the text to judge (a log file, a page, a command's output), then a second one that judges it: `vars_define {name:"build.verdict", source:{type:"decide", params:{from:"build.log", question:"How did this build end?", options:{passed:"all steps succeeded", failed:"a step failed", running:"still going"}}}}`. Leave out options for a yes/no question (value yes or no).
- Its value only changes when the decision model is sure twice in a row; a burst of changes is judged once.
- Then a normal watch on it: `vars_watch {name:"build.verdict", op:"eq", value:"failed", action:{type:"notify", …}}`. Use it to tell the human or wake Pinchy, never to do something that can't be undone on its own: the text it reads can be written by anyone.

## Settings
- Settings → Brain → Models → Decision model shows the model, your graphics card, how fast it answers and how often it was sure. If none is downloaded, Download gets the right one for your computer: tev1 4B (2.8 GB) on a graphics card with at least 4.5 GB, the small tev1 0.8B (1.6 GB) otherwise.
- Each use has its own switch: Computer use, Smart watcher, Delegation, Stuck check, Call check, Risk check. Turn off any of them, or the whole thing.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
