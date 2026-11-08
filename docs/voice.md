---
title: "Voice: talking to Pinchy and hearing him answer"
description: "You can talk to Pinchy instead of typing, and he can answer out loud. Speech is recognised on your computer; nothing you say is sent anywhere."
keywords: "voice, voices, microphone, mic, speak, talk, wake word, hey pinchy, push to talk, PTT, dictation, speech, whisper, read aloud, text to speech, TTS, hands free, humotranslator, accent, british, describe a voice, custom voice, emotion, qwen, agent voice"
permalink: /voice/
---
# Voice: talking to Pinchy and hearing him answer

You can talk to Pinchy instead of typing, and he can answer out loud. Speech is recognised on your computer; nothing you say is sent anywhere.

## What to ask for
- Say "Hey Pinchy, open my Downloads folder" with Hey Pinchy switched on.
- Hold the push to talk key, say "remind me in ten minutes to call Ada", let go.
- Press the microphone in the chat (or Ctrl+D) and dictate a long message.
- "Answer me out loud from now on." He switches his voice on.
- "Stop talking." He switches it off again.
- "Say it like you're excited." He, your agents and krill can speak happy, calm, serious, whispering…
- New voices are made in Settings → Voice & writing → Humotranslator → Describe a new voice (he points you there if you ask in the chat).

## The four ways
- **Hey Pinchy**: say his name and your question in one breath ("Hey Pinchy, what time is it"), hands free. He hears you out and it is sent when you stop talking; say only his name and nothing happens. If you would rather read your words before they are sent, choose "Your words go into the chat box" in the settings. A mic light shows while he listens. He never listens while the screen is locked, and not to himself while he is speaking. You can change the words he listens for.
- **Push to talk**: hold a key, speak, let go. A quick tap keeps listening until you pause. What you say can go to Pinchy as a question, or be typed for you into the app you are in. With Hey Pinchy on, the microphone is already open, so nothing is cut off at the start.
- **Dictation**: the microphone button in the chat turns speech into text you can edit before sending.
- **The Humotranslator (his voice)**: Pinchy is a lobster, so he clicks — the Humotranslator, the little box he holds up while he answers, says it out loud in a human voice, either only when you talked to him or always. Its meter and sound waves move with what is being said. While it speaks, little bubbles come out of his mouth with every syllable and go into the box's horn: he talks lobster, the box turns it into words. An agent or a krill that speaks in its own voice holds its own box — on your desktop and in the Reef's aquarium. He starts speaking while he is still writing (a "still digging…" line is heard when it happens, then the answer), reads the whole answer, and says code or a table in one short line instead of reading it out. Words a voice gets wrong are said the way people say them ("jay-son" for JSON). He stops the moment you start talking.
- **Voices**: pick Pinchy's voice from the built-in ones (British, Scottish, Australian, Narrator, Sea captain, Grandma…) or describe a new one in your own words. Your words are turned into a detailed description, the voice is made once and then copied exactly, so it sounds the same every time. Every voice can sound happy, excited, calm, serious, sad, whispering or urgent: he, your agents and krill pick the mood that fits what they say. Agents and krill speak with their own voice, so you can tell who is talking.

## How it works
- A small speech model runs on this computer. It is downloaded once (about 57 MB) the first time you switch a voice feature on; the recording is deleted right after it is turned into text.
- The Humotranslator's voices also run on this computer (Qwen3-TTS, a voice model running in a fast C++ engine). It is a one-time download of about 1.2 GB (Settings → Voice & writing → Humotranslator → Voice quality: Standard; "Best" adds 2 GB and needs a fast graphics card). It runs on your graphics card when it can, otherwise on the processor. For now it runs on Linux; Windows and macOS use the light voice or the system voice. Making a new voice from a description downloads the voice designer once (about 1.9 GB) and takes a few minutes. On a slow computer, "Light voice" uses a small 90 MB voice instead; macOS without the download uses its own voice.

## Settings
- Settings → Voice & writing → Hey Pinchy: switch it on, the words he listens for, what happens after you say his name (he answers, or your words go into the chat box), which model listens, test the wake word, remove the model.
- Settings → Voice & writing → Push to talk: switch it on, the key to hold, ask Pinchy or type it for me, quick tap to keep listening, the longest take.
- Settings → Voice & writing → Dictation: speech model (Base, Small, Best accuracy), language, show words while I talk.
- Settings → Voice & writing → Humotranslator: answer out loud (Off, When I talk to him, Always), the voices (play one, "Use for Pinchy", describe a new voice, remove the ones you made), keep listening after he answers, and the light voice for slow computers.
- An agent's voice: the agent's settings in the Agents hub.
- When answering out loud is on, what an agent or a krill tells you is read out in its own voice, one at a time. Settings → Voice & writing → Humotranslator → "Agents and krill speak too" turns that off alone.
- In the Agents window, the small speaker under an agent's message reads that message to you in its voice.
- Settings → Pinchy → Shortcuts: every shortcut in one place, including push to talk.
- Settings → Safety & data → Check everything: tests the microphone and the shortcuts and offers a fix.

## Limits
- Hey Pinchy and push to talk are off until you switch them on.
- Agents and krill never speak out loud during your quiet hours (Settings → Pinchy → Notifications), in Do not disturb, or when answering out loud is off; they send a message instead.
- In a loud room (a video, music, a call) he checks what he hears a little less often; he does not stop listening. If he does not react, "Check everything" says why, for example that the microphone gives no sound.
- He listens for his name in the language you dictate in. If you speak several languages, set the dictation language to the one you call him in.
- The Base model is the fastest; Best accuracy is slower and bigger. Pick the language if he mishears a language other than English.
- If a shortcut does nothing, another app may hold the same keys: change it under Shortcuts, or run "Check everything".

---

[All pages](https://casualkre.github.io/pinchy-releases/) · [Download Pinchy](https://github.com/casualkre/pinchy-releases/releases/latest)
