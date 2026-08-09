---
layout: page
title: Real-Time Speech Interpreter and Meeting Intelligence
permalink: /projects/realtime-speech-translation/
group: Product Development
order: 3
context: Live multilingual events and post-meeting intelligence
summary: Architected a multilingual streaming speech interpreter delivering live transcription, translation, and synthesized interpretation for high-profile events, with operator and audience displays, later extended into speaker-attributed meeting records, summaries, decisions, and action items.
tech: [Azure Speech, Real-Time Translation, Speaker Diarization, PyQt]
---

### Problem

High-profile multilingual events required real-time transcription, translation, and spoken interpretation with sufficiently low latency to follow live speeches. The system also needed to run continuously across multiple presenters while providing professional audience displays and reliable operator controls.

Government organizations later needed the same speech platform extended into speaker-attributed meeting records, summaries, decisions, and action items.

### My role

Architect and lead developer of the end-to-end platform, responsible for:

- Speech and translation architecture
- Desktop application and audience interfaces
- Windows packaging and license management
- Independent comparative evaluation
- Client requirements and on-site installation
- Live event operation
- Meeting-intelligence extension
- Azure-native productization planning

### Approach

#### Live Speech Interpreter

Built a configurable multilingual streaming pipeline using Azure AI Speech:

- Generated interim transcription and translation results as speech occurred, followed by corrected final results
- Produced synthesized translated speech with minimal additional latency
- Supported continuous operation across multiple presenters and extended speaking sessions
- Maintained separate input, output, voice, playback, and language controls

Developed two audience presentation modes:

- Real-time subtitles: Continuously displayed live transcription and translation
- Cinematic subtitles: Synchronized translated speech with word-level highlighting during playback

A PyQt operator console controlled microphones, mixer inputs, synthesized voices, audio outputs, playback speed, segmentation, typography, colors, opacity, scrolling, fading, and audience-window placement across multiple monitors.

The application was distributed as a standalone Windows executable with a professional installer and time-limited licensing.

Independent human reviewers compared the system with two competing implementations across transcription accuracy, translation quality, latency, speech intelligibility, and stability during extended operation. My implementation received the strongest overall evaluation and was selected for live use.

#### Meeting Intelligence

Extended the platform with batch transcription, speaker diarization, and LLM-powered meeting analysis:

- Preserved original recordings and transcripts
- Produced refined, speaker-attributed transcripts
- Generated executive summaries and discussion topics
- Identified decisions, action items, owners, and follow-up requirements
- Created template-based Word and PDF reports
- Maintained searchable archives of previous meetings

### Outcome

- Successfully operated for four continuous hours during a high-profile multilingual event involving multiple presenters
- Reused across additional government events and high-level delegations
- Meeting-intelligence extension deployed across multiple government organizations and remains in ongoing use
- Helped secure an approximately $3 million client engagement
- Led to an ongoing effort to productize the platform as an Azure-native, subscription or usage-based offering

### Technologies

Azure AI Speech, Azure Speech SDK, continuous speech recognition, neural machine translation, neural text-to-speech, batch transcription, speaker diarization, Azure-hosted LLMs, Python, PyQt, real-time streaming, Windows application packaging, human evaluation.
