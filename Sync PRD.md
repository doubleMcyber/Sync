\# Product Requirements Document (PRD)  
\#\# Product Name: Sync (working name)  
\#\# Platform: Web (Desktop-first)  
\#\# Version: MVP v1  
\#\# Status: Definition Complete

\---

\#\# 1\. Overview

\#\#\# Product Summary  
\*\*Sync\*\* is a calm, ambient study companion that displays a personalized lo-fi video loop of an idealized version of the user studying. It provides \*\*silent accountability\*\* through presence rather than metrics, using subtle visual metaphors instead of explicit timers or gamification.

Users open Sync \*before\* studying to “sync” into focus. The app remains present while they work, either fullscreen or in picture-in-picture mode.

\---

\#\# 2\. Problem Statement

Most productivity tools:  
\- Interrupt focus with timers, numbers, notifications, and guilt  
\- Require planning, tracking, or active engagement  
\- Treat productivity as something to optimize rather than inhabit

Users who already \*want\* to work need:  
\- A sense of presence  
\- Gentle accountability  
\- A calm ritual that makes starting easier and staying natural

\---

\#\# 3\. Product Vision & Thesis

\#\#\# One-Sentence Thesis  
\> People focus better when they feel quietly accompanied by an ideal version of themselves, not monitored by tools.

\#\#\# Design Philosophy  
\- Presence over productivity  
\- Metaphor over metrics  
\- Silence over instruction  
\- Identity over optimization

This is \*\*not\*\* a task manager, habit tracker, or coaching system.

\---

\#\# 4\. Goals & Non-Goals

\#\#\# Goals  
\- Create a calm, immersive study environment  
\- Encourage longer focus sessions without explicit pressure  
\- Feel like a \*presence\* rather than an app  
\- Require near-zero interaction during use

\#\#\# Non-Goals (Explicit)  
\- ❌ Task management  
\- ❌ Calendar planning  
\- ❌ Streaks or gamification  
\- ❌ Notifications or reminders  
\- ❌ AI coaching or chat  
\- ❌ Emotional analysis or feedback

\---

\#\# 5\. Target User

\#\#\# Primary User  
\- Students, creators, or knowledge workers  
\- Already motivated but struggle with starting or sustaining focus  
\- Uses lo-fi videos, ambient music, or body-doubling for focus  
\- Values aesthetics, calm, and minimalism

\#\#\# User Mindset  
\> “I don’t need another system. I just want to lock in.”

\---

\#\# 6\. Core User Experience

\#\#\# Primary Flow  
1\. User opens Sync  
2\. A personalized lo-fi study video begins playing  
3\. User enters fullscreen or PiP  
4\. User studies alongside their avatar  
5\. Optional: start a silent pomodoro via visual metaphor  
6\. User closes Sync when finished

No onboarding tutorial required beyond a single setup screen.

\---

\#\# 7\. Core Features (MVP Scope)

\#\#\# 7.1 Personalized Lo-Fi Video Loop (Core)

\*\*Description\*\*  
\- A looping video scene depicting a stylized version of the user studying  
\- No eye contact with the viewer  
\- Subtle, continuous motion (writing, sipping, posture shifts)

\*\*Requirements\*\*  
\- Seamless loop (10–30s)  
\- Full-bleed background  
\- Day and/or night variants (optional for MVP)  
\- Video stored and played locally

\---

\#\#\# 7.2 Display Modes

\#\#\#\# Fullscreen Mode  
\- Looks like a YouTube lo-fi stream  
\- No visible UI by default  
\- Controls appear only on hover

\#\#\#\# Picture-in-Picture (PiP)  
\- Miniaturized version of the same video  
\- No overlays  
\- Sits quietly in corner of screen

\---

\#\#\# 7.3 Silent Pomodoro via Visual Metaphor

\*\*Concept\*\*    
Time is represented by a translucent mug in the scene, not by numbers.

\*\*Behavior\*\*  
\- When a session starts:  
  \- Mug begins full  
  \- Avatar sips periodically  
  \- Liquid level lowers over time  
\- At end of work session:  
  \- Mug empty  
  \- Avatar stands and leaves to refill (break)  
\- During break:  
  \- Avatar is absent or idle

\*\*Flow Extension\*\*  
\- User can “pour more” (add time) without breaking immersion  
\- No numeric countdown displayed by default

\*\*Implementation (MVP)\*\*  
\- Video swapping between pre-rendered clips  
\- Smooth crossfade transitions  
\- Timer logic exists but UI is hidden

\---

\#\#\# 7.4 Audio (Optional)

\- Default: silence  
\- Optional: curated lo-fi audio loop  
\- Independent volume control  
\- Audio continues across video transitions

No third-party streaming integrations in MVP.

\---

\#\#\# 7.5 Weekly Reflection (Optional / Lite)

\- Passive summary (opt-in)  
\- Example:  
  \- “You synced for \~7.5 hours this week.”  
\- No charts, streaks, or rankings  
\- Presented as reflection, not performance

\---

\#\# 8\. UX & UI Principles

\- No visible timers by default  
\- No text overlays during focus  
\- No popups or interruptions  
\- UI elements hidden unless intentionally summoned  
\- Aesthetic \> efficiency

\---

\#\# 9\. Technical Requirements

\#\#\# Platform  
\- Web (Desktop-first)  
\- Chrome, Safari, Edge support  
\- Mobile support not required for MVP

\#\#\# Core Tech  
\- React (Next.js or Vite)  
\- HTML5 \`\<video\>\` for playback  
\- Picture-in-Picture API  
\- LocalStorage / IndexedDB for preferences

\#\#\# Performance  
\- Videos must preload before switching  
\- No visible black frames during transitions  
\- App should run smoothly for multi-hour sessions

\---

\#\# 10\. Privacy & Trust

\- User images/videos stored locally only  
\- No uploads to servers  
\- No biometric analysis  
\- No background data collection

Privacy stance should be stated clearly in:  
\- Terms of Service  
\- PRD  
\- Landing page copy

\---

\#\# 11\. Out of Scope (Future Possibilities)

\- Automated avatar generation  
\- AI animation synthesis  
\- Native desktop app (always-on-top)  
\- Time-aware environments (real-time day/night sync)  
\- Multiple avatar “modes”  
\- Shared or social features

These are explicitly \*\*not MVP\*\*.

\---

\#\# 12\. Success Metrics (Qualitative)

Because this is a presence-based product, success is measured differently.

\#\#\# MVP Success Looks Like:  
\- User voluntarily opens Sync before studying  
\- Sessions last longer than baseline  
\- App is left open without interaction  
\- User reports feeling “less alone” or “more locked in”

Quantitative metrics are secondary.

\---

\#\# 13\. Risks & Mitigations

\#\#\# Risk: Feels like “just a video”  
\*\*Mitigation:\*\*    
Lean hard into personalization \+ metaphor \+ PiP presence

\#\#\# Risk: Feature creep into productivity app  
\*\*Mitigation:\*\*    
Strict adherence to Non-Goals section

\#\#\# Risk: Distraction from avatar  
\*\*Mitigation:\*\*    
Minimal motion, no eye contact, no expressive emotion

\---

\#\# 14\. MVP Definition (One-Line)

\> A web app that plays a personalized, looping lo-fi study video with optional silent pomodoro mechanics, designed to function as a calm study presence rather than a productivity tool.  
