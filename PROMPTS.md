# ⚙️ Advanced Teaching Movie for Fatigue Failure

This repository contains the complete project files, technical documentation, English voiceover scripts, SSML configurations, and AI generation prompts for our 3-minute engineering teaching movie on **Fatigue Failure**, presented on November 4.

---

## 📋 1. Project Overview & Objectives
* **Topic**: Fatigue Failure, Macro-Fractography, and Life Prediction[cite: 1, 5]
* **Target Duration**: 3 Minutes
* **Core Engineering Concepts**:
  * Macro-fractography (Crack origin, beach marks, final failure zone)[cite: 5].
  * S-N diagram, stress amplitude, and the endurance limit[cite: 1].
  * High-cycle vs. low-cycle fatigue and mean stress effects (Goodman diagram)[cite: 1].
  * Linear Elastic Fracture Mechanics, Paris' Law, and Fracture Toughness ($K_{IC}$)[cite: 1].

---

## 🔬 2. Macro-Fractography & Failure Stages
As analyzed in our specimen study, fatigue failure under cyclic loading consists of three distinct stages[cite: 1, 5]:
1. **Crack Origin (Initiation)**: Typically forms at surface defects, sharp geometric notches, or machining marks where stress concentration is localized[cite: 5].
2. **Fatigue Zone & Beach Marks**: Smooth, concentric ripples representing progressive crack advancement during variable loading cycles[cite: 5].
3. **Final Failure Zone**: A rough, abrupt fracture region when the remaining cross-section can no longer bear the maximum tensile load[cite: 5].

---

## 📈 3. Analytical Models & S-N Curves
* **S-N Diagram**: Plots stress amplitude ($S$) against the logarithm of cycles to failure ($N$)[cite: 1].
* **Endurance Limit**: For ferrous alloys, the curve flattens at a specific stress threshold, below which the component theoretically achieves an infinite fatigue life[cite: 1].
* **Fracture Mechanics**: When pre-existing micro-cracks exist, Linear Elastic Fracture Mechanics and Paris' Law are applied to track crack growth until critical fracture toughness ($K_{IC}$) is reached[cite: 1].

---

## 🤖 4. AI Workflows, Prompts & Open-Source Records
To achieve professional production standards, this project leverages advanced AI pipelines and open-source documentation:
* **Open-Source Records & Chat Contexts**: 
  * [Gemini Open Source Session 1](https://share.gemini.google/FxV8kekmMtKH)
  * [Gemini Open Source Session 2](https://share.gemini.google/yfMMmIByP25e)
  * [Gemini Open Source Session 3](https://share.gemini.google/rGsGzRpYeCBG)
* **Image Generation Prompts**:
  * *Specimen Photo*: `"Macro photography of a metal fatigue failure surface in a steel rod, showing clear beach marks and beach patterns, industrial laboratory background, high resolution, realistic."`
  * *S-N Curve Animation*: `"Clean 2D scientific animation of an S-N curve graph, stress amplitude versus cycles to failure on a log scale, highlighting the endurance limit, dark mode style."`

---

## 🎙️ 5. SSML Voiceover Configuration
To bypass robotic text-to-speech limitations, professional SSML (Speech Synthesis Markup Language) tags were implemented to control natural breath pauses, pacing, and technical emphasis:

```xml
<speak version="1.0" xml:lang="en-US">
  <p>
    <s>Ever bent a paper clip back and forth until it snapped?</s>
    <break time="240ms"/>
    <s>The force was small, yet the metal failed. The answer is fatigue failure.</s>
  </p>
</speak>
