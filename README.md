# Introduction
**AnimationAPI** is a comprehensive collection of Lua functions that, using the [Rōblox platform](http://roblox.com), **allows one to easily manipulate camera and character controls in order to assist with machinema-making**.  This library has been designed to facilitate programmers to control everything in a scene without having to consult other APIs.  It can be installed as a plugin from the [Rōblox catalogue](https://www.roblox.com/catalog/2723483316/redirect) or inserted as a `Script` into either the game's `Workspace` or `ServerScriptService` services.  All the public functions that this API uses are stored in ``_G.AnimationAPI``; note that the library isn't loaded immediately, so make sure to execute the following code before a script accesses the API:
```lua
while not _G.AnimationAPI do wait() end
```
It is recommended that you assign a script-local variable to the library once it has finished loading, preferably one that is distinctive from other variables in code.
```lua
local AnimAPI = _G.AnimationAPI
```

More documentation is provided in [this repository's wiki](https://github.com/Windows81/Animation-API/wiki)

## AnimationAPI's Jokes
* This thingy is good.
* +1 714 463 5142
* +44 7031 959 982
* README?  No!  Read *YOU*!
