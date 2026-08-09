---
layout: page
title: Real-Time Speech Interpreter and Meeting Intelligence
permalink: /projects/realtime-speech-translation/
group: Product Development
order: 3
context: Live multilingual events and post-meeting intelligence
summary: Architected a bidirectional Arabic-English speech interpreter delivering live transcription, translation, and synthesized headset audio for high-profile events, with operator and audience displays, later extended into speaker-attributed meeting records, summaries, decisions, and action items.
tech: [Azure Speech, Real-Time Translation, Speaker Diarization, PyQt]
---

### Problem

High-profile multilingual events required simultaneous Arabic-English transcription and translation, with spoken output for headset users and latency low enough to follow live speeches. The system also needed to operate continuously across multiple presenters while providing professional audience displays and reliable operator controls.

Government organizations later needed the same speech foundation extended into speaker-attributed meeting records, summaries, decisions, and action items.

### My role

Architect and lead developer of the end-to-end system, responsible for service selection, speech-pipeline implementation, desktop interfaces, Windows packaging, comparative evaluation, client requirements, on-site installation, and live operation.

I also developed the meeting-intelligence extension and later led early productization planning with cloud-platform and Microsoft architecture teams.

### Approach

Built a bidirectional Arabic-English pipeline using the Azure Speech SDK and `SpeechTranslationConfig`. Continuous-recognition events produced interim transcription and translation results as speech occurred, followed by corrected final results at the end of each utterance. Azure neural text-to-speech generated translated audio with minimal latency.

Developed two audience presentation modes:

- Real-time subtitles displaying live transcription and translation
- "Cinematic subtitles" synchronizing translated speech with word-level highlighting during playback

A PyQt desktop application provided a dedicated operator console and separate audience-facing windows. Operators could manage source and target languages, microphones and mixer inputs, synthesized voices, audio outputs, playback speed, segmentation, typography, colors, opacity, scrolling, fading, and placement across multiple monitors.

The application was packaged as a standalone Windows executable with a professional installer and time-limited license management for controlled deployments.

Independent bilingual reviewers compared the system against two alternative implementations across transcription accuracy, translation quality, latency, speech intelligibility, bidirectional Arabic-English performance, and stability during extended speech. My implementation received the strongest overall evaluation and was selected for live use.

The platform was later extended with batch transcription and speaker diarization for meeting intelligence. It retained original recordings and transcripts while using an Azure-hosted LLM to refine transcription, generate executive summaries, identify decisions, extract action items and owners, organize discussion topics, and produce template-based Word and PDF reports.

### Outcome

Successfully operated for four continuous hours during a high-profile multilingual event involving multiple presenters. Following its initial success, the system garnered interest and was reused across additional government events and high-level delegations.

The meeting-intelligence extension entered immediate production use across multiple government organizations and remains in ongoing operation. Its adoption helped secure an approximately $3 million client engagement and led to an ongoing effort to productize the platform as an Azure-native, subscription or usage-based offering.

### Technologies

Azure AI Speech, Azure Speech SDK, Speech Translation, continuous speech recognition, neural machine translation, neural text-to-speech, batch transcription, speaker diarization, Azure-hosted LLMs, Python, PyQt, real-time streaming, Windows application packaging, human evaluation.
