---
layout:     post
title:      "An Extensive Fishing Overhaul"
subtitle:   "Keyboardturner"
active: journal
image:
  feature: "pc_0009.png"
date:       2024-02-26
header-img: "img/postcover/pc_0009.png"
tags: [feedback, fishing]
categories: [warcraft]
comments: false
---

# An Extensive Fishing Overhaul


In this write-up I wanted to provide some feedback on the fishing system and how I'd like to see it redesigned. I felt like while fishing got some interesting systems in Dragonflight (such as the harpoon and tuskarr stuff), it was lacking in depth where other gathering professions had talents and trees to utilize. I've tried to organize my thoughts as best as I can, there's probably some details I didn't include or left ambiguous. Overall, this is what I envision Fishing can be as a fun and engaging profession while still maintaining its relaxing gameplay style. This is somewhat meant to be an expansion-agnostic base idea that could be iterated upon later.



### **Equipment**

New types of fishing rods (tools):



* **Spinning Rods**: These basically replace the old style fishing rod. They’re standard and can be used in all types of fishing, but won’t yield you the maximum amount of skill. This is basically to keep old style fishing accessible without locking it out.
* **Casting Rods**: These are primarily used to target freshwater fishing areas. This _usually_ is inland, but not always (some places have saltwater regions inland, and perhaps some secret freshwater fish can be found in the ocean?)
* **Surf Rods**: These are for saltwater fishing. Primarily this will target the seas. Like the casting rod, you can try to use this in freshwater areas for secret fish, but the heavy lines and lures may be too intimidating for most normal freshwater fish. These rods will also be specifically relevant to fishing tours.

All of these rods can be transmogged between each other, but for the purposes of mechanics, they remain separate. It’s essentially like transmogging swords, maces, and axes. Typically the stats will be random or targetable, like other gathering tools.

Additional fishing equipment slots:



* **Hats**: Like other gathering equipment, these will have Deftness and Perception. Some higher level gear will have additional fishing skill, similar to older helms. However the stats will be much more valuable than the skill in the vast majority of cases.
* **Boots**: Unlike other gathering professions, fishing uses boots instead of a backpack. However, the boots will still have finesse.

The fishing equipment transmog will utilize cosmetic slot items, such as being hidden, heritage armor, or other items such as glasses. Likewise, all fishing gear will be cosmetic to be transmogged over normal player armor.

Stats would also ideally come into play similar to how they currently work for other gathering professions. Skill affects the baseline gather quality where applicable, Finesse allows capturing more fish, Deftness increases the speed of a fishing cast, and Perception allows a chance of rare fish. Fish have varying qualities, which ultimately affect other professions which may reasonably use them such as alchemy and cooking.


### **Abilities**

When engaged in fishing mode, the main action bar will be replaced similar to when mounted on a dynamic flight mount. The amount of abilities won’t be large, and engaging in combat (any time the player attacks) will revert the action bar to its default state.

4 Primary Abilities:



* **Cast**: The typical fishing spell. It casts the line.
* **Snag**: This is essentially the old style of “loot”. It’s equivalent to clicking the bobber with old equipment, but it’s set up in a way that also allows the player to “automate” clicking the bobber, similar to how some addons such as Better Fishing allow for.
* **Haul**: This is likely a “standard” catch size for the majority of the new fishing mode. It’ll typically have your standard fish at low quality. Stats of course come into play with quality/quantity of fish.
* **Bounty**: This is a larger (and rarer) catch, it indicates rare materials or extra-bountiful catches.

**Addons shouldn’t be able to distinguish which ability is needed**. Technically, you could set up a macro (or an addon button/keybind in the middle of the screen) to automate reeling in the catch, but there will be a major downside that it can’t possibly know which proper ability to use, as using the incorrect ability causes the fish to slip off the hook. This is essentially the same as it is now, but with more mechanics in place. You could technically set up an addon to have a button which becomes active that clicks the bobber at around ~7.5 seconds after casting fishing, but it will only ever get a small portion of the actual casts. It’s just inefficient and bad. Only lazy fishing bots would do this and at that point is an obvious bannable offense.

**A fishing catch is indicated in 3 main ways** - the bobber shaking, the sound, and a new fish hook icon which temporarily appears above the player character’s head. The icon should never show to other players for the sake of immersion and lessening confusion to prevent accidentally reeling in other catches. Each icon, sound, and bobber shaking for each reel in type would be different. The larger the catch, the more hefty the sound, intense the shaking, and intense the icon is (3 hooks with maybe a pair of intimidating eyes or tentacles or something). In addition, a new reeling-in animation for the player model could play when reeling in, giving a feel to the size of the catch caught. It should feel almost like an intense battle if you catch the largest fish.

A new UI Widget akin to the dragonriding vigor bar will be displayed, with the resource being called **Tidal Essence**. It is built up from 0 by your Snag, Haul, and Bounty abilities, similar to generating Rage. It will deteriorate over time upon exiting fishing mode, so if the player engages combat they should aim to kill the creature as quickly as possible if they don’t want to lose all their Tidal Essence.

Additional abilities:



* **Cutbait**: This can typically be used on higher quality Common and Uncommon fish. It is used to catch even larger Rare and Epic fish. This can only be used on the most recently-caught fish within a 1 minute time limit. Canceling fishing mode also cancels the ability to use the fish. The fish is also consumed in the process. This would use a medium-to-small amount of Tidal Essence, scaling with other talents and gear.
* **Neptulon’s Grace**: You exchange Tidal Essence for a temporary duration increase in your stats. This can be Finesse, Perception, or Deftness. It should use a large-to-medium amount of Tidal Essence.
* **Tidemother’s Gratuity**: This allows you to essentially multi-reel in Snag, Haul, and Bounty casts. The cast still needs to result in a fishing bobber being ready, but it will be a special ability you can use. This would use nearly the maximum amount of Tidal Essence. Although in most cases a player will likely use this on a Bounty reel, there may be cases where using it on a Haul or Snag may actually be more worthwhile.

These abilities essentially create a layer of a build/spend system, they aren’t really _required _to fish, but they’d go a long way in adding a level of engagement and participation for those who are invested in the system. So it’s not like a player needs to know complexities in a system just to get a quest item.



### **Specializations**

**Angler**

Generalized fishing trails for quality of life and core fishing skill buildup.

&nbsp;&nbsp;&nbsp;&nbsp;Primary Trait: **Angler**



* Grants fishing skill for every point spent.

  - 5: **Surface Tension**: Walk on water.

  - 10: Learn **Sub-Specialization**

  - 15: Learn to **Refine Filet (Rank 2)**

  - 20: Learn **Sub-Specialization**

  - 25: Learn to **Refine Filet (Rank 3)**


    Sub-Specialization: **Rafting**



* Grants fishing skill for every point spent. While in fishing mode and while walking on water, gain a raft that allows you to travel across water faster. Deftness increases the speed of the raft.

    - 5: Finesse decreases the deceleration rate of the raft.


    - 10: Fishing while rafting grants 5 Perception.


    - 15: **Wave Hop**: Dash forward 20 yds on the raft, incapacitating enemies and allowing you to retain the raft while on land for the duration of the dash. (If Underlight Blessing is learned, allow usage of Wave Hop while swimming)


  Sub-Specialization: **Way of the Flounder**



* Grants fishing skill for every point spent. While in fishing mode, reduce the range at which enemies can detect you. Finesse improves this effect. (Canceled when moving)

    - 5: No longer canceled by movement.


    - 10: Fishing while sneaking grants 5 Finesse.


    - 15: **Underlight Blessing**: Become a fish when underwater, allowing water breathing and rapid swim speed. (If Wave Hop is learned, allow usage of Wave Hop while swimming)


**Bounty Fisher**

A specific focus on abundance of fish.

&nbsp;&nbsp;&nbsp;&nbsp;Primary Trait: **Fisher Friends**



* When within 100 yards of other fishing players, gain the Fisher Friends buff. While this is active, your current fishing pool has a chance to explode, providing a buff to all players within 100 yards for a higher chance to catch fish from that pool.

    - 5: Learn **Multi-Hook (Rank 1**): Allows hooking two kinds of fish in one catch.


    - 10: Increase Finesse


    - 15: Unlock choice of Primary Trait: **Freshwater Schools** or **Saltwater Schools**.


    - 20: Increase Perception


    - 25: Learn **Multi-Hook (Rank 2)**: Allows hooking three kinds of fish in one catch.

\
    Primary Trait: **Lone Lure**

* When not within 100 yards of any other fishing players, you have a chance to barrel up fishing nodes instantly. Is negated if the Fisher Friends trait is active.
* - 5: Learn **Multi-Bait (Rank 1)**: Allows use of two kinds of bait at once.

    - 10: Increase Deftness


    - 15: Unlock choice of Primary Trait: **Freshwater Schools** or **Saltwater Schools**.


    - 20: Increase Finesse


    - 25: Learn **Multi-Bait (Rank 2)**: Allows use of three kinds of bait at once.


    Primary Trait: **Freshwater Schools**


    Having a bait equipped for Freshwater regions allows you to see schools of these fish.


  - 5: Freshwater schools can be seen with Fish Eyes.


    Primary Trait: **Saltwater Schools**


    Having a bait equipped for Saltwater regions allows you to see schools of these fish.


    - 5: Saltwater schools can be seen with Fish Eyes.


    **Fish Eyes**: Toggle on to see distant pillars in the sky indicating rare fish locations from afar.

**Specialty Tackler**

Focuses on baits, rare fish, and elemental fishing.

&nbsp;&nbsp;&nbsp;&nbsp;Primary Trait: **Ghostfish Getaway**



* If you are fishing and engage in combat suddenly, you break free from all effects which cause loss control of your character and spontaneously gain invisibility. (2 minute cooldown) (If Underlight Blessing is learned, you remain in stealth if used while swimming until Underlight Blessing wears off)

    - 5: Unlock **Sub-Specialization**


    - 10: Increase Perception when using bait. 


    - 15: Unlock **Sub-Specialization**


    - 20: Increase Finesse when using bait.


    Sub-Specialization: **Tidal Charging**

* Gain tidal essence while your bobber is within a school of fish or when you are benefiting from Fisher Friends.

    - 5: Your passive health and resource regeneration are greatly increased while fishing


    - 10: Increase Deftness


    - 15: You have a chance to gain extra Tidal Essence outside of schools of fish


    Sub-Specialization: **Reeling Refund**

* Each catch has a chance to refund bait used. Perception increases the chance of refund.

    - 5: Bait duration increased by 50%


    - 10: Increase Perception


    - 15: Bait duration increased by 100%



### **Elemental Fishing**

For the majority of our fishing experiences, we’ve been more or less familiar largely with aquatic fishing, and a little bit of lava fishing every now and then. These two pretty much make up 2 of several types of fishing, representing the elements of Water and Fire. However, there are other forms of fishing that can be introduced:



* **Skyfishing (Air)**: Many of the tallest peaks and mountaintops hold secret migrations of skyfish. They often elusively sift through the clouds, hiding within and absorbing nutrients ambiently. Some of the regions they can be found at are the tallest regions of Hyjal, Blackrock Mountain, Storm Peaks, Kun-Lai Summit, Highmountain, Drustvar, and Zuldazar.
* **Sandfishing (Earth)**: Sandfish spontaneously emerge during certain seasons of the year. They exist within the ever-shifting deserts of the world, such as Tanaris, Uldum, Vol’dun, and some smaller select areas like Bronze Dragonshrines.
* **Netherfishing (Magic)**: This covers anomalous areas of fishing. Some fish (and fish-like creatures) reside between the dimensions of magical realms. These sorts of fish can often be found in the outer edges of Outland, Argus, the Shadowlands, and a few other areas steeped in magical energy.
* **Deep Sea Fishing (Water)**: This covers fishing in regions where you’re allowed to stand on the seabed. These fish rarely ever can be caught from the surface regions of the world. Some zones include areas such as Vashj’ir, and the dive bars of Kul Tiras, Zandalar, Nazjatar, Exile’s Reach, and the Dragon Isles.


### **Bait**

Baits (and tackle) are all instead hidden currency items that will be added to a tacklebox storage UI (possibly accessible automatically upon entering fishing mode or via fishing journal). Bait items that currently take up bag space will now have an on-use effect to convert onto the currency. This also helps with buying/selling the items on the auction house. As the system grows larger with more fish and inevitably more bait items, they would end up consuming more bag space. Conversion into a hidden currency keeps bags free, the real currency tab less cluttered, and placing the information in a more relevant location.


### **Catch Conditions**

Three primary conditions can come into play for catching particular fish - time of day, season, and weather. The use of specific baits and skills can negate some of these conditions in a limited capacity.

Time of day for a particular fish comes in 4 states:



* 00:00 to 06:00: [Fish] has a chance to be caught at its full potential.
* 06:00 to 12:00: [Fish] has a chance to be caught at half its potential.
* 12:00 to 18:00: [Fish] has no chance of being caught.
* 18:00 to 00:00: [Fish] has a chance to be caught at half its potential.

The state is similar for Seasons, where there are the 2 strongest points (Summer/Winter) and 2 overlapping points (Spring/Autumn):



* September 23 to March 21: Generalized Winter Season
* March 21 to September 23: Generalized Summer Season
* September 23 to December 21: Autumn Season (Winter/Summer overlap)
* December 21 to March 21: True Winter Season (No Summer overlap)
* March 21 to June 21: Spring Season (Winter/Summer overlap)
* June 21 to September 23: True Summer Season (No Winter overlap)

Similar rules for time of day fish apply to seasons.

Weather-specific fish also can only be caught during specific weathers, with some weathers being more likely during certain seasons than others (ie snow only during true winter). Weather should be a predictive system that can be forecast by at least a week in advance (which is actually a thing in lore considering we have magic and its influences), and in addition shouldn’t be truly random just simply to not have multiple levels of RNG making the system feel unfun. Having to fish in one area for a whole day hoping for weather that will never occur is not something that should ever happen. Weather can of course still be random when generated a week ahead of time, but the forecast for the upcoming week should remain the same.


### **Fishing Trips**

Fishing Trips are a new “world” event where multiple players join onto a boat that visits a select set of locations upon the seas. The crew consists of a few key members, of which core to the travel is the use of teleportation mages. The ship arrives/exits the harbor as normal, but the whole boat + players are soon enclosed in a large teleportation sphere when they reach far enough from the harbor. The ship is then teleported to the new location (a semi-”instanced” open-world location, but without interference of other players and allowing for sharding population distribution). Sometimes these teleports can “encounter interference,” teleporting to faraway and wild unintended locations. Each trip begins and ends at Fizzle and Pozzik’s Speedbarge, which can be easily accessed by taking the Caverns of Time portal in Stormwind/Orgrimmar. Any level character can queue up for this activity.

Some location ideas:



* **The Shimmering Deep** (Southwest Kalimdor - Thousand Needles)
* **Bay of Azshara** (Northeast Kalimdor - Great Sea)
* **The Seething Shore** (Southwest Kalimdor - Veiled Sea)
* **Tiragarde Sound** (Kul Tiras - Great Sea)
* **Misty Reed Strand** (Southeast Eastern Kingdoms - Forbidding Sea)
* **Sun’s Reach Harbor** (Northern Quel’Thalas - North Sea)
* **Mistveil Sea** (Eastern Pandaria - South Seas)
* **The Lost Glacier** (Northrend - North Sea)
* **The Bay of Kings** (Zandalar - South Seas)
* **Isle of Spears** (Northrend - Frozen Sea)
* **The Shrouded Reach** (Southern Krasarang Wilds - South Seas)
* **Darkmoon Island** (Great Sea)
* **The In-Between** (Shadowlands - Special)
* **Netherstorm** (The Twisting Nether - Special)
* **Abyssal Maw** (Vashj'ir - Special)

Each fishing trip consists of 2 predetermined planned locations and 1 random location. Each location lasts about 10 minutes. The main goal for each group on a fishing trip will be to fill a bar (by catching as many fish / high prized fish as possible) and a weekly quest. Although it can be completed every hour as many times as a player wants, the main goal will be a weekly reward, of which most players can safely ignore if they wish. For low level players, this could be a possible alternative activity to dungeons/questing to level up. Additionally, each location provides an opportunity to level fishing skill in a particular region. Fishing skill itself is not a requirement to participate, in fact it should be encouraged as an alternate means to level fishing for past expansions. The thing that can be utilized would be things like fishing specialization talents for instance, however players shouldn’t feel like a low fishing skill exactly detracts from the rest of the group, or that a group of 20 low level fishers have no chance at completing an event. Things like skill and stats should be more relevant toward the personal loot rewards and drops.

In general, fishing trips should be rewarding enough to do, providing short and long term grind goals. Each fishing trip should also always be rewarding no matter what the results of RNG are such as providing currency to be used for a vendor, random materials for profession crafting, or even a hefty sum of gold. 


### **Reward Structure**

Collecting rare fish to work towards rewards such as mounts, pets, transmog, toys, better fishing gear crafting components. These could either be specific catches from certain conditions, or as a vendor reward using currency gained from generalized fishing + fishing trips.

**Mounts**

Several mount rewards in particular can be applied, such as the Wonderous Wavewhisker, TCG Turtle mounts, otters, other turtle mounts not yet applied in game, and other fish-related mounts. These should be considered very expensive currency rewards with additional achievement requirements.

**Pets**

Similar applies to mounts, but these should be much easier lower tiers to obtain. There are many numerous fish pets that can be listed, but it could also be a chance to add other pets that aren’t currently or are no longer available such as the time-limited trading post pets. Some specific pets could be Cap’n Crackers, Flurky, Lurky, Murkimus the Gladiator, Pebble, and Glub.

**Transmog**

A special Angler transmog. This should be a moderate-expensive reward. This is designed especially with an angler look in mind. The set would be completely cosmetic, and could even have a toy/ability to appear when fishing mode is engaged.

**Toys**

Toys should probably remain centric towards fishing in thematics. Having them be beneficial toward fishing probably wouldn’t be the best aim however, when that could instead be refashioned as talents or abilities. Some toys could be additional raft appearances, or providing alternate means to obtain certain grindy items/toys like Bipsi's Bobbing Berg. Other toys could be transformation items, such as into a tuskarr or jinyu. Unique bobbers, or alternate means to obtain the Legion bobbers. The list goes on.

**Crafting Components**

Creating a more powerful fishing pole, hat, or pair of boots should be a goal for fishing, but implementing it shouldn’t be as simple as “get it crafted by a tailor/engineer” after buying all the materials off the auction house or relying on mettle from another unrelated profession. Being able to actually obtain your own parts to fit your fishing pole without depending on a fluctuating auction economy would help with a feeling of agency. Even if you may need an engineer to successfully craft a pole, the fisherman was the one to obtain the parts and feels a sense of accomplishment and goals met. Who knows, you may even be able to craft something a little more spicy than a rare tool - something that extends into epic, or even legendary quality? Emissive glow in the dark / glitter emitter fishing rods & bobbers are neat.

Most of these rewards should be Bind on Pickup as opposed to tradeable, but there could be some exceptions. Generally tradeable things should be consumables that aren’t permanent, such as potions or food or some non-fishing crafting components.


Cover image credit: [Jason Kang, Hearthstone Card Art](https://www.artstation.com/artwork/1nAN9e)