---
title: Crosstalk — AI disclosure
version: 0.4.0-draft
effective_date: TBD
status: draft, not in force
---
# Crosstalk — AI disclosure

> Draft for review. Not in force until Fedor AB publishes it with an effective date.

## What Crosstalk tells you

The hosts you hear on Crosstalk are not real people. An AI language model writes what they say, and an AI speech system produces their voices. Nobody records, reviews or edits a host segment before you hear it.

Because the hosts are generated, what they say about an artist, a song, the date or the weather can be wrong. Treat it as entertainment, not as a source of facts.

The music is different. Crosstalk plays your own Apple Music through your own subscription, and it does not generate or change the music.

## Where the app says so

The app tells you that the hosts are AI on the screen that asks for your permission, before the first host segment plays. In Settings, the switch for the hosts is labelled "AI Hosts".

## Marking inside the audio

Every host segment is also marked as AI-generated in two ways that software can read:

- **A watermark in the sound itself.** The hosts' voices are produced by Google's Gemini speech models, and Google embeds its SynthID watermark in the audio they generate.
- **A label in the audio file.** Crosstalk writes an "AI-generated" statement into the metadata of each audio file it delivers to the app. The app plays that file and does not hand it out.

**How to check a segment.** If you have a file with a Crosstalk host segment, you can check it with Google's SynthID Detector (synthid.com). The detector accepts audio files; it asks you to sign in and to accept Google's terms. It reports that the audio was made with Google's AI; it does not name Crosstalk. In November 2026 we checked host segments as Crosstalk delivers them, and re-encoded copies of them, and the detector found the watermark in each. We have not tested a screen recording or a recording made through a microphone.
