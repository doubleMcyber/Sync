# Sync

**Sync** is a calm, ambient study companion that helps you lock in by studying alongside an idealized, lo-fi version of yourself.

This is not a productivity app.  
There are no streaks, no notifications, and no guilt.  
Just quiet presence, subtle motion, and time felt indirectly.

---

## Why Sync Exists

Most productivity tools demand attention.

Sync does the opposite.

It creates a shared study space where focus emerges naturally—through ritual, presence, and identity rather than metrics.

You open Sync *before* you study.  
You leave it open *while* you study.  
You close it when you’re done.

That’s it.

---

## Core Concept

- A **personalized lo-fi study loop** (video, not static)
- An **ideal version of you** studying quietly
- **Time represented visually**, not numerically
- **Silent accountability** via presence
- Fullscreen or **Picture-in-Picture** mode

Sync doesn’t tell you what to do.  
It simply stays with you while you do it.

---

## Features (MVP)

### 🎞 Personalized Study Loop
- Seamless looping lo-fi video
- Stylized avatar (no eye contact)
- Subtle, continuous motion
- Day / night variants (optional)

### ☕ Visual Pomodoro (Optional)
- No timers on screen
- A translucent mug represents time
- Mug empties as work progresses
- Avatar leaves to refill during breaks
- Extend focus by “pouring more”

### 🪟 Display Modes
- **Fullscreen**: immersive, YouTube-style
- **Picture-in-Picture**: quiet presence in the corner

### 🎧 Audio (Optional)
- Default: silence
- Optional curated lo-fi loop
- Independent volume control

### 📊 Reflection (Optional)
- Weekly, passive summary
- No charts, streaks, or rankings
- Reflection over performance

---

## What Sync Is *Not*

- ❌ Task manager  
- ❌ Calendar  
- ❌ Habit tracker  
- ❌ Coaching system  
- ❌ Gamified productivity app  

If you’re looking for optimization, this isn’t it.

---

## Tech Stack

- **Frontend:** React (Next.js or Vite)
- **Media:** HTML5 `<video>`
- **Storage:** LocalStorage / IndexedDB
- **APIs:** Picture-in-Picture
- **Platform:** Web (Desktop-first)

All media is stored and played **locally**.

---

## Getting Started (Local Development)

```bash
# Clone the repo
git clone https://github.com/your-username/sync.git
cd sync

# Install dependencies
npm install

# Run locally
npm run dev
