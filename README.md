![menu location](https://ellacharmed.files.wordpress.com/2019/11/resource-factory-in-menu.png)

# STA-ResourceFactory
Creates a whole bunch of resources, using the Fish Factory mesh from the modtool sample. Clones 10 units of the following resources every 5(?) game-minutes (aka 300 of Production Time): 
- Antibiotics
- Cloth
- Component
- Concrete
- Debris
- Electronics
- Fiber
- Firewood
- Iodine
- Metal
- Parts
- Plank
- Plastic
- Tools
- Trash
- Wood

Located in Build menu under Resources tab. 

##  Requirements
* Input: Plank 5 units - v0.2
* 100 Science Points: need to build a General Storage first. Otherwise, produced items have no where to go and thus cannot be used.
* Construction Cost: Metal 10 units
* Repair cost: Metal 1 unit
* Demolished returns: Metal 25 units, Plastic 5 units


## Expected outcome
* Output: 10 units of the listed resources above
<img src="https://ellacharmed.files.wordpress.com/2019/11/resource-factory-in-action.png" width="50%" alt="resource factory in action"/>

##  Known issues/Future enhancements
- [DONE]Demolishing won't recoup construction materials - v0.2
- [DONE]to figure out what happened to the pause button, earlier tests with an input requirement had one - v0.2
<img src="https://ellacharmed.files.wordpress.com/2019/11/testing-with-one-resource.png" width="25%" alt="testing with one resource"/>




##  Acknowledgements
- Modtool project and wiki guide with Fish Factory sample: https://sta.paradoxwikis.com/Modding:_Basics
- Tips of correcting the Description from [@Gcrazygamer](https://www.reddit.com/user/Gcrazygamer/): https://www.reddit.com/r/survivingtheaftermath/comments/dmq3kj/tip_for_modders_and_bug_for_xbox_mods/ 
