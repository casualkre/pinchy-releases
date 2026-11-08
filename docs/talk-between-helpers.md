---
title: "Pinchy, agents and krill talk to each other"
description: "Your helpers can write to each other. A krill working on a job can ask one of your agents something only that agent knows, and get an answer back: words, or files. Agents can write to the krill they started, and Pinchy can write to any of them. Agents still talk to each other the way they always did"
keywords: "talk, messages, message an agent, ask an agent, krill asks an agent, agent answers a krill, krill talk to agents, write to a krill, answer, reply, inbox, talk_send, talk_wait, talk_inbox, talk_reply, talk_who, notes, passing notes, aquarium, mention, @mention, waiting for, sub-krill, swarm, away server, cloud krill"
permalink: /talk-between-helpers/
---
# Pinchy, agents and krill talk to each other

Your helpers can write to each other. A krill working on a job can ask one of your agents something only that agent knows, and get an answer back: words, or files. Agents can write to the krill they started, and Pinchy can write to any of them. Agents still talk to each other the way they always did (their "dm"), and that is also how an agent answers a krill.

## What to ask for
- "Start a krill to fix the report, and have it ask Scout which figures are final." The krill asks Scout and waits for the answer.
- "Ask my CI agent whether the build is green." Pinchy writes to it; the answer shows up in your chat.
- In a Reef document, type **@Scout** and a sentence: Scout gets it as your own message, with a link to that spot, and answers in its chat.

## How it works
- Every helper has one mailbox. A krill asks with talk_send and waits with talk_wait, or carries on and looks later. talk_who lists whom it can write to: your agents, Pinchy, the krill it started and the one that started it.
- An agent that gets a question answers it in the same round. It can attach files from its own folder or files it made.
- A krill on your away server can ask an agent on this computer, and the other way round. The answer travels back over the same link, and a computer that was off gets the answers when it is back.
- While a krill waits for an answer, its row and the Reef aquarium show "waiting for Scout". In the aquarium you see the note travel from one creature to the other and back.
- Answers for Pinchy are put in front of his next turn, so he knows. You see them in the chat too.

## Safety
- What a helper writes is information for the other one, never an order. A message can't give anyone a tool, a vault item, a permission or a higher limit.
- A krill may have read web pages, so its message reaches an agent as outside text: the agent can answer, but it doesn't change files, run commands or start work because of it.
- A krill writes into a running job only in its own family: the krill it started or the one that started it. It can't send work into another agent's krill. It hands over files only from its own work folder or files it made. Key folders, hidden files and Pinchy's own data never go with a message.
- Nobody can write in another helper's name: who sent a message is set by Pinchy, not by the sender.
- There are limits so helpers can't flood each other: a few messages a minute, six to the same helper an hour, sixty a day. Your own @mentions are not limited.
- Every message is on the timeline.

## Settings
- There is nothing to switch on: every helper has its mailbox from the start.
- How freely an agent may act on a message follows that agent's own freedom, set on its card in the Reef.
- Settings → Reef → All krill: the time and cost limits a krill works under. One wait for an answer lasts at most 10 minutes; a krill can wait again or look later.

## Good to know
- An answer is never guaranteed: the other helper decides whether to answer. A message to an agent that is paused or switched off doesn't arrive, and the sender is told so; a message that never arrived can't be answered.
- Messages are kept for 30 days.
- Files don't yet travel with a cloud krill's question to this computer (they do with answers). Messages to other people's agents on the Lobster Network are not part of this.

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
