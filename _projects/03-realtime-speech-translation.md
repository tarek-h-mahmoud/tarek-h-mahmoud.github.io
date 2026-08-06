---
layout: page
title: Real-Time Multilingual Speech Translation
permalink: /projects/realtime-speech-translation/
group: Product Development
order: 3
context: Live multilingual events and post-meeting intelligence
summary: Architected and delivered a real-time, multi-speaker translation system combining speech recognition, diarization, machine translation, and text-to-speech. Built on Azure Speech Services for live multilingual events and post-meeting intelligence.
tech: [Azure Speech Services, ASR, Diarization, TTS]
---

### Problem

Live multilingual events needed spoken translation in real time, with production-grade reliability and latency low enough to follow a conversation as it happens.

### My role

Architect and implementer of the end-to-end system, including benchmarking against an alternate internal implementation.

### Approach

A streaming pipeline chaining speech recognition, speaker diarization, machine translation, and text-to-speech, built on Azure Speech Services and driven through a desktop interface for live operation. The architecture was designed around a strict latency budget and evaluated comparatively against an internal alternative. The same pipeline supports post-meeting intelligence over recorded sessions.

### Outcome

Ran continuously for hours during live multilingual events.

### Technologies

Azure Speech Services, streaming ASR, speaker diarization, machine translation, text-to-speech, Python, Qt.
