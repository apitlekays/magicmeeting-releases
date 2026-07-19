<div align="center">

# 🎙️ MagicMeeting

### Your meetings, transcribed and minuted — without a single byte leaving your Mac.

**Record any meeting. Get a speaker-labeled transcript, action items, and polished minutes in minutes — 100% on-device. No cloud. No account. No one listening in.**

<br/>

[![Download for macOS](https://img.shields.io/badge/Download%20for%20macOS-Universal%20App-1f6feb?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/apitlekays/magicmeeting-releases/releases/latest)

<br/>

[![Version](https://img.shields.io/github/v/release/apitlekays/magicmeeting-releases?label=latest&color=24c8db)](https://github.com/apitlekays/magicmeeting-releases/releases/latest)
[![Platform](https://img.shields.io/badge/macOS-12.3%2B%20universal-1f6feb)](#-requirements)
[![Privacy](https://img.shields.io/badge/privacy-100%25%20on--device-2ea043)](#-your-audio-never-leaves-your-mac)
[![Signed & Notarized](https://img.shields.io/badge/Apple-signed%20%2B%20notarized-lightgrey)](#-install-in-30-seconds)

</div>

---

## The meeting is over. The work of remembering it shouldn't just be beginning.

You sat through the whole thing. Now you're scrubbing a recording, guessing who said what, and rebuilding minutes from half-legible notes — while the cloud transcription service you pasted the audio into keeps a copy forever.

**MagicMeeting does all of it the moment you hit stop — and keeps every second of audio on your machine.** Hit record, and watch the transcript stream in live, already split by speaker. Fix a word, tag a decision, mark an action item, and export clean minutes to PDF or Word. That's it.

<div align="center">

### [⬇ Download the latest release →](https://github.com/apitlekays/magicmeeting-releases/releases/latest)

*Free. Signed & notarized by Apple. Opens with no Gatekeeper warning — online or offline.*

</div>

---

## 🔒 Your audio never leaves your Mac

This is the whole point. Most transcription tools ship your meetings — often confidential ones — to someone else's servers. MagicMeeting doesn't.

- **No cloud, no API, no account.** The speech models download once (checksum-verified) and everything runs locally from then on.
- **No telemetry.** We don't phone home. There's nothing to opt out of.
- **Works on a plane.** Full transcription with zero connectivity.
- **Your data stays yours.** Every recording, transcript, and note lives in a local database on your disk — under your control, deletable in one click.

If it can't leave your machine, it can't leak.

---

## ✨ What you get

### 🎙 Live recording & instant transcription
Capture your **microphone and system audio** together — perfect for calls where the other side comes through your speakers. The transcript appears as you speak, so you're never staring at a spinner after the meeting.

### 👥 Speaker labels that actually hold up
Every voice is separated automatically. **Rename a speaker once** — "Speaker 2" becomes "Aisyah" — and it updates everywhere: transcript, notes, and minutes. (More on why our speaker separation is unusually reliable [below](#-robust-by-measurement-not-by-marketing).)

### ✍️ A transcript you can actually fix
Double-click any line to correct it. **Merge** fragmented lines into one clean turn, or **split** a run-on segment where two people overlapped — non-destructively, and reflected everywhere it matters. Your edits flow straight through to notes and exports.

### 📋 Minutes & action items, ready to send
Turn decisions into tracked **action items** with owner, priority, and status, aggregated into a single Minutes-of-Meeting table that stays in sync with the transcript. Stop rewriting minutes from scratch.

### 🗂 Research-grade notes
Highlight any excerpt, tag it with a code, and attach a note — then jump from any note straight back to that exact moment in the audio. Built for people who *analyze* conversations, not just skim them.

### 📄 Export that's ready for the room
One click to **PDF** or **Word (.docx)** — transcript, minutes, or notes — with clean, reproducible output you can drop into a report or email.

### 🌊 Waveform player with click-to-seek
Scrub the recording on a rendered waveform, or click **any timestamp** in the transcript, notes, or minutes to jump there instantly.

### 📁 Already have a recording?
Point MagicMeeting at an existing audio file and get the full treatment — transcript, speakers, minutes — without recording live.

---

## 🌍 Speaks your language — ~99 of them

Every recording is transcribed on-device by a multilingual model that handles roughly **99 languages**. Pick one when you start a session, or let it **auto-detect**.

For select languages, optional **accuracy packs** swap in a specialized on-device model that beats general transcription on that language — Russian, Hindi, Bengali, Tamil, Telugu, Urdu, and more, with new packs added over time (no app update required).

> Arabic · Bahasa Malaysia · Bahasa Indonesia · Bengali · Cantonese · Mandarin · Dutch · English · French · German · Hebrew · Hindi · Italian · Japanese · Korean · Persian · Portuguese · Russian · Spanish · Swahili · Tamil · Telugu · Thai · Turkish · Ukrainian · Urdu · Vietnamese — *and many more.*

---

## 🔬 Robust by measurement, not by marketing

Anyone can wire up Whisper. The hard part is making it survive **long, real, multi-speaker meetings** — where off-the-shelf pipelines famously break in two ways: Whisper **hallucinates** phrases into silence ("thank you for watching"), and speaker diarization **collapses**, merging everyone into one person.

MagicMeeting is tuned against a **built-in evaluation harness** that replays a real **4-hour-38-minute** multilingual meeting through the exact production pipeline and scores it on real metrics — word error, character error, speaker error, and hallucination rate. Every improvement has to *prove itself on real audio* before it ships. The results:

| | Before | After |
|---|---|---|
| **Hallucinated phrases** | 2.7% | **0%** |
| **Speech attributed to the wrong speaker** | 38% | **0%** |

That second number is the one to notice. Most on-device tools cluster speakers greedily as audio streams in — and one early mistake cascades into whole-meeting collapse that can never be undone. MagicMeeting keeps every voice fingerprint and **re-clusters globally when the meeting ends**, so it can pull a collapsed cluster back apart into distinct people. Reliability you can reproduce on the audio you actually record.

---

## 🚀 Install in 30 seconds

1. **[Download the latest `.dmg`](https://github.com/apitlekays/magicmeeting-releases/releases/latest)** — one universal build runs natively on Apple Silicon **and** Intel.
2. Open it and drag **MagicMeeting** to **Applications**.
3. Launch it.

The build is **signed with a Developer ID certificate and notarized + stapled by Apple**, so it opens cleanly with no Gatekeeper prompt — online or offline. And it **updates itself**: new versions are cryptographically verified and installed in-app, so you're always current.

---

## 💻 Requirements

- **macOS 12.3 (Monterey) or later** — universal build (Apple Silicon + Intel).
- **System-audio capture** (recording what comes through your speakers) requires **macOS 13 (Ventura) or later**; microphone recording works on 12.3+.
- A few hundred MB of disk for the speech models (downloaded once, on first use).

---

## ❓ FAQ

**Is my audio really never uploaded?**
Correct. There is no server and no account. After a one-time model download, MagicMeeting runs fully offline — you can pull the network cable and it works identically.

**Do I need a subscription or license key?**
No. Download it and go.

**Where are my recordings stored?**
In a local database on your Mac, under your control. Delete a session and its audio, transcript, speakers, and minutes are gone for good.

**Can it transcribe files I already recorded?**
Yes — point it at an audio file and get a full speaker-labeled transcript and minutes.

**Which Macs are supported?**
Any Mac on macOS 12.3+, Apple Silicon or Intel, from a single universal download.

---

<div align="center">

## Stop re-listening to your meetings.

### [⬇ Download MagicMeeting for macOS →](https://github.com/apitlekays/magicmeeting-releases/releases/latest)

*On-device transcription · speaker labels · minutes & action items · PDF/Word export — private by design.*

<br/>

<sub>This repository is the public download host for MagicMeeting. The application source lives in a separate private repository; this repo distributes the signed, notarized macOS installers and auto-update artifacts only.</sub>

</div>
