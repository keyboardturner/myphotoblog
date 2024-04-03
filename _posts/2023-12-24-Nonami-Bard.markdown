---
layout:     post
title:      "Nonami - Bard / Rogue"
subtitle:   "Keyboardturner"
active: journal
image:
  feature: "pc_0008.png"
date:       2023-12-24
header-img: "img/postcover/pc_0008.png"
tags: [art, nonami]
categories: [warcraft]
comments: false
gallery1: 
  - image_path: /gallery/archive/g00001/FullRender_CombinePortraitSigned.png
    image-caption: Portrait
    image-copyright: © Keyboardturn
  - image_path: /gallery/archive/g00001/FullRender_CombineSigned.png
    image-caption: Full
    image-copyright: © Keyboardturn
  - image_path: /gallery/archive/g00001/RefSheetViews.png
    image-caption: Reference Sheet
    image-copyright: © Keyboardturn
---

# Nonami - Bard / Rogue

<!-- Gallery __-->
      
{% include subgallery.html id="gallery1" %}

<!-- end of GALLERY __ -->

I just wanted to make something for my human rogue character. I never really felt like the in-game customization options gave me the look I really wanted.

This took a ton of time to make, particularly as I put a lot of work into the body, a new hair system, reworked parts of the ship UV, and completely made the guitar custom.

Below are some work in progress projects I made along the way.

Here I had experimented with trying to get a particular outline look using curves paired with a mesh+texture to emulate WoW hairstyles. This testing was first done on a Void Elf.

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview1.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview2.png" alt="[PH]"/>

I then attempted a slightly different method, combining the outline method with a fading texture to give the ends a softer look. However, I didn't feel that this actually captured the "Warcraft" style that I wanted to keep. This instead could potentially be used for something like FFXIV renders.

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview3.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview4.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview5.png" alt="[PH]"/>

From here I decided to begin testing with purely curves without outlines, but making each "strand" significantly smaller but still closely matching the silhouette of the WoD-era hairstyles.

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview6.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview7.png" alt="[PH]"/>

A comparison between the two:

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview8.png" alt="[PH]"/>

I then implemented one more technique, which I believe particularly helps make a hairstyle look modern without deviating too much from the "Warcraft" technique, which I had planned from the start of using the curves and converting to mesh later on: Splitting the ends of the hair pieces.

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview9.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview10.png" alt="[PH]"/>

I further then began working on the human model a bit, and began testing out some textures. I incidentally made a very skin texture that worked particularly well to look high quality without sacrificing the original painted details of the skin. I turned up the reflectivity to better show the smaller details (or what the skin could otherwise look like when wet vs. dry).

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview11.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview12.png" alt="[PH]"/>

I then began working on the Guitar model. This was actually a bit of an [older project](https://twitter.com/keyboardturn/status/1389332750730027017) that I revisited. I reworked some significant parts of the new model though, replacing the headstock and neck, reworking the body UV and textures, and giving each string a varying size.

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview13.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview14.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview15.png" alt="[PH]"/>

Eventually I reworked and custom created the tuning pegs, although I did steal the anchor from Jaina's necklace to place as detail. My character hails from the seas, so having a guitar with an anchor design makes sense.

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview16.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview17.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview18.png" alt="[PH]"/>

I then returned back to the character model, this time to create an armature skeleton for the hair. The skeleton is actually separate from the model, and as it's also an armature, I should be able to technically reshape it to fit any character model, extend/detract its length, and so on. This makes the hairstyle incredibly malleable to be used in all future projects. Although it was time-consuming to create, it'll be a resource I'll be able to use in my future projects for a long time to come.

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview19.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview20.png" alt="[PH]"/>

An example of the same hairstyle with different scaled bones to give it a long or short appearance.

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview21.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/blenderpreview22.png" alt="[PH]"/>

From here, it was just a matter of posing the character to place into the scene and adjust lighting, which can now be seen in the end result.

<img loading="lazy" src="/assets/images/nonami_bard/FullRender_CombineSigned.png" alt="[PH]"/>

<img loading="lazy" src="/assets/images/nonami_bard/FullRender_CombinePortraitSigned.png" alt="[PH]"/>