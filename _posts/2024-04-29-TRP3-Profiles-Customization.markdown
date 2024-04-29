---
layout:     post
title:      "Total RP 3 Profile Customization"
subtitle:   "A bit of a guide to the customization of TRP3's About section and various 'hidden' capabilities"
active: journal
image:
  feature: "pc_0011.png"
date:       2024-04-29
header-img: "img/postcover/pc_0011.png"
tags: [guide, addons, totalrp3]
categories: [warcraft]
comments: false
---

# Total RP 3 Profile Customization


#### Table of Contents

- [Image Position](#image-position)
- [Image Scale](#image-scale)
- [Links](#links)
- [Template Profile](#template-profile)
- [Other Notes](#other-notes)

This isn't really meant to be about how to use [Total RP 3](https://www.curseforge.com/wow/addons/total-rp-3), plenty of guides have been made about this already. This is actually aimed more at the customization side of a profile - what may make it catch your eye, and basically "how to make it pretty". This is of course mostly what works for me, and some examples of techniques. This also means that I'm not trying to make a "DO" and "DO NOT" list or anything like that - not unless it pertains to literally breaking the addon text formatting and the like.

## Image Position

There's a few techniques you can use to help with your textures - this is more of a basic rundown of some of them.

For this example I will use a basic texture: `{img:Interface\ACHIEVEMENTFRAME\UI-Achievement-Bling:128:128}`

<img loading="lazy" src="https://droppy.thebottom.net/$/3cVA5" alt="[PH]"/>

Typically this texture will be displayed displayed in the center of the About section. It's pretty basic. You have a tag indicating that it's an image, the image path which is found using the provided TRP3 browser *or* the [interface art export](#viewing-the-full-interface-art), and then some size coordinates for `XXX:YYY`. Icons are almost the same thing, however you may have noticed that they're treated like text. You can see this with this example, where the text and icon are on the same line and centered: `{p:c}{icon:ability_ambush:25}Your text here{/p}`

<img loading="lazy" src="https://droppy.thebottom.net/$/lXFEE" alt="[PH]"/>


Images can actually work similar, but they're also a bit different. At the end of the image code but still within the brackets, you can put in an l or r, for left and right. This would be an example of the above: `{img:Interface\ACHIEVEMENTFRAME\UI-Achievement-Bling:128:128:r}`

<img loading="lazy" src="https://droppy.thebottom.net/$/nstZv" alt="[PH]"/>

The texture should now placed on the right of the About section - notice that it seemingly appears within the same line as the text. However there are a few very key things to note - your placement of textures, and its "layering" upon the text is *generally* dependent upon which line comes first and how large the image is. This isn't always a guarantee as there's nothing that necessarily explicitly dictates this rule and I've heard others say they've seen it mess up, but I've personally not actually seen it happen. But it is something to keep in mind, and it is a low possibility subject to change in future patches.

## Image Scale

There are also additional things that can be used in unconventional ways. For example, aforementioned was the `XXX:YYY` size components. Typically if you want the image to look the way it does, you use the same ratio for its size - but there are some textures which work well to emulate separators / breaks when pushed to extremes. One example commonly found in the image browser are the pet battle textures. By squishing the Y value to extremely small values, you can produce what looks like a multi-colored line. In this example, I take the texture, give it a wide 512 pixel value, and then squish its height down to 3. Typically anywhere between 2-6 range tends to look decent. You can do this on any texture really, but the pet battle ones are a favorite and accessible from the TRP3 default browser: `{img:Interface\PETBATTLES\Weather-Sandstorm:512:3}`

<img loading="lazy" src="https://droppy.thebottom.net/$/F4nM7" alt="[PH]"/>

A combination of some of these working together can produce many different "elements" on themselves. This is an example of a "Title template" I made:

```
{img:Interface\PVPFrame\Icons\prestige-icon-8-1:64:64:l}{img:Interface\PVPFrame\Icons\prestige-icon-8-1:64:64:r}
{img:Interface\GLUES\Models\UI_NightborneElf\rg_shadow_elf:512:100:l}
{img:Interface\PETBATTLES\Weather-Sandstorm:512:3}
{h2:c}{col:ff3059}Title Text{/col}{/h2}
 
{img:Interface\PETBATTLES\Weather-Sandstorm:500:2}{img:Interface\PETBATTLES\Weather-Sandstorm:400:2}
```

<img loading="lazy" src="https://droppy.thebottom.net/$/3MNAh" alt="[PH]"/>

The first line places gem icons on the left and right sides. Then a shadowy backdrop texture found in [full interface art directory](#viewing-the-full-interface-art) is placed upon the left side, causing it to be its own layer beneath the following. The top of the title line is then established, followed by the text given a Header Title 2 set in the center and given some color. The text is put in, and then the color and header tags are closed. **This detail is crucial for the compatibility of other RP Profile addons and not breaking things. While it *may* continue to work on TRP3, it may not work well for other players. Always make sure to close the appropriate tags where necessary.**

A new line which is a just a space is now placed. This is literally just a space to space out the text from the bottom line. Then finally, 2 additional lines, one with a width fof 500 and one with a width of 400.

## Links

There are also other little tricks that can be done regarding links and colors. For example, you can custom-color a link by surrounding it in a color tag.

```
{col:a095db}{link*https://www.curseforge.com/wow/addons/total-rp-3-unit-frames*TRP3 Unit Frames}{/col}
```

<img loading="lazy" src="https://droppy.thebottom.net/$/oPQHb" alt="[PH]"/>

Colors are also retained outside of the tags if the text is on the same line, so you can revert back to the non-link color once added. This can save some space in your profile data size, which can be crucial to help lessen bandwidth usage as the bandwidth of addon data is actually quite limited and can often hit its limit in crowded events. An example of these combined:

```
{p:c}{col:ff0000}Some red text here {col:a095db}{link*https://www.google.com/*Link text here}{/col} Red text here{/col}{/p}
```


<img loading="lazy" src="https://droppy.thebottom.net/$/KyPZW" alt="[PH]"/>

I usually tend to just use 1 color per line as well, rather than attempting a gradient of individual characters. Sometimes it can look pretty, but it's also very difficult to read when editing, and also difficult to set up. Maybe hopefully one day a better built in method for gradients is implemented however. I tend to use [this tool](https://colordesigner.io/gradient-generator) to transition the colors of each line. It allows you to choose 2 colors, and generate a selection of "steps" between the beginning and end points. There are also various modes by which the color values "travel" from one point to another (around a color wheel vs. straight through it, etc.)


Links also don't always need to necessarily contain an actual website URL. In fact, the link text doesn't always need to be text - it can be set to an icon, but it can't be an icon and text or an image else it will appear as horrendous broken garbage. Additionally, the URL can only contain text and no images or icons, and additionally can't be colored to custom colors.

```
{p:c}Some text {link*Tooltip text here*{icon:ability_ambush:25}}{/p}
```

<img loading="lazy" src="https://droppy.thebottom.net/$/HPokN" alt="[PH]"/>

## Template Profile

Here is an example of a template profile I tend to use when making a character profile. I use it mainly as a guideline to fill out some basic and quick information. In my personal experience, players are more receptive to brief and clear details laid out in a profile. By no means is this a standard, in fact I would hope that you would vary your profile to be unique and not just copy mine - but it is something I want to provide as a resource to learn. I provide a History or timeline of their past - what events they may have attended for example. I then put in other details about the charcter - similar to the At First Glances, these explain things like general magic usage, experience with professions, character art links, and other details specific to the character. I then put in some Out of Character info about myself as a person - specific things that aren't *really* necessary to know such as RP experience, age range, or other specific things that may link outside of the game such as addons I made. I generally go into writing these not expecting players to read everything before walking into RP, so it's all considered extra. But that's also just my style of making a profile.

```
{img:Interface\GLUES\Models\UI_MainMenu_BurningCrusade\HellfireStars2:250:250:l}{img:Interface\GLUES\Models\UI_MainMenu_BurningCrusade\HellfireStars2:250:250:r}
{img:Interface\PETBATTLES\Weather-Rain:512:3}{img:Interface\GLUES\Models\UI_NightborneElf\rg_shadow_elf:500:70:l}
{h2:c}{col:b2fba5}History{/col}{/h2}
{img:Interface\GLUES\Models\UI_DemonHunter\Legion_Effect_Spin_01:512:512:l}
{img:Interface\PETBATTLES\Weather-Rain:512:3}
{icon:achievement_dungeon_outland_dungeonmaster:25}{col:d7f4d2} Placeholder.{/col}
{icon:inv_misc_quiver_03:25}{col:cef2c8} Placeholder.{/col}
{icon:spell_nature_natureguardian:25}{col:c5f0bd} Placeholder.{/col}
{icon:ability_druid_catform:25}{col:bceeb3} Placeholder.{/col}
{icon:inv_misc_herb_felweed:25}{col:b2eca8} Placeholder.{/col}
{icon:ability_druid_balanceofpower:25}{col:a9e99d} Placeholder.{/col}
{img:Interface\PETBATTLES\Weather-Rain:512:3}{img:Interface\GLUES\Models\UI_NightborneElf\rg_shadow_elf:500:70:l}
{h2:c}{col:b2fba5}Other Details{/col}{/h2}
{img:Interface\GLUES\Models\UI_MainMenu_BurningCrusade\HellfireStars2:250:250:l}{img:Interface\GLUES\Models\UI_MainMenu_BurningCrusade\HellfireStars2:250:250:r}
{img:Interface\PETBATTLES\Weather-Rain:512:3}
{icon:Ability_Hunter_SurvivalInstincts:25}{col:a0e793} Placeholder.{/col}
{icon:spell_nature_protectionformnature:25}{col:96e588} Placeholder.{/col}
{icon:ability_druid_treeoflife:25}{col:8ce27d} Placeholder.{/col}
{icon:ability_dualwield:25}{col:82e072} Placeholder.{/col}
{icon:ability_dualwieldspecialization:25}{col:77dd66} Placeholder.{/col}
 
{img:Interface\PETBATTLES\Weather-Rain:512:3:l}{img:Interface\PETBATTLES\Weather-ArcaneStorm:512:3}{img:Interface\GLUES\Models\UI_NightborneElf\rg_shadow_elf:500:70:l}
{h2:c}{col:ff6ca1}OOC{/col}{/h2}
{img:Interface\GLUES\Models\UI_MainMenu_BurningCrusade\HellfireStars2:250:250:l}{img:Interface\GLUES\Models\UI_MainMenu_BurningCrusade\HellfireStars2:250:250:r}
{img:Interface\PETBATTLES\Weather-Rain:512:3:l}{img:Interface\PETBATTLES\Weather-ArcaneStorm:512:3}
{p:c}{col:ffc8dd}Placeholder{/col}{/p}
{p:c}{col:f5c8e9}Placeholder{/col}{/p}
{p:c}{col:e6c9f4}Placeholder{/col}{/p}
{p:c}{col:d2ccfc}Placeholder{/col}{/p}
{p:c}{col:bbcfff}Placeholder{/col}{/p}
{p:c}{col:a2d2ff}Placeholder{/col}{/p}
{img:Interface\PETBATTLES\Weather-Rain:512:3:l}{img:Interface\PETBATTLES\Weather-ArcaneStorm:512:3}{img:Interface\GLUES\Models\UI_NightborneElf\rg_shadow_elf:500:100:l}
```



<img loading="lazy" src="https://droppy.thebottom.net/$/UrSrG" alt="[PH]"/>

## Other Notes

#### Viewing The Full Interface Art

<details>
<summary> ► Read More</summary>

By default TRP3 only really has a texture browser for a select list of decent interface textures, and for good reson. Most other interface elements are just atlases or pieces of frames that don't generally look great. Until the possible day of a whole rework of how the About section handles textures (and maybe even the introduction of Atlases and/or using file data ID in addition to texture paths), this is also unlikely to really change. However, there are a few other small images that can be found elsewhere not included in this curated list one may find appealing.

There's multiple ways to go about viewing the interface art. I've provided <a href="https://github.com/keyboardturner/wow-ui-art/tree/retail_png">my own repo</a> where I've already exported and converted the files. You can just use the button labelled as <code><> Code</code> and select <code>Download ZIP</code> then extract the files to view them in your file explorer. Notice that the branch selected at the top is called <code>retail_png</code>.

A few other resources similarly exist, though they may not be very convenient, fast, or simply not updated - but it does come down to personal preference. <a href="https://github.com/Gethe/wow-ui-textures">Gethe's WoW UI Textures</a> is an outdated resource I used to use some time back, but it was discontinued and hasn't been updated for Dragonflight. My project is basically the same.

You can alternatively use other file browser applications such as <a href="https://github.com/WoW-Tools/CASCExplorer/releases">CASCExplorer</a>, <a href="https://www.kruithne.net/wow.export/">wow.export</a>, or <a href="https://github.com/Marlamin/wow.tools.local">wow.tools local</a>, but these are more for extracting raw files. Useful tools to have, but for this purpose they may not be convenient.
</details>


#### Exporting Interface Files Yourself

<details>
<summary> ► Read More</summary>

If you want to be more self-reliant, you can export the game's interface art files yourself, and it's actually fairly easy to do and even supported by Blizzard's own game rather than using third party software. This is the list of all named texture files, which is also the list of textures TRP3's about section supports.

When you open the game launcher, the gear icon next to the Play button has a Game Settings option. A checkbox for "Additional command line arguments" can be checked, allowing you to enable console access. Put <code>-console</code> into the text input of this checkbox and launch the game. Generally the console is opened via the <a href="https://en.wikipedia.org/wiki/Backtick">backtick / grave accent key</a>. This is the easiest, most user-friendly way to do this. Other methods can be found <a href="https://warcraft.wiki.gg/wiki/Console#Running_the_client_with_the_-console_flag_enabled">here</a>.

Once the console appears, you'll be able to put in the following to begin exporting the files: <code>ExportInterfaceFiles art</code>. The game client may freeze up for a minute or two depending on your computer hardware write speed. It's pretty normal, it's literally exporting thousands of files as fast as it can.

From here, you can navigate to your WoW folder directory, which can also be easily found from the same gear icon on the launcher by selecting "Show in Explorer". Inside the highlighted client folder (usually <code>_retail_</code>) is a new folder called "BlizzardInterfaceArt". I'd also recommend possibly moving this folder into a new location that you don't mind taking up a lot of space. This folder contains a whole slew of other directories and images, but there's a few issues that may become immediately apparent - all these files are in a .blp format. There are some tools people have made to convert these files into .png format, such as <a href="https://www.wowinterface.com/downloads/info6127-BLP2PNG.html">BLP2PNG</a>, where you can drag files or even folders onto the .exe provided in the download link. It will also convert .png back into .blp, primarily only useful for addon devs (hence it being an addon dev resource tool). I however actually use a different program, but I only use it for converting .blp into .png and *not* the other way around. This program is called <a href="https://www.wowinterface.com/downloads/info22128-BLPNGConverter.html">BLPNG Converter</a> - it provides a nice small interface and additional progress bar. It will automatically skip anything it can't convert as well, so no need to worry about accidentally converting non-.blp files.

From here, that's pretty much the whole process. Every major patch tends to add in new textures, but they're typically just icons or other assets that wouldn't display nicely, hence why I made <a href="https://github.com/keyboardturner/wow-ui-art/tree/retail_png">my own repo</a> to track differences during major patches.

</details>

#### Unicode Characters

I tend to generally avoid unicode characters not normally found on a standard keyboard. Most of the time things like dots and such should work fine for most normal users, but bear in mind that any user who has an addon which changes their default game font may not be able to see the characters placed in. That means things like <a href="https://lingojam.com/FullWidthTextGenerator">full width characters</a> or <a href="https://lingojam.com/VaporwaveTextGenerator">other symbols and emojis</a> will appear as boxes to them. There's no way to choose the font you want to present your text in to other players, it uses the Blizzard default fonts, but sometimes players do replace those fonts with ones that don't support various unicode.

#### Backing Up Profiles Automatically

Something else to also have which is useful is backing up your addon data automatically using a cloud service. This is especially useful in case your profiles wipe, and not just for Total RP 3. A useful write-up guide for this can be found on the <a href="https://github.com/Total-RP/Total-RP-3/wiki/How-to-backup-and-synchronize-your-add-ons-settings-using-a-cloud-service">Total RP 3 Wiki</a>.

## Some Example Images

Below are a handful of handpicked textures that can be found in the Glues folder:

<details>
<summary> ► Read More</summary>

Some of these can be rescaled to be be wider, or purposefully stretched to make a "blurred" backdrop.

<code>{img:Interface\Calendar\EventNotification:128:128}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/9eiK4" alt="[PH]"/>


<code>{img:Interface\Calendar\Holidays\Calendar_HarvestFestivalOngoing:128:128}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/kJo9x" alt="[PH]"/>

<code>{img:Interface\CastinBar\UICastingBarChannelMask:128:128}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/zzZnN" alt="[PH]"/>

<code>{img:Interface\Challenges\challenges-background:512:512}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/LfUUr" alt="[PH]"/>

<code>{img:Interface\CHARACTERFRAME\TemporaryPortrait-Female-Gilnean:64:64}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/om3lz" alt="[PH]"/>

<code>{img:Interface\COMMON\bluemenu-goldborder-horiz:64:128}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/Mlpdh" alt="[PH]"/>

<code>{img:Interface\CovenantRenown\DragonflightMajorFactionsPlunderstormBackground:1024:1024}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/lajsi" alt="[PH]"/>

<code>{img:Interface\ENCOUNTERJOURNAL\UI-EJ-BACKGROUND-ArcaneVaults:512:512}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/iW1Uq" alt="[PH]"/>

<code>{img:Interface\Mount\Motionsicknesspart4:2048:2048}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/YpqOM" alt="[PH]"/>

<code>{img:Interface\PLAYERFRAME\MonkDragonBar:256:128}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/yVznb" alt="[PH]"/>

<code>{img:Interface\Timer\Alliance-Logo:256:256}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/jzEtu" alt="[PH]"/>

<code>{img:Interface\Timer\Challenges-Logo:256:256}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/Jc3Mm" alt="[PH]"/>

<code>{img:Interface\Timer\Horde-Logo:256:256}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/CvY6D" alt="[PH]"/>

<code>{img:Interface\GLUES\Models\UI_PIRATE\UI_PIRATE\UI_Pirate_Clouds:1024:512}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/5eVUB" alt="[PH]"/>

<code>{img:Interface\GLUES\Models\UI_PandarenCharacterSelect\tu_fallingPetals_Red:256:256}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/bBNbu" alt="[PH]"/>

<code>{img:Interface\GLUES\Models\UI_NightborneElf\rg_shadow_elf:256:256}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/FaHuF" alt="[PH]"/>

<code>{img:Interface\GLUES\Models\UI_MainMenu_BurningCrusade\HellfireStars2:256:256}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/Mom9X" alt="[PH]"/>

<code>{img:Interface\GLUES\Models\UI_DemonHunter\Legion_Effect_Spin_01:256:256}</code>

<img loading="lazy" src="https://droppy.thebottom.net/$/TU6XD" alt="[PH]"/>





</details>
