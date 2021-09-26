# STA-ResourceFactory

![menu location](Assets/Images/sta-resource-factory-build-menu-location.jpg "menu location")

Creates a whole bunch of resources, using the Fish Factory mesh from the modtool sample (for now). Meant as a sandbox-enabler mod to test out game features and learn game mechanics, and counter the lack of resources in game.

## How to install

- Mod Subscription is not working via [paradoxplaza.com STA's Mod page](https://mods.paradoxplaza.com/games/surviving_aftermath). Use Manual method in guide linked below. As such, you can simply download the .mod file from the [release page](https://github.com/ellacharmed/STA-ResourceFactory/releases) of this repository, as well.
- Read the guide at my [ellacharmed.wordpress.com](https://ellacharmed.wordpress.com/2019/11/04/how-to-use-mods-in-surviving-the-aftermath/) blog page.

## Design considerations

### Why does this mod exist?

Well, due to some game-design constrains and bugs in the game, resources were an issue at the beginning of Early Access release back in October 2019. And since then, the subsequent patches have addressed some, but not all bugs, and also introduced a few more. So this mod initially is to ensure that my gameplay can proceed despite these constraints and bugs from one patch cycle to the next.

And then, my "pet-peeves" were shown not to be an isolated incident. And indeed, other players are complaining of the same issues, and so I uploaded it and release it to the public and here we are.

With the introduction of the Resource Extractors in one of the updates, I had thought that this mod is made redundant and have not updated it for months as I have been playing other games. But, as of patch version **1.12.4.8223 (Jan 2021)**, there's still some inherent bugs (the lockups aka stuck-running-bug still exists), and further balancing is still required despite all the improvements and enhancements of the past year. The production versus consumption values, that have been re-tweaked in this patch, still do not allow for the growth of the colony the way that suits our individualistic playstyle.

### Game design constraints

- Due to the game design only allowing 1 function per building, built-in Storage has been removed from all factories. You need the in-game storage now.
- This design constrain also means that I could not make each factory have a secondary function of providing auto-scout map, power, water, and heat.

### Mod design

- Buildings available after "Shoot the flare" step.

- Located in Build menu under Resources tab, as shown in introduction image above. Food Factory is located under Food tab.

- The Recipes produce individual item types.

- ![pause-button](Assets/Images/pause-button.png "pause-button")Includes a Pause button to halt production as and when required. (patch 1.0)

- ![Production Limit](Assets/Images/production-limit.png "Production Limit")Added Production Limit. Use together with the Pause button so you don't overwhelmed your colony with transporting-resources-tasks when you don't have enough Carriers for other essential transporting tasks (like transporting Firewood).

- Currently made "**Automated**" like the upgraded Resource Extractors for Basic and Pharma.

- 2 Worker slots for Food and Manufacturing, these 2 buildings also require inputs. So that the stored items would be used and relieve the Storage capacity.

- Removed the disaster-related features and the Energy requirement in the Fish Factory sample mod.

- Removed the use of Input values to clone basic resources due to [issue #7](https://github.com/ellacharmed/STA-ResourceFactory/issues/7). Since resources shall not be consumed to clone more, I've reduced the output values so the Storage and Stockpile won't be overloaded.

- Since the Resource Factory is using the Fish Factory's mesh, the buildings have been differrentiated by placing a logo on the building's roof. (v0.3.6). I've also been updating the Fish Factory for every patch cycle. You can get it from the [StA-FishFactory release page](https://github.com/ellacharmed/StA-FishFactory/releases). ![fish vs resource](Assets/Images/fish-vs-resource.jpg "fish vs resource")

## Requirements

- Construction Cost: 4 Plank, 2 Plastic
- ~~Repair cost: Metal 2 units~~ Made Indestructible. Repair resources taken to building but turn red again with no repair done. Same issue with Fish Factory, so need further study.
- Demolished returns: 5 Plastic

## Expected outcome

- Output: recipe groups revamped for update 1.12.4 (Jan 2021)

[![Watch the video](Assets/Images/vid_poster_image.jpg)](https://youtu.be/SMTmhD1iRSE "Click to play recipe-groups") _Click image to play video via Youtube; video recorded while on Update 8_

## Known issues

- UNITY-engine-related: Mods work only when enabled on NEW games (a Unity game design limitation)
- UNITY-engine-related: Cannot load a second Save game in same gameplay session, have to QUIT to Desktop first. One time mod-enablement per one session load of the game.
- Mod-tool-related: input values (x) cancelling output (y) in recipes, even though x value is not equal to y value, when the using the same input & output resources. So x Concrete cannot create y Concrete. See [issue #7](https://github.com/ellacharmed/STA-ResourceFactory/issues/7)
- Non-flexible Building UI: icons can go off-screen from the Building UI's dialog box. The User Interface is not yet flexible, sizable or draggable.

![UI overflow on both sides](Assets/Images/sta-resourcefactory-buildingUI-both.jpg "UI overflow on both sides") _UI overflow on both sides_ ![UI overflow on right side](Assets/Images/sta-resourcefactory-buildingUI-right.jpg "UI overflow on right side") _UI overflow on right side_

## Acknowledgements

- The [Fish Factory sample mod](https://github.com/iceflake/survivingtheaftermath) by IceFlake Studios
- [Modtool project and paradoxwiki guide](https://sta.paradoxwikis.com/Modding:_Basics)
- Tips of correcting the Description from reddit post by [@Gcrazygamer](https://www.reddit.com/user/Gcrazygamer/): [tip_for_modders_and_bug_for_xbox_mods](https://www.reddit.com/r/survivingtheaftermath/comments/dmq3kj/tip_for_modders_and_bug_for_xbox_mods/)

## Discussion

- for bug reports or questions, please post in [[mod] Ellacharmed's Resource Factory](https://forum.paradoxplaza.com/forum/index.php?threads/mod-ellacharmeds-resource-factory.1272140/) thread on the [Paradox Surviving The Aftermath forums](https://forum.paradoxplaza.com/forum/index.php?forums/surviving-the-aftermath.1060/)

## Links

![fish-factory-mod](https://steamuserimages-a.akamaihd.net/ugc/1769329128553792572/0D6D81F8EE4B776F7CEEEE9EA86640A4FE502DFC/?imw=5000&imh=5000&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false "Fish Factory mod")

- Ella's version of the Fish Factory. Fixed some text in Localization and Events. Changed icon.
  - [download from github](https://github.com/ellacharmed/StA-FishFactory)
  - [subscribe from Steam](https://steamcommunity.com/sharedfiles/filedetails/?id=2472277310)

![Windfall-event-mod](https://steamuserimages-a.akamaihd.net/ugc/1769329097644045757/C08DB431BC041D7387946FC8C22E9AAE1A3096D0/?imw=637&imh=358&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=true "windfall event mod")

- Windfall mod

  - [download from github](https://github.com/ellacharmed/STA-Windfall)
  - [download from paradoxplaza](https://mods.paradoxplaza.com/mods/3571/Any)
  - [subscribe from Steam](https://steamcommunity.com/sharedfiles/filedetails/?id=2472277310)

- [How to install and use Mods in Surviving the Aftermath](https://ellacharmed.wordpress.com/2019/11/04/how-to-use-mods-in-surviving-the-aftermath/) guide via [ellacharmed](ellacharmed.wordpress.com)'s Wordpress blog
