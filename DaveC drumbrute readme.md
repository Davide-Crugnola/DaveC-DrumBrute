# DaveC Drumbrute — Analog Engine Workstation 🥁🎛️

[![License: MIT](https://img.shields.io/badge/License-MIT-orange.svg)](https://opensource.org/licenses/MIT)
[![Web Audio API](https://img.shields.io/badge/Web%20Audio%20API-v2-blue.svg)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-3.0-38bdf8.svg)](https://tailwindcss.com/)

An interactive, browser-based drum machine and 32-pattern bank workstation inspired by classic hardware grooveboxes. Featuring a realistic Web Audio API analog synthesis engine, 14 instrument channel strips, advanced sequencing features, and full Web MIDI integration.

---

## 🌟 Key Features

*   **Realistic Analog Synthesis Engine:** Custom DSP synthesized drum voices with parameters for **Tune, Decay, Tone, and Snap**. Supports custom audio sample loading (`.wav`, `.aif`, `.mp3`) per track.
*   **64-Step Polyrhythmic Sequencer:**
    *   Per-step **Probability** (0–100%).
    *   Per-step **Micro-Timing** (early/late offset).
    *   Individual polyrhythmic step lengths per instrument channel.
    *   Global **Swing** and **Randomness** controls.
*   **Virtual Mixer & Master FX Chain:**
    *   **Steiner-Parker Style Filter** (LP, HP, BP, Notch with resonance and cutoff controls).
    *   **Master Drive & Soft-Clip Distortion**.
    *   **Algorithmic Delay & Reverb** with dedicated send buses.
    *   **12-Band Master Graphic Equalizer** and **Master Dynamics Compressor**.
*   **ReBirth-Style 32-Pattern Bank System:** 4 Banks (A–D) × 8 Patterns each with local storage persistence and genre-based algorithmic pattern generators (House, Techno, Trap, Dub, DnB, and more).
*   **Advanced Control & Connectivity:**
    *   **Interactive WOW Knobs:** Physics-based rotation, inertia, fine-precision mode, and customizable skin styles (*Classic, Soft-Touch Rubber, Industrial Metal, Neon Cyber*).
    *   **MIDI Learn & Sync:** Map hardware MIDI CC knobs directly to UI parameters, receive/send MIDI Clock, and support Web Serial MIDI.
    *   **Roller / Looper Touch Strip:** Instant note-repeat functionality (1/2 to 1/64 divisions).
    *   **DAW Export Tools:** One-click **SysEx Dump (JSON)** import/export and **JUCE C++ VST3 wrapper** export for Ableton Live 12 integration.

---

## 🚀 Quick Start

Since **DaveC Drumbrute** is built entirely as a client-side web application, no compilation or complex setup is required.

1. Clone or download this repository:
   ```bash
   git clone https://github.com/Davide-Crugnola/DaveC-Drumbrute.git
   ```
2. Open `DaveC Drumbrute.html` in any modern Web Browser (*Google Chrome, Microsoft Edge, Firefox, or Safari*).
3. Click the **POWER ON / START** button in the top right header to initialize the Web Audio context.

---

## 🎛️ How to Use

### 1. Sequencer & Pattern Controls
* **Selecting Channels:** Click on any channel strip to set it as the active instrument track.
* **Step Modes:** Toggle between **NOTE**, **PROBABILITY**, and **MICRO-TIMING** mode above the step grid to adjust parameters per step.
* **Euclidean Generator:** Use the Euclidean sub-panel knobs to generate algorithmic rhythms by setting *Pulses* and *Rotation* for the active track.

### 2. MIDI & Hardware Mapping
* **Right-Click** on any knob to enter **MIDI Learn** mode. Move a physical control on your external MIDI controller to pair it instantly.
* Open the **⚙️ MIDI Learn Manager** modal to review, export, or import your custom CC map.

### 3. Presets & Memory
* Choose from **300 pre-configured genre presets** via the top preset dropdown.
* Use the **RANDOM BATTERY** button to generate a completely unique kit and pattern based on your selected music genre.

---

## 🛠️ Built With

* **Web Audio API** — Real-time analog sound synthesis, convolution reverb, and master DSP effects chain.
* **HTML5 / JavaScript (ES6+)** — Modular single-file application architecture.
* **Tailwind CSS** — Hardware-inspired UI styling.
* **Web MIDI API & Web Serial API** — External hardware device synchronization and control.

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.