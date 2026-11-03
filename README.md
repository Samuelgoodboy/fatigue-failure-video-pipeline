# 🔩 Fatigue Failure — Automated Academic Video & Neural TTS Pipeline

An automated Python media-processing pipeline created for the **Materials Science Mini-Lesson: Fatigue Failure**. This project replaces legacy offline synthetic narration with studio-grade Neural Text-to-Speech (`edge-tts`) and dynamically re-aligns hardcoded subtitles using `FFmpeg`.

---

## 🎯 Project Overview

Educational engineering animations require clear, authoritative narration and precise visual-audio synchronization. This repository contains the narration script, prompt engineering workflow, and Python automation script that:
1. **Generates Neural Voiceover**: Converts a 12-scene time-coded academic script into a natural American English lecture track (`en-US-AndrewNeural`) with synchronized `.srt` word timings.
2. **Mutes Legacy Audio**: Strips the original robotic audio track from the base animation (`Fatigue_Class_Video_NEW.mp4`).
3. **Masks Hardcoded Subtitles & Burns Dynamic ASS Subtitles**: Applies a color-matched `#0B131B` bounding-box mask (`y=87.4%` to `98.8%`) to cover legacy baked-in captions while preserving the progress bar UI, then renders newly aligned subtitles.

---

## ⏱️ 12-Scene Academic Script Structure (3:00 Runtime)

| Scene | Timecode | Topic | Key Engineering Concepts |
| :--- | :--- | :--- | :--- |
| **01** | `00:00 – 00:10.5` | **Hook** | Paper clip bending & low-force failure mystery |
| **02** | `00:10.5 – 00:23.0` | **Definition** | Repeated loading vs. single static load |
| **03** | `00:23.0 – 00:36.2` | **Cycle** | Bicycle wheel spoke loading/unloading cycle |
| **04** | `00:36.2 – 00:51.7` | **Three Stages** | Initiation, crack propagation, final sudden rupture |
| **05** | `00:51.7 – 01:06.7` | **Crack Animation** | Incremental cyclic crack length extension |
| **06** | `01:06.7 – 01:25.1` | **Fracture Surface** | Crack initiation site, curved beach marks, rough final break |
| **07** | `01:25.1 – 01:39.7` | **S–N Diagram** | Stress amplitude ($S$) vs. Cycles to failure ($N$) |
| **08** | `01:39.7 – 01:56.4` | **Endurance Limit** | High/low stress trends & steel endurance limit threshold |
| **09** | `01:56.4 – 02:12.6` | **Fracture Toughness** | Material resistance to unstable crack-driven fracture |
| **10** | `02:12.6 – 02:27.6` | **Stress Intensity ($K$)** | $K = Y \sigma \sqrt{\pi a}$ and critical fracture limit ($K_{IC}$) |
| **11** | `02:27.6 – 02:42.0` | **Prevention** | Stress reduction, fillet radii, material selection, NDT inspection |
| **12** | `02:42.0 – 03:00.0` | **Summary** | Core takeaways & closing hold |

---

## 🛠️ Tech Stack & Requirements

* **Python 3.10+**
* **[edge-tts](https://github.com/rany2/edge-tts)**: Microsoft Edge Neural TTS API for natural academic voice synthesis and subtitle timing extraction.
* **[imageio-ffmpeg](https://github.com/imageio/imageio-ffmpeg)**: Self-contained FFmpeg binary wrapper for audio remuxing, `drawbox` masking, and `libass` subtitle rendering.

---

## 🚀 How to Run

1. **Clone the repository and install dependencies:**
   ```bash
   pip install edge-tts imageio-ffmpeg
