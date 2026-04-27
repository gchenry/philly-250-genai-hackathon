# "Philly 250" GenMedia gHack: Founder Fathers in Modern Philly

## Introduction

Welcome to the "Philly 250" GenMedia gHack! In this challenge-based learning experience, you will work in teams of up to 5 people to build 30-to-60-second broadcast-quality commercials celebrating Philadelphia's 250th Anniversary (Semiquincentennial).  Your creative mission is to answer a simple premise: "What would the Founding Fathers do in Modern Philly?"

The ultimate goal of this hackathon is highly commercial. Visit Philadelphia intends to evaluate and potentially use the winning videos as actual ad copy for their 2026 tourism campaigns! You will use Google Cloud's generative AI tools to bring your vision to life, ensuring your final ad is coherent, consistent, and on-brand.

![Challenge Overview](./images/easy-ads-overview.png)

This isn't about writing code. It's about mastering the art of the prompt. You will use Google Cloud's generative AI tools within Vertex AI Studio to bring your vision to life. The challenge lies in guiding these models to produce a final ad that is not just aesthetically pleasing, but also **coherent, consistent,** and **on-brand,** complete with **multilingual voice-over**, graphic overlays and a **custom soundtrack**.

## The Tech Stack

You will master the following Generative Media suite:
*   **Gemini:** For scripting, planning, and prompt generation.
*   **Imagen 3 (NanoBanana) via Vertex AI Studio:** For premier image and storyboard generation.
*   **Veo (Pro Model):** For high-definition image-to-video generation.
*   **Google Vids:** The video assembly and editing engine.
*   **Chirp 3 HD / Gemini TTS & Lyria:** For AI voiceovers and custom soundtrack generation.

## Learning Objectives

This hack will help you master the following skills:

- Advanced Prompt Engineering  
  - Crafting detailed prompts to control style, composition, and object consistency.  
- Consistent Generation  
  - Creating a believable product and protagonist and maintaining their appearance across different shots.  
- Text-to-Image Generation  
  - Composing a set of graphical elements to enhance the visual appeal of the ad and convey brand information: logos, taglines, etc.  
- Text-to-Video Generation  
  - Directing AI to create dynamic, high-quality video clips from text and image prompts.  
- Text-to-Speech Generation  
  - Creating a professional voice-over in multiple languages.  
- Text-to-Music Generation
  - Composing a custom soundtrack that matches the mood of the ad.  
- Video Assembly  
  - Stitching generated visual and audio assets into a final, polished video.


## Challenges

- Challenge 1: From History to Narrative
- Challenge 2: The Visual Blueprint  
- Challenge 3: From Stills to Motion  
- Challenge 4: The Assembly  
- Challenge 5: Giving It a Voice  
- Challenge 6: The Soundtrack  

## Prerequisites

- Basic understanding of generative AI concepts (text-to-image, text-to-video, text-to-speech).  
- Access to a Google Cloud project with Vertex AI Studio enabled, including access to Gemini, Veo, Chirp, and Lyria models.  
- Access to a basic video editing tool (e.g., Google Vids, DaVinci Resolve, Adobe Premiere Pro, CapCut, iMovie, or any online editor).

## Contributors

- Murat Eken  
- Gino Filicetti  
- Jeff Katzen  
- Justin Grayston
- Len Henry

## Challenge 1: From History to Narrative

### Introduction

Every ad starts with a product and tells a story to sell that product. In this challenge, our "product" is the City of Philadelphia celebrating its 250th Anniversary. We will come up with brand guidelines for Visit Philly, design a story and a character, and make sure everything stays coherent.

#### The Product

The "product" being advertised is the City of Philadelphia celebrating its 250th Anniversary, with the goal of promoting tourism for the 2026 Semiquincentennial.

> [!NOTE]  
> This challenge is all about building our story and characters, we're expecting you to craft descriptions, which we'll use in the subsequent challenges to create prompts. So, your descriptions should be detailed enough to capture the essence of your story, but keep in mind that we're not designing prompts yet.

### Description

First, create a document (e.g. Google Doc) that's shared with your whole team, so you can collaborate and keep track of your work.

Establish a set of **brand guidelines** for your Visit Philly commercial. Outline the aesthetic, values, mood, color palette, and target audience (e.g., global tourists, history buffs).

Next, create a description of your **protagonist** (e.g., George Washington, Benjamin Franklin, Frederick Douglass). This description needs to be detailed enough so that we can achieve consistency from shot to shot.

Now, craft an **overall narrative** to tell the story of your Founding Father experiencing modern Philadelphia. Create textual descriptions of **at least three scenes** describing what happens in each scene and how they tie together.

Finally, create a **tagline or call to action** that meets the brand guidelines (e.g., "Visit Philadelphia in 2026"). We’ll use that text in our final ad video. 

> [!NOTE]  
> Using Gemini in this challenge is fair game, but if you want to flex your creative muscles and do your own writing, please feel free to.

### Success Criteria

- You have created a set of brand guidelines describing the *aesthetics*, *values*, *mood/color palette* and *target audience* for the brand.
- You have created a detailed text description of the protagonist of your narrative.
- You have created a text description/script for at least three scenes that seamlessly tell your story.
- You have created a tagline or call to action that meets the brand guidelines.
- Your work is stored in a shared document (e.g. Google Doc) that's accessible by your team.

### Learning Resources

- [Gemini Prompts for Ad Copy](https://felloai.com/2025/08/7-effective-gemini-prompts-for-ad-copy-that-actually-bring-results/)
- [Storytelling in the Ad Creative Process](https://mailchimp.com/resources/storytelling-in-marketing)  

### Tips

- Focus on your story and keep in mind that you have 30 seconds to tell that story.
- Don't try to squeeze too many different things in a single scene.
- Using Gemini is fair game, but make sure that you keep its output brief and clear.
- Although Gemini will help with inspiration, it will generate similar (and rather bland) ideas if you enter the challenge description in verbatim (we've seen far too often an architect called Elara to be the protagonist).

## Challenge 2: The Visual Blueprint

### Introduction

Now that we have our brand guidelines, our Founding Father, and our narrative, it’s time to create our visuals. This is the storyboard of your ad, which visually shows the flow of your narrative.

### Description

First, we will create our protagonist. Using **Gemini Native Image (Nano Banana)**, generate a representative image of your historical figure using your description from Challenge 1. Once you have your protagonist, generate more images depicting them at different angles (front, side, back, 3/4). To prevent randomness and noise in the final video, prompt a 3D "contact sheet" (showing the protagonist from multiple angles) to establish visual consistency.

> [!NOTE]  
> Given the limit of 3 images as context when generating videos and images, consider creating a "contact sheet" for the protagonist and product with all images at the various angles together in one image file.

Next, create **16:9 images** for your storyboard visualizing your three scenes (e.g., Benjamin Franklin at City Hall or eating a cheesesteak). These storyboard images should contain accurate and consistent depictions of your protagonist.

We also need a **final closing frame** that will inform Veo on how to end the video. It should include space for the Visit Philly / Philly 250 logo and space for your call to action.

### Brand Resources
[Visit Philadelphia Brand Guidelines](https://www.visitphilly.com/wp-content/uploads/2022/04/APRIL2022_VP-VISUAL-BRAND-GUIDE.pdf)


> [!NOTE]  
> These storyboard images will be used in the next challenge and there are multiple ways to reference them. You can use them as start/end frames, you can use them as *Subject* reference. If you don't design your storyboard images with that idea or if you don't use them in the next challenge, you will struggle with the consistency.

We also need a **final closing frame** that will inform Veo on how to end the video. It should include space for the Visit Philly / Philly 250 logo and space for your call to action.

> [!IMPORTANT]  
> The storyboard images must be in 16:9 format because we'll use them as references for the video clips we'll create in the next challenge

We've already created a storage bucket for you, make sure that all of this work is stored in that bucket, as we'll use these assets when we compose our final video (copying those images into your document and screenshotting will negatively impact the quality of these images).

### Success Criteria

- Multiple consistent images are generated that clearly define the **protagonist's appearance** from various angles.
- You have generated **distinct storyboard images** and a **final closing frame image**.
- The protagonist's appearance and the overall aesthetic/mood are visibly consistent across all storyboard images.
- Your coach approves of the visual consistency of your images.
- The images are stored in the storage bucket that has been provided to you.

### Learning Resources

- [Vertex AI Studio Quickstart](https://cloud.google.com/vertex-ai/generative-ai/docs/start/quickstarts/quickstart)
- [Nano Banana Prompting Guide](https://developers.googleblog.com/en/how-to-prompt-gemini-2-5-flash-image-generation-for-the-best-results/)

### Tips

- If you're in a squeeze for time, you can parallelize the protagonist, product, and logo generation. You'll need both product and protagonist contact sheets to start with the storyboard images though.
- Keep in mind that some models will have limitations with respect to how many reference images you can include in a prompt and the maximum size. See for example the *Technical Specifications* for [Nano Banana](https://cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/2-5-flash-image)
- There are also limits in the Media Studio UI, you might want to use the Import from Cloud Storage options instead of uploading your images in your prompt

## Challenge 3: From Stills to Motion

### Introduction

With your storyboard and protagonist created, it's time to bring your vision to life. This challenge is about converting your static scenes of modern Philly into dynamic video clips.

### Description

Using the *Veo* family of models in Vertex AI Studio, generate video clips for each of your storyboard scenes from Challenge 2. Make sure you use your generated images as references in your prompts to guide the model.

> [!IMPORTANT]  
> It's fine to have background sound or noises for some parts of your video, but keep in mind that you'll be generating voice-overs in a later challenge. Also, if you need to have dialog that syncs with lips on the screen, that needs to be done during video creation time.
> Because Veo generation is currently capped at 8-second clips, you must use the "Reference to Video" function—uploading your generated contact sheets alongside text prompts to force the model to maintain character consistency across multiple short clips.

Once finished, store your favorite clips for each scene in the storage bucket provided to you (ideally in a separate folder).

### Success Criteria

- High-quality video clips for each of the storyboard scenes are generated.
- The total runtime for the video clips should be around ~30 seconds (min: 20 seconds and max: 1 minute).
- The video aesthetics, mood and color palette are *highly consistent* with the corresponding static images.
- The motion depicted is *smooth* and *realistic*.
- When viewed in sequence, the clips form a coherent narrative, with logical transitions.
- Your coach approves of the visual consistency of your videos and their fidelity to your storyboard images.
- The videos have been stored in the storage bucket that has been provided to you.

### Learning Resources

- [Generate videos with Veo](https://cloud.google.com/vertex-ai/docs/generative-ai/video/generate-videos)
- [Veo Prompting Guide](https://cloud.google.com/blog/products/ai-machine-learning/ultimate-prompting-guide-for-veo-3-1)

### Tips

- Similarly to the previous challenge, if you're pressed for time, you can parallelize the video generation for the various scenes.

## Challenge 4: The Assembly

### Introduction

You have all your visual components. Now it's time for post-production. In this challenge, you'll act as the editor, assembling the generated clips into a single, seamless advertisement.

### Description

Using **Google Vids**, stitch together the Veo video clips you created in Challenge 3. The goal is to create a single, cohesive video file that flows logically and tells the intended story.

To close out the ad, add in the Visit Philly logo, any static graphics you created, and your tagline/call to action.

> [!NOTE]  
> You could use *Nano Banana* for generating text as well, but in case you're not getting what you want, you can just use text elements within your video editor.

### Success Criteria

- The video is around 20-30 seconds long (min: 20 seconds and max: 1 minute).
- The video tells a coherent story, using the shots generated in the previous challenge.
- The final assembled video is free of jarring cuts, ridiculous transitions (no star wipes!) or continuity errors.

### Tips

- [Google Vids](http://vids.google.com) is a great and free service for editing videos.

## Challenge 5: Giving It a Voice

### Introduction

A silent film can be powerful, but a voice-over can deliver a targeted message. In this challenge, we’ll generate professional-sounding voice-overs for your ad. To make your Visit Philly campaign global-ready, at least one voice-over must be in a foreign language.


### Description

First, write a short, compelling script for your ad. The script should consist of multiple pieces of voice-over audio to be inserted into your ad in different spots. The script should align with the brand guidelines you've defined.

> [!NOTE]  
> Once again, Gemini is fair game to generate the script, but you're also free to use your own writing creativity.

Next, use the *Chirp 3 HD* model in Vertex AI or the *Gemini TTS* model to generate the voice-overs from your script. Choose one of the voice-overs and generate it in a foreign language, (e.g. Italian, Afrikaans, Turkish).

Finally, add these audio tracks to the video you assembled in Challenge 4 in the proper places in your video sequence timeline.

### Success Criteria

- A short, on-brand script is written describing multiple voice-overs needed in the ad.
- Multiple high-quality voice-overs are generated with at least **one** in a foreign language.
- The voice-overs are successfully added to the video file, with timing that matches the visuals.

### Learning Resources

- [Prompting tips for Chirp 3 HD](https://docs.cloud.google.com/text-to-speech/docs/chirp3-hd#scripting-and-prompting-tips)
- [Prompting tips for Gemini Text to Speech](https://docs.cloud.google.com/text-to-speech/docs/gemini-tts#prompting_tips)

## Challenge 6: The Soundtrack

### Introduction

Music is an important layer of emotion in your ad. To complete your masterpiece, you will use Google's *Lyria* model to compose a custom piece of background music that complements the visuals and voice-over.

### Description

Using the *Lyria* model in Vertex AI, generate a music track for the entire ad. Remember to adhere to your brand guidelines.

Once you have a track you're happy with, add it as a final audio layer to your video sequence timeline. Make sure to balance the volume so that the music complements the voice-overs without overpowering them.

### Success Criteria

- A music track is generated for the entire length of the ad.
- The music's mood and style align with the brand guidelines.
- The music is successfully added to the video, creating a final, polished ad with visuals, voice-over, and a soundtrack.  
- You've exported your final ad as an **MP4** file.

### Tips

- Keep in mind that Gemini itself can be a helping hand here. If you give it your brand guidelines and/or your video, it can give you a recommendation for a good soundtrack to use.
- The Lyria model is trained from the point of view of a musician and their instrument. You'll get better results if your prompt speaks in the language of instruments.
