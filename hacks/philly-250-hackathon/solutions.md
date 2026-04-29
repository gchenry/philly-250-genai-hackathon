# Easy Ads: From Concept to Creation with GenMedia

## Introduction

Welcome to the coach's guide for the *"Philly 250" GenMedia gHack*. As a local Google Cloud volunteer coach, you are assigned to teams at a 5:1 ratio. Your role is to provide strategic guidance, troubleshoot physics errors in generation, and review solutions, but **do not give teams the direct answers**. 

The ultimate outcome of this event is highly commercial: Visit Philadelphia intends to evaluate these videos for actual 2026 tourism campaigns. Quality and consistency are paramount!

> [!NOTE]  
> If you are a gHacks participant, this is the answer guide. Don't cheat yourself by looking at this guide during the hack!

## Coach's Guides

## Challenges

- Challenge 1: From History to Narrative
- Challenge 2: The Visual Blueprint  
- Challenge 3: From Stills to Motion  
- Challenge 4: The Assembly  
- Challenge 5: Giving It a Voice  
- Challenge 6: The Soundtrack  

## Challenge 1: From Product to Narrative

### Notes & Guidance

If the participants are using Vertex AI Studio for generating the story, they should turn on auto-save. This way they can keep track of their progress and easily hand over the generated descriptions to the next driver.

In this challenge, teams are tasked with answering: *"What would the Founding Fathers do in Modern Philly?"*

If the participants are using Vertex AI Studio for generating their Visit Philly brand guidelines and story, they should turn on auto-save. This way they can keep track of their progress and easily hand over the generated descriptions to the next driver.

> [!TIP]  
> Coursework should teach the "secret" of using Gemini to generate the highly specific, logic-based prompts required for the downstream image and video models. Using the first best response might lead to generic outputs, so encourage teams to add creativity and iterate.

It is helpful to have generic system instructions when using Gemini to capture the purpose and subject:

```text
We're creating an ad for Visit Philadelphia's America's 250th Anniversary. The premise is a historical Founding Father (e.g., Benjamin Franklin) interacting with modern Philadelphia. The tone should be engaging for global tourists.
```

We're expecting *at least* three scenes, but it makes sense to have more (and shorter) scenes. Veo will struggle if there's too much happening in a single scene. The snippet below is from *Veo Prompting Best Practices*:

> Attempting to prompt "A knight battles a dragon, then flies on its back to a castle, then attends a feast" in a single prompt for an 8-second clip will likely result in a muddled or incomplete depiction of one small part, or a very rushed and incoherent sequence. Instead, generate each distinct part as a separate clip if needed.

#### Pro Tips for the Students

- Take **5 mins** with your team discussing the brand guidelines, the specific Founding Father, and the tone. Don't waste time here.
- Focus on your story and keep in mind that you have 30-60 seconds to tell that story. Each scene is about 8 seconds.  
- Don't try to squeeze too many different things in a single scene. Keep it simple.  
- Parallelize your work.
  - One person can work on the Protagonist description.
  - One person on Styling and Brand Guidelines.
  - The rest can work on the storyline/narrative.

---

## Challenge 2: The Visual Blueprint

### Notes & Guidance


The idea is that participants should use the descriptions from Challenge 1, and use either Gemini or *Help me write* capabilities within Vertex AI Media Studio to generate the required prompts. 

> [!IMPORTANT]  
> Participants must use **Imagen 3 / NanoBanana** for premier image and storyboard generation. 

To prevent randomness and noise in the final video, **participants must be challenged to successfully prompt a 3D "contact sheet"** (showing the protagonist from multiple angles) to establish visual consistency.

> [!WARNING]  
> At the time of this writing, Nano Banana in Vertex AI Media Studio has a limit of 10MB, so if there are too many images inserted in a single conversation, things will fail. Also, there are limits to how many images can be included in a single prompt (3 for Nano Banana at the moment). Participants should use multiple conversations and/or fewer images if they hit these limits.

#### Pro Tips for the Students

- The more details provided by the output of the previous challenge, the more consistent your images will be.
- Avoid too many things at once. Keep the scene clean. 
- Google Models take IP and Safety very seriously. Do not use any real modern persons or copyrighted brands. 
- Have a distinct 16:9 final closing frame with space for the Visit Philly logo[cite: 3].

---

## Challenge 3: From Stills to Motion

### Notes & Guidance

The storyboard images created in the previous challenge should be used as a *Reference* to generate the video clips. If the participants gloss over this, they will struggle with consistency. Similarly, just like the previous challenge, **DO NOT** let them struggle for too long.

There's a plethora of different options here, participants can use the story board imags as *Reference*s, or generate start and end frames based on the story board and use those for the newer *Veo* models.

#### Pro Tips for the Students

- In the interest of time and so that everyone gets to play, parallelize this task across your team.
- Video generation is time-intensive. To optimize efficiency, we recommend that **two or three team members simultaneously generate distinct video sets**. Afterwards, compare and select the most effective clips, or regenerate as necessary. Do not delay progress.
- For enhanced consistency, consider **utilizing a screenshot of the final frame** from Video 1 as the initiating frame for Video 2.
- Upload **3-5** images and detailed descriptions.
- Can't emphasize enough to go through this guide [Veo on Vertex AI video generation prompt guide](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/video/video-gen-prompt-guide). This separates a great shot from a good shot.
- Google Models take IP and Safety very seriously. Do not use any known persons, products, films, references, likeness or names. Safety filter will trigger if Gemini detects such references in the prompt.
- If you see your Founding Father develop discrepancies between scenes (e.g., their wig changes), go back to the previous challenge and develop better reference images.

## Challenge 4: The Assembly

### Notes & Guidance

#### Video Editor

In the rest of this gHack's challenges, you will be piecing together your final ad video. Unless you prefer your own editing tools (Adobe Premiere Pro, Final Cut Pro, DaVinci Resolve, etc), we strongly recommend using Google Vids.

Google Vids is a web-based video creation app designed to make producing professional videos as simple as creating a slide deck without any prior video editing experience. It is available on any Google Workspace account and also on personal gmail accounts if necessary.

#### Pro Tips for the Students

- Don't worry about the sound at this step. Just focus on the complete Video. You will add a voiceover in the next step  
- You could use Gemini for generating text as well, but in case you're not getting what you want, you can just use text elements within your video editor.
- Ensure the final closing frame includes the Visit Philly / Philly 250 logo and your call to action.

## Challenge 5: Giving It a Voice

### Notes & Guidance

You'll have the choice to use Google's Chirp 3 HD model or Gemini itself to create the voice-overs. The difference between these two lies in the source of vocal identity and style. Chirp functions as an advanced text-to-speech engine, requiring a pre-existing voice, either from its library or a custom clone, to articulate the provided text with high fidelity; any stylistic nuance is primarily achieved through manipulating the text itself with punctuation and pacing adjustments. In contrast, Gemini operates as a true generative voice model, creating the vocal characteristics and delivery style from scratch based on natural language prompts. This allows a user to conjure a voice by describing it (e.g., "a deep, soothing voice") and directing its emotional tone (e.g., "speak with excitement"), offering a layer of creative control and on-the-fly vocal design that Chirp, in this context, does not.

**Crucial Hackathon Requirement:** To make the Visit Philly campaign global-ready, at least one of the voice-overs must be generated in a foreign language (e.g., Italian, Spanish, French). Ensure teams do not skip this requirement!

#### Pro Tips for the Students

- This is the final touch of your video. A good narrative is what you need.
- You can sample voices and choose the right voice from the samples [here](https://docs.cloud.google.com/text-to-speech/docs/chirp3-hd).  
- If you have already established if it's a male or female voice the choice is easier!
- Finally, add these audio tracks in the proper places in your video sequence timeline. You can use Vids to insert the audio. You can change the speed of the audio in both Vids and in Chirp.

## Challenge 6: The Soundtrack

### Notes & Guidance

Teams will use **Lyria** to compose a custom background music score, layering all audio elements into their final Vids project.

Remind teams that the music should match the brand guidelines they set in Challenge 1. For example, they might want to prompt Lyria to blend historic orchestral tones (fife and drum) with modern Philly beats

#### Pro Tips for the Students
- Including instrument information in the prompt can be helpful.
- Make sure to balance the volume in Google Vids so that the music complements the voice-overs without overpowering them.