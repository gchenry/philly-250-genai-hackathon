# Philly 250: Founding Fathers in Modern Philly — Coach's Guide

## Introduction

Welcome to the official Coach's Guide for the **Philly 250 GenMedia gHack**. This workshop tasks participants with a high-stakes creative challenge: producing a **30-to-60-second broadcast-quality commercial** for Philadelphia’s 250th Anniversary (the Semiquincentennial).

The core prompt for participants is: **"What would the Founding Fathers do in Modern Philly?"** Your role as a coach is to provide strategic guidance, helping teams navigate technical hurdles while ensuring their content remains professional and on-brand for **Visit Philadelphia**.

> **Important**
> This guide is intended for coaches and Google Cloud volunteers. If you are a participant, please refer back to your project **README.md** to maintain the integrity of the challenge.

---

## Logistics & Coaching Strategy

*   **Date & Location:** May 5-6, 2026, at CIC Philadelphia.
*   **Coach Ratio:** We aim for a **5:1 ratio**.
*   **Environment:** Labs are hosted via **Google Cloud Skills Boost**.
*   **The Goal:** Winning videos will be evaluated by **Visit Philadelphia** for actual 2026 tourism campaigns.

---

## Challenge 1: From History to Narrative

**Estimated Time:** 30 Minutes

### Key Concepts to Explain
*   How to use Gemini for creative "What If" scenarios.
*   The importance of the **Visit Philly** brand voice.

### Known Blockers & Hints
*   **Blocker:** Teams write scripts that are too long or complex for 60 seconds.
*   **Hint:** Remind them that "Less is More." A 3-scene structure is the "sweet spot" for AI video generation.
*   **Blocker:** Generic or boring scripts.
*   **Hint:** Encourage a "hook"—e.g., Ben Franklin trying to use a touch-screen kiosk.

---

## Challenge 2: The Visual Blueprint

**Estimated Time:** 45 Minutes

### Key Concepts to Explain
*   **Character Consistency:** Using a "Contact Sheet" to anchor the AI model.
*   **Visual Prompting:** Using descriptive tags for clothing and lighting.

### Known Blockers & Hints
*   **Blocker:** Characters look different in every frame.
*   **Hint:** Teams **must** generate a "Contact Sheet" (a grid of the character from different angles) in **Imagen 3** before moving to video.
*   **Blocker:** 1770s clothing looks historically inaccurate.
*   **Hint:** Use specific descriptors like "colonial navy blue wool coat with brass buttons."

---

## Challenge 3: From Stills to Motion

**Estimated Time:** 60 Minutes

### Key Concepts to Explain
*   **Reference to Video:** Using image inputs to guide **Veo Pro**.
*   **Compute Latency:** Managing expectations for generation times.

### Known Blockers & Hints
*   **Blocker:** Video generation "hallucinates" and changes the character's face.
*   **Hint:** Upload the **Contact Sheet** as a reference image in the Veo UI to "lock" the character's identity.
*   **Blocker:** Generation taking too long.
*   **Hint:** Start the next clip generation as soon as the previous one begins rendering.

---

## Challenge 4: The Assembly

**Estimated Time:** 45 Minutes

### Key Concepts to Explain
*   Timeline management in **Google Vids**.
*   Narrative pacing.

### Known Blockers & Hints
*   **Blocker:** Jarring transitions between AI clips.
*   **Hint:** Show teams how to use standard "cuts" or subtle fades rather than complex AI transitions that might distort the faces.

---

## Challenge 5: Audio & Final Polish

**Estimated Time:** 30 Minutes

### Key Concepts to Explain
*   Text-to-Speech (TTS) vs. Music Generation (Lyria).
*   Soundscape layering.

### Known Blockers & Hints
*   **Blocker:** Audio doesn't match the historical/modern fusion theme.
*   **Hint:** Suggest a "Modern-Colonial Fusion"—e.g., Hip-hop beats mixed with a harpsichord.
*   **Blocker:** Voiceovers sound too robotic.
*   **Hint:** Use **Gemini TTS** with specific emotional modifiers in the prompt to get a more "theatrical" performance.

---

## Success Criteria

1.  **Narrative:** Does the story align with a tourism ad?
2.  **Consistency:** Does the Founding Father look like the same person in every scene?
3.  **Branding:** Does it include the **Visit Philly** messaging?
4.  **Duration:** Is the final export between **30 and 60 seconds**?

---

## Contributors
*   **Murat Eken**
*   **Gino Filicetti**
*   **Jeff Katzen**
*   **Justin Grayston**
*   **Len Henry**