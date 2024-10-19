---
layout:     post
title:      "Nonami - Bard / Rogue"
subtitle:   "The work in progress of making artwork for a human model character, and exploration into some unique hair modelling."
active: journal
image:
  feature: "pc_0008.png"
date:       2023-12-24
header-img: "img/postcover/pc_0008.png"
tags: [art, nonami]
categories: [warcraft]
comments: false
gallery00001: 
  - image_path: https://kbt.thebottom.net/upload/2024/10/16/20241016231159-2fba1c49.png
    image-caption: Nonami Bard - Portrait
    image-copyright: © Keyboardturn
  - image_path: https://kbt.thebottom.net/upload/2024/10/16/20241016231205-5e93c21b.png
    image-caption: Nonami Bard - Full
    image-copyright: © Keyboardturn
  - image_path: https://kbt.thebottom.net/upload/2024/10/16/20241016231211-e1976917.png
    image-caption: Nonami Bard - Reference Sheet
    image-copyright: © Keyboardturn
---

# Nonami - Bard / Rogue

<!-- Gallery __-->
      
{% include subgallery.html id="gallery00001" %}

<!-- end of GALLERY __ -->

I just wanted to make something for my human rogue character. I never really felt like the in-game customization options gave me the look I really wanted.

This took a ton of time to make, particularly as I put a lot of work into the body, a new hair system, reworked parts of the ship UV, and completely made the guitar custom.

Below are some work in progress projects I made along the way.

Here I had experimented with trying to get a particular outline look using curves paired with a mesh+texture to emulate WoW hairstyles. This testing was first done on a Void Elf.

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231317-425568b6.webp" alt="[Model Viewer preview of a Void Elf with distinct purple hair. The hair has a black outline border along the geometry, producing an almost painted outline effect similar to video game art styles such as the Borderlands series. The outline effect may be called Sobel operator, though this was not the exact method used in the image.]"/> <!-- blenderpreview1 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231318-8be33a04.webp" alt="[Model viewer preview of a Void Elf wtih distinct purple hair. This is another angle provided to the image before, highlighting a view looking down at the hair and showcasing the many black outline ridges of the hair geometry.]"/> <!-- blenderpreview2 -->

I then attempted a slightly different method, combining the outline method with a fading texture to give the ends a softer look. However, I didn't feel that this actually captured the "Warcraft" style that I wanted to keep. This instead could potentially be used for something like FFXIV renders.

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231318-7ed228a5.webp" alt="[A different effect employed upon the Void Elf hair, displaying the ends of the hair against the back of the body. The hair dapers off and fades with an almost brush-like effect similar to how realistic hair is done, which is very markedly from WoW's style of geometric hair.]"/> <!-- blenderpreview3 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231319-a66ccd17.webp" alt="[Another angle of the effect shown in the previous image, this time showcasing a fringe/bangs hairstyle along the side profile shot of the Void Elf character. The hair produces a realistic effect near the ends.]"/> <!-- blenderpreview4 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231319-05e184a4.webp" alt="[A front view of the hairstyle shown previously. One side of the hairstyle has longer hair, while the other side is unfinished. The hairstyle is clean and realistic, contrasting to the Warcraft stylization of the Void Elf model which the hair rests upon.]"/> <!-- blenderpreview5 -->

From here I decided to begin testing with purely curves without outlines, but making each "strand" significantly smaller but still closely matching the silhouette of the WoD-era hairstyles.

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231320-c4ae4b48.webp" alt="[Work made overlaying a base hairstyle with newer purple hair pieces. The new hair roughly follows the same direction and style as the old hairstyle. The old hairstyle is colored black and grey, and is visibly lower polygon and lower texture resolution.]"/> <!-- blenderpreview6 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231320-361df00e.webp" alt="[A more complete version of the previous hairstyle, with the hair now changed to a darker natural brown.]"/> <!-- blenderpreview7 -->

A comparison between the two:

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231321-d1b65889.webp" alt="[A similar image to the last, comparing the old hairstyle and its general silhuoette. The hairstyle is noticeably lower in polygon and texture resolution.]"/> <!-- blenderpreview8 -->

I then implemented one more technique, which I believe particularly helps make a hairstyle look modern without deviating too much from the "Warcraft" technique, which I had planned from the start of using the curves and converting to mesh later on: Splitting the ends of the hair pieces.

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231322-f7294a7f.webp" alt="[End parts of the newer hairstyle, displaying split geometry to the hair. Each part of split into 3 pronged ends. The hairstyle is currently placed on a Void Elf, despite the hairstyle belonging to the human model.]"/> <!-- blenderpreview9 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231322-a74c6fc0.webp" alt="[A larger view of the overall split ends. The effect produces the same effect as Warcraft's style, but seemingly with even more polygons and pieces.]"/> <!-- blenderpreview10 -->

I further then began working on the human model a bit, and began testing out some textures. I incidentally made a very skin texture that worked particularly well to look high quality without sacrificing the original painted details of the skin. I turned up the reflectivity to better show the smaller details (or what the skin could otherwise look like when wet vs. dry).

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231323-0e3159ed.webp" alt="[A human model displaying reflective eyes, smoothed skin texture, and a faint skin shader that appears as a sort of bump map. The small detail of the skin shader produces a more detailed effect upon the skin, as though skin pores are catching light and producing shadows.]"/> <!-- blenderpreview11 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231323-16466db2.webp" alt="[A similar image to the last, however this time displaying the skin shader as much more reflective similar to the eyes. The reflectivity makes it appear as though it the skin is wet, contrasting to the dryer effect previously.]"/> <!-- blenderpreview12 -->

I then began working on the Guitar model. This was actually a bit of an [older project](https://twitter.com/keyboardturn/status/1389332750730027017) that I revisited. I reworked some significant parts of the new model though, replacing the headstock and neck, reworking the body UV and textures, and giving each string a varying size.

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231324-36e5d28d.webp" alt="[An image of a basic guitar in Blood Elven (Thalassian) style. The guitar has a red-brown wooden textured body and golden metalltic border. There are 6 strings lined across the body, from left to right displaying a thicker string to a thinner string.]"/> <!-- blenderpreview13 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231325-8c9ec491.webp" alt="[A newer iterated version of the guitar, displaying an even redder hue to the body and edges. The angled headstock notably includes tuning pegs rotated randomly, with 4 on the left side and 2 on the right side. Each tuning peg is detailed with a small anchor design.]"/> <!-- blenderpreview14 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231325-a4f006d8.webp" alt="[Another angled view of the guitar, displaying the neck and strings. The strings are noticeably of varying shape, ranging from larger to smaller from left to right.]"/> <!-- blenderpreview15 -->

Eventually I reworked and custom created the tuning pegs, although I did steal the anchor from Jaina's necklace to place as detail. My character hails from the seas, so having a guitar with an anchor design makes sense.

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231326-476ebae3.webp" alt="[A singular tuning peg, displaying a different style that reduces the anchor size to look as though the peg can be gripped easier.]"/> <!-- blenderpreview16 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231326-b1ea4b1d.webp" alt="[All 6 tuning pegs in their default, non-rotated positions along the headstock of the guitar. Each one is evently spaced on each side]"/> <!-- blenderpreview17 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231327-8ad5a7d4.webp" alt="[Another angle of the same headstock, this time from the front showing the pegs lining up to the cylinders that run through the headstock and connect to each string.]"/> <!-- blenderpreview18 -->

I then returned back to the character model, this time to create an armature skeleton for the hair. The skeleton is actually separate from the model, and as it's also an armature, I should be able to technically reshape it to fit any character model, extend/detract its length, and so on. This makes the hairstyle incredibly malleable to be used in all future projects. Although it was time-consuming to create, it'll be a resource I'll be able to use in my future projects for a long time to come.

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231328-afec6245.webp" alt="[The newer hairstyle placed upon the human model, displaying the bare armature (skeleton) used to control the hair.]"/> <!-- blenderpreview19 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231328-d1062c94.webp" alt="[The hairstyle now posed in wild directions with the armature now hidden. The hairstyle is purposefully posed to show the versatility of the hair, no longer being constrained by the weight of the body.]"/> <!-- blenderpreview20 -->

An example of the same hairstyle with different scaled bones to give it a long or short appearance.

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231329-2f27b745.webp" alt="[The same hairstyle, this time lengthened using the armature. The hair retains its general same style, but now extends beyond the shoulders and can cover one of the eyes.]"/> <!-- blenderpreview21 -->

<img loading="lazy" src="https://kbt.thebottom.net/upload/2024/10/16/20241016231329-2924598b.webp" alt="[The same hairstyle, this time shortened using the armature. The hair retains its general same style, but now rests at a length above the shoulders along the jaw and chin.]"/> <!-- blenderpreview22 -->

In a later addition, I also applied basic real-time physics to the hair skeleton to try and give it some life. It's however still a heavy work-in-progress with a lot of clipping and no collision regions set up, but it was an interesting experiment.

<video loading="lazy" width="100%" controls loop>
  <source src="https://kbt.thebottom.net/upload/2024/10/17/20241017202347-37bdeaf2.mp4"> <!-- hairtest1 -->
  Your browser does not support the video tag or is currently unavailable.
  [Alt: A video displaying a wavy physics effect upon the hair controlled by the armature. The hair tends to clip slightly into the human model shoulder. The human model looks around, animated in one of the default game poses.]
</video>

<video loading="lazy" width="100%" controls loop>
  <source src="https://kbt.thebottom.net/upload/2024/10/17/20241017202344-624a139e.mp4" type="video/mp4" type="video/mp4"> <!-- hairtest short -->
  Your browser does not support the video tag or is currently unavailable.
  [Alt: A video displaying a wavy physics effect upon the hair controlled by the armature. Because the hair is shorter, it tends to clip less with the body of the model. The human model looks around, animated in one of the default game poses.]
</video>

From here, it was just a matter of posing the character to place into the scene and adjust lighting, which can now be seen in the end result.

<img loading="lazy" src="https://droppy.thebottom.net/$/Uy5RW" alt="[A full quality wide screen view of the newer artwork, displaying a feminine human character dressed in a v-shaped tunic, flower wrist, and flower crown. The human character is holding a guitar. As the character plays, highlighted golden notes and pink ember effects appear in the background. The entire background is lightly blurred, displaying the cabin of a ship, including a navigator globe, table wtih ink and paper, and blue lit windows. The scene is generally darkened in the background. The foreground is much clearer, specifically focusing on the character's face, while parts of the guitar and hand which display closer are slightly out of focus.]"/> <!-- FullRender CombineSigned -->

<img loading="lazy" src="https://droppy.thebottom.net/$/Up1im" alt="[The same image as before, but now cropped in a portrait view specifically focusing on the face. The rest of the background is blurred, while displaying a closer detailed view that highlights the soft shading of the face shape.]"/> <!-- FullRender CombinePortraitSigned -->