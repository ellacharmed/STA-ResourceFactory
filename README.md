![menu location](https://ellacharmed.files.wordpress.com/2019/11/resource-factory-in-menu.png)

# STA-ResourceFactory
Creates a whole bunch of resources, using the Fish Factory mesh from the modtool sample (for now). Meant as a sandbox-enabler mod to test out game features, and counter the early access bugginess of the game.

##Design considerations
- Removed the disaster-related features in the Fish Factory sample mod.
- Churns out chunks of resources every 2 min (in-game time).
- The MODS user interface in the game has no scrollable panel to go to a second page, so we are limited to using 4 mods at a time (for now). Even if you placed more than 4 files in the Mods folder in Windows Explorer, only 4 would be visible.
- One mod to rule them all situation (for now). The 4 mods you select cannot all use the same mesh if the mod is a building-type. All the buildings will revert to just one upon the next load of the Save game. This appears to be a modtool design limitation, for the moment. Unless I missed a configuration somewhere.
- Have built-in capacity storage for for 350 units for each of the 16 resources. (v0.3)
- Free 2000 Science Points (v0.3)


Located in Build menu under Resources tab. 

##  Requirements
* 100 Science Points: need to build a General Storage first. Otherwise, produced items have no where to go and thus cannot be used.
* Construction Cost: Metal 10 units
* Repair cost: Metal 1 unit
* Demolished returns: Metal 25 units, Plastic 5 units


## Expected outcome
* Output: see list below for each recipe group
<img src="https://ellacharmed.files.wordpress.com/2019/11/resource-factory-in-action.png" width="50%" alt="resource factory in action"/>
* Select the recipe group for the products you wish to clone. 

**1. Recipe group: Medicine**
- Input: Medicine 1
- Antibiotics: 1
- Iodine: 1
- Medicine: 1

**2. Recipe group: Raw building resources**
- Input: nothing
- Concrete: 5
- Debris: 5
- Fiber: 5
- Firewood: 5
- Metal: 5
- Trash: 5


**3. Recipe group: Refined building resources**
- Input: nothing
- Component: 5
- Electronics: 5
- Parts: 5
- Plank: 5
- Plastic: 5
- Wood: 5

**4. Recipe group: End products**
- Input: Fiber 1, Metal 1
- Cloth: 5
- Tools: 5

##  Known issues/Future enhancement roadmap
- UNITY-engine-related: Mods work only when enabled on NEW games (a Unity game design limitation)
- UNITY-engine-related: Cannot load a second Save game, have to QUIT to Desktop first. One mod-enablement per one load of the game.
- TODO: Create a more appropriate mesh model
- TODO: Use a different icon based on model thumbnail
- TODO: Research Worker slots? (Might be a current modtool limitation)
- [DONE]Demolishing won't recoup construction materials (v0.2)
- [DONE]to figure out what happened to the pause button, earlier tests with an input requirement had one (v0.2)


##  Acknowledgements
- Modtool project and wiki guide with Fish Factory sample: https://sta.paradoxwikis.com/Modding:_Basics
- Tips of correcting the Description from [@Gcrazygamer](https://www.reddit.com/user/Gcrazygamer/): https://www.reddit.com/r/survivingtheaftermath/comments/dmq3kj/tip_for_modders_and_bug_for_xbox_mods/ 
