<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://ai.google.dev/static/site-assets/images/share-ais-513315318.png" />
</div>

# SheShield 🛡️

SheShield is a modern, full-stack, responsive safety companion web application built specifically for **last-minute, high-stress emergency situations**. By eliminating messy menus, nested tabs, and artificial loading restrictions, SheShield places its three core action protocols right at the very top of the screen—ensuring a user can activate a security workflow in under a second.

---

## 🚀 The Core Problem
During a split-second personal crisis, panic makes it incredibly difficult to navigate standard user interfaces. Traditional safety solutions fail because they are **too slow**, lack **proactive route intelligence**, and completely break down if an emergency dispatch line happens to be **busy or unreachable**. 

SheShield solves this by combining immediate top-screen accessibility, multimodal AI route processing, and an intelligent automated fail-safe escalation engine.

---

## ✨ Features & Core Workflows

### 🟢 1. Route Safety Auditor (Pre-Transit Prevention)
* **How it works:** Users upload a raw screenshot of their live navigation map or cab route.
* **The AI Tech:** The image data is converted to inline base64 and securely transmitted to **Gemini 1.5 Flash** with zero payload size limits.
* **Outcome:** The AI evaluates spatial layout and territory density, dynamically returning an authentic safety index score (1-10) and a precise 2-sentence geographical risk advisory before the journey begins.

### 🟡 2. Active Shield & Two-Way Ghost Call (In-Transit Deterrence)
* **How it works:** A single toggle switch arms localized low-latency ambient audio keyword monitoring.
* **The AI Tech:** Detecting distress triggers an immediate full-screen incoming "Ghost Call" simulator from "Bhaiya (Home)".
* **Outcome:** Powered by the browser's native **Web Speech API**, the application speaks out loud using natural, human-like localized voice accents. Large, bright onscreen text scripts guide the user through a realistic dialogue response loop in **English, Hindi, or Marathi** to psychological deter a nearby threat without arousing suspicion.

### 🔴 3. Critical SOS Panic Button (Split-Second Emergency Response)
* **How it works:** A massive, pulsing red target positioned at the absolute top of the screen designed for instant muscle-memory interaction.
* **The Fail-Safe Escalation Loop:**
  * **Phase A:** Captures high-precision browser GPS coordinates and instantly broadcasts an automated text tracking alert via Twilio to **3 saved family mobile numbers**.
  * **Phase B:** Concurrently places an automated emergency precinct dispatch call, using voice synthesis to broadcast a verbal distress alert to the operator.
  * **Phase C (Smart Backup):** If the gateway logs a busy or dropped connection status within 5 seconds, the app triggers an immediate secondary high-priority text escalation to all 3 family contacts instructing them to dial emergency services manually.

---

## 🛠️ Tech Stack

* **Frontend:** React.js, Tailwind CSS (Mobile-responsive + Desktop smartphone frame mockup layout)
* **Backend Runtime:** Node.js, Express
* **AI Engine:** Google Generative AI SDK (Gemini 1.5 Flash Model)
* **Audio Synthesis:** Web Speech API (`window.speechSynthesis`)
* **Telephony Gateway:** Twilio SMS and Voice Webhooks
* **Persistence:** LocalStorage API (for securing 3 emergency family contacts and language preferences)

---

## ⚙️ Setup and Installation

### Prerequisites
Ensure you have [Node.js](https://nodejs.org/) installed on your machine.

### 1. Clone the Repository
```bash
git clone [https://github.com/YOUR_USERNAME/SheShield.git](https://github.com/YOUR_USERNAME/SheShield.git)
cd SheShield
# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/24d91a59-8516-4f79-bf05-404788c5b94c

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`
