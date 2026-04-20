# Philly 250: Founding Fathers in Modern Philly — Coach's Guide

## Introduction

Welcome to the official Coach's Guide for the **Philly 250 GenMedia gHack**. This workshop tasks participants with a high-stakes creative challenge: producing a **30-to-60-second broadcast-quality commercial** for Philadelphia’s 250th Anniversary (the Semiquincentennial).

The core prompt for participants is: **"What would the Founding Fathers do in Modern Philly?"** Your role as a coach is to provide strategic guidance, helping teams navigate technical hurdles while ensuring their content remains professional and on-brand for **Visit Philadelphia**.

> [!IMPORTANT]
> This guide is intended for coaches and Google Cloud volunteers. If you are a participant, please refer back to your project **README.md** to maintain the integrity of the challenge.

---

## Logistics & Coaching Strategy

*   **Date & Location:** May 5-6, 2026, at CIC Philadelphia.
*   **Coach Ratio:** We aim for a **5:1 ratio** to ensure high-touch strategic support for every team.
*   **Environment:** Labs are hosted via **Google Cloud Skills Boost**. Ensure teams use the table-specific short links to access their "pre-warmed" environments.
*   **The Goal:** The stakes are high—**Visit Philadelphia** intends to evaluate the winning videos for potential use in their actual 2026 tourism campaigns.

---

## The Five Challenges

Teams must progress through five distinct phases to complete their commercial. Below are the technical strategies found in **solutions.md** to help you unblock them.

### Challenge 1: From History to Narrative (Ideation & Scripting)
Participants establish their **Visit Philly brand guidelines** and choose a historical protagonist.

*   **Coaching Tip:** While using Gemini is required, first drafts are often generic. Encourage teams to find a "hook"—like Ben Franklin trying to use a touch-screen kiosk or George Washington at a modern sporting event.
*   **Scripting:** Scripts should be limited to **3 scenes**. Remind teams that simpler scenes result in better video generation later.

### Challenge 2: The Visual Blueprint (Storyboarding)
Teams use **Imagen 3 (NanoBanana)** in Vertex AI Studio to generate high-quality 16:9 storyboards.

*   **The Secret Sauce:** To ensure **Character Consistency**, teams **must** generate a "Contact Sheet" (a 3x3 or 4x4 grid) of their character from different angles.
*   **Prompting:** Guide teams to use consistent descriptors (e.g., "Silver-haired man in a 1770s navy blue colonial coat with brass buttons") across all image prompts.

### Challenge 3: From Stills to Motion (Video Generation)
This is the most compute-heavy step. Participants will use the **Veo Pro Model**.

*   **Reference to Video:** Coaches should show teams how to upload their **contact sheets** and storyboard stills as references. This "anchors" the model, forcing it to keep the character's face and clothes consistent.
*   **Iteration:** If the character looks different in a clip, have the team refine their reference image rather than fighting the text prompt.

### Challenge 4: The Assembly (Editing)
Teams bring all assets into **Google Vids** for post-production.

*   **Pacing:** Help teams manage their timeline. A 30-60 second ad usually needs 4-6 strong clips.
*   **Transitions:** Ensure the flow between AI-generated clips doesn't feel jarring or "dream-like."

### Challenge 5: Audio & Final Polish
The final layer involves **Chirp 3 HD, Gemini TTS, and Lyria**.

*   **Voice:** Use **Gemini TTS** for specific character lines or **Chirp 3 HD** for high-fidelity narrations.
*   **Music:** **Lyria** should be used to create a custom soundtrack. Suggest a "Modern-Colonial Fusion" (e.g., Hip-hop beats with a harpsichord) to match the theme.

---

## Success Criteria

As you monitor the room, check that teams are hitting these benchmarks:
1.  **Narrative:** Does the story make sense for a tourism ad?
2.  **Consistency:** Does the Founding Father look like the same person in every scene?
3.  **Branding:** Does it include the **Visit Philly** messaging?
4.  **Duration:** Is the final export strictly between **30 and 60 seconds**?

Successful teams are eligible for custom **digital Credly badges** acknowledging their mastery of GenMedia workflows.