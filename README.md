# Animation-API
* This thingy is good.
* +1 714 463 5142
* +44 7031 959 982
* README?  No!  Read *YOU*!

# Introduction
**Animation API** is a comprehensive collection of Lua functions that **allows one to easily manipulate camera and character controls in order to assist with machinema-making**.  This library has been designed to facilitate programmers to control everything in a scene without having to consult other APIs.  It can be installed as a plugin from the [Rōblox catalogue](https://www.roblox.com/catalog/2723483316/redirect) or inserted as a `Script` into either the game's `Workspace` or `ServerScriptService` services.  All the public functions that this API uses are stored in ``_G.AnimationAPI``; note that the library isn't loaded immediately, so make sure to execute the following code before a script accesses the API:
```lua
while not _G.AnimationAPI do wait() end
```
It is recommended that you assign a script-local variable to the library once it has finished loading, preferably one that is distinctive from other variables in code.
```lua
local AnimAPI = _G.AnimationAPI
```

To run this module on a script executor *(i.e. JJSploit, Synapse, RC7)*, insert the following code into the Lua console:
```lua
--Loads the published plugin object.
scr=game:GetObjects('rbxassetid://2723483316')[1]

lclSrc=sc.AnimLocal.Source
	:match'%-%-{B}%-%-(.+)%-%-{F}%-%-'
	:gsub('r%equire','newReq')

--Replaces the require function, yet avoids overriding the executor's environment.
function newReq(o)local s='r=function()\n'..o.Source..'\nend'loadstring(s)local re=r()return re end
src=scr.Source:gsub('require%(','newReq('):gsub('script','scr'):gsub('NestedLocalLoadstring',lclScr)

--Encapsulates the main module into a function.
delay(7,f)
loadstring('f=function()\n'..src..'\nend')
```

More documentation is provided in [this repository's wiki](https://github.com/Windows81/Animation-API/wiki)
