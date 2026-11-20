# 📡 EchoSensus HUD
> **Spatial Audio Visualization, Kinetic Typography & Multi-Lingual Haptic Hazard Warning System for the Deaf and Hard-of-Hearing (DHH)**

Built for **AI Vibeathon 2026**.

---

## 💡 Overview
Over 430 million people worldwide live with disabling hearing loss. Standard assistive solutions lack **spatial awareness**—leaving users unaware of critical directional sound cues such as approaching vehicles, emergency sirens, or a peer speaking from behind.

**EchoSensus HUD** bridges sound awareness and physical safety by converting live ambient sound into a **360° visual radar**, **kinetic live captions**, and **smartwatch haptic vibration alerts**.

---

## ✨ Key Features
* 🧭 **360° Spatial Radar HUD:** Real-time visual tracking of sound direction (bearing) and decibel intensity using Web Audio API frequency analysis.
* 🌐 **Multi-Lingual Engine:** Built-in support for live Speech-to-Text and synthesized female voice alerts across **English**, **Hindi**, **Kannada**, **Tamil**, **Telugu**, and **Spanish**.
* 🚨 **Hazard & Siren Detection:** Automatic sound-spike classification (screams, horns, alarms) triggering full-screen emergency warnings and continuous haptic pulses.
* ⌚ **Smartwatch Haptic Signals:** Distinct vibration patterns mapped to sound direction and hazard severity.
* 🌙 **Low-Power Sleep / Standby Mode:** Battery-efficient low-power monitoring that automatically wakes the display upon high-volume detection.

---

## 🛠️ Tech Stack & Architecture
* **Frontend:** React, Vite, Lucide React Icons
* **Audio Processing:** Web Audio API (`AnalyserNode`), Web Speech API (STT), SpeechSynthesis API (TTS)
* **Native Mobile Integration:** Capacitor JS (Android Native Wrapper)
* **Target Platforms:** Progressive Web App (PWA) & Android (`.apk`)

---

## 📲 Android Deployment
The app compiles to a native Android APK with configured permissions in `AndroidManifest.xml`:
* `RECORD_AUDIO` (Live mic spectrum analysis & speech capture)
* `VIBRATE` (Haptic alert engine)
* `MODIFY_AUDIO_SETTINGS`

---

## 🚀 Getting Started

### Prerequisites
* Node.js (v18 or higher)
* npm

### Installation
```bash
# Clone the repository
git clone [https://github.com/apekshadudaganvi2007-byte/EchoSensus-HUD.git](https://github.com/apekshadudaganvi2007-byte/EchoSensus-HUD.git)

# Navigate to directory
cd EchoSensus-HUD

# Install dependencies
npm install

# Run development server
npm run dev
