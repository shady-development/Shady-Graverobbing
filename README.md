# Shady-Graverobbing
rob graves and sell the items 
# Shady-Graverobbing
*Do you have a shovel? Are you down bad? Need some quick loot to repo it back to a pawn shop? Well fear no more. You can now do exactly that!*

## Dependencies
- qb-core
- PolyZone

## Optional Dependencies
- ps-dispatch

## How to Install
- Add the following item to your `qb-core/shared/items.lua`
```lua
	    ['shovel'] 				 		 = {['name'] = 'shovel', 			    	['label'] = 'Shovel', 					['weight'] = 15000,   ['type'] = 'item', 		['image'] = 'shovel.png', 				['unique'] = false, 	['useable'] = false, 	['shouldClose'] = false,    ['combinable'] = nil,   ['description'] = ''},
        ["grub"] 						 = {["name"] = "grub",  					["label"] = "Grub",  					["weight"] = 100, 	  ["type"] = "item",  		["image"] = "grub.png",  				["unique"] = false,     ["useable"] = false,    ["shouldClose"] = false,  	['combinable'] = nil,	["description"] = "", },
        ['humanarm'] 				 	 = {['name'] = 'humanarm', 			    	['label'] = 'HumanArm', 				['weight'] = 100, 	  ['type'] = 'item', 		['image'] = 'humanarm.png', 			['unique'] = false, 	['useable'] = false, 	['shouldClose'] = false,    ['combinable'] = nil,   ["description"] = "", },
        ["humanbody"] 					 = {["name"] = "humanbody",  				["label"] = "HumanBody",  				["weight"] = 100, 	  ["type"] = "item",  		["image"] = "humanbody.png",  			["unique"] = false,     ["useable"] = false,    ["shouldClose"] = false,  	['combinable'] = nil,	["description"] = "", },
        ['humanbones'] 				 	 = {['name'] = 'humanbones', 			    ['label'] = 'HumanBones', 				['weight'] = 100, 	  ['type'] = 'item', 		['image'] = 'humanbones.png', 			['unique'] = false, 	['useable'] = false, 	['shouldClose'] = false,    ['combinable'] = nil,   ['description'] = ''},
        ["humanbrain"] 					 = {["name"] = "humanbrain",  				["label"] = "HumanBrain",  				["weight"] = 100, 	  ["type"] = "item",  		["image"] = "humanbrain.png",  			["unique"] = false,     ["useable"] = false,    ["shouldClose"] = false,  	['combinable'] = nil,	["description"] = "" , },
        ['humaneye'] 				 	 = {['name'] = 'humaneye', 			    	['label'] = 'HumanEye', 				['weight'] = 100, 	  ['type'] = 'item', 		['image'] = 'humaneye.png', 			['unique'] = false, 	['useable'] = false, 	['shouldClose'] = false,    ['combinable'] = nil,   ['description'] = ''},
        ["humanhead"] 					 = {["name"] = "humanhead",  				["label"] = "HumanHead",  				["weight"] = 100, 	  ["type"] = "item",  		["image"] = "humanhead.png",  			["unique"] = false,     ["useable"] = false,    ["shouldClose"] = false,  	['combinable'] = nil,	["description"] = "", },
        ['humanheart'] 				 	 = {['name'] = 'humanheart', 			    ['label'] = 'HumanHeart', 				['weight'] = 100, 	  ['type'] = 'item', 		['image'] = 'humanheart.png', 			['unique'] = false, 	['useable'] = false, 	['shouldClose'] = false,    ['combinable'] = nil,   ['description'] = ''},
        ["humanintestines"] 			 = {["name"] = "humanintestines",  			["label"] = "HumanIntestines",  		["weight"] = 100, 	  ["type"] = "item",  		["image"] = "humanintestines.png",  	["unique"] = false,     ["useable"] = false,    ["shouldClose"] = false,  	['combinable'] = nil,	["description"] = "", },
        ['humankidney'] 				 = {['name'] = 'humankidney', 			    ['label'] = 'HumanKidney', 				['weight'] = 100, 	  ['type'] = 'item', 		['image'] = 'humankidney.png', 			['unique'] = false, 	['useable'] = false, 	['shouldClose'] = false,    ['combinable'] = nil,   ["description"] = "", },
        ["humanleg"] 					 = {["name"] = "humanleg",  				["label"] = "HumanLeg",  				["weight"] = 100, 	  ["type"] = "item",  		["image"] = "humanleg.png",  			["unique"] = false,     ["useable"] = false,    ["shouldClose"] = false,  	['combinable'] = nil,	["description"] = "", },
        ['humanliver'] 				 	 = {['name'] = 'humanliver', 			    ['label'] = 'HumanLiver', 				['weight'] = 100, 	  ['type'] = 'item', 		['image'] = 'humanliver.png', 			['unique'] = false, 	['useable'] = false, 	['shouldClose'] = false,    ['combinable'] = nil,   ['description'] = ''},
        ["humanlungs"] 					 = {["name"] = "humanlungs",  				["label"] = "humanLungs",  				["weight"] = 100, 	  ["type"] = "item",  		["image"] = "humanlungs.png",  			["unique"] = false,     ["useable"] = false,    ["shouldClose"] = false,  	['combinable'] = nil,	["description"] = "", },
        ['humanpancreas'] 				 = {['name'] = 'humanpancreas', 			['label'] = 'HumanPancreas', 			['weight'] = 100, 	  ['type'] = 'item', 		['image'] = 'humanpancreas.png', 		['unique'] = false, 	['useable'] = false, 	['shouldClose'] = false,    ['combinable'] = nil,   ['description'] = ''},
        ["humanskull"] 					 = {["name"] = "humanskull",  				["label"] = "HumanSkull",  				["weight"] = 100, 	  ["type"] = "item",  		["image"] = "humanskull.png",  			["unique"] = false,     ["useable"] = false,    ["shouldClose"] = false,  	['combinable'] = nil,	["description"] = "", },
        ['humantorso'] 				 	 = {['name'] = 'humantorso', 			    ['label'] = 'HumanTorso', 				['weight'] = 100, 	  ['type'] = 'item', 		['image'] = 'humantorso.png', 			['unique'] = false, 	['useable'] = false, 	['shouldClose'] = false,    ['combinable'] = nil,   ['description'] = ''},
       










```
- Add the image from `Images` to your `inventory/html/images`
- Add the following snipets to `ps-dispatch`
```lua
-- cl_events.lua
local function GraveRobbery()
    local currentPos = GetEntityCoords(PlayerPedId())
    local locationInfo = getStreetandZone(currentPos)
    local gender = GetPedGender()
    TriggerServerEvent("dispatch:server:notify",{
        dispatchcodename = "GraveRobbery", -- has to match the codes in sv_dispatchcodes.lua so that it generates the right blip
        dispatchCode = "10-86",
        firstStreet = locationInfo,
        gender = gender,
        model = nil,
        plate = nil,
        priority = 2, -- priority
        firstColor = nil,
        automaticGunfire = false,
        origin = {
            x = currentPos.x,
            y = currentPos.y,
            z = currentPos.z
        },
        dispatchMessage = 'Exhumare', -- message
        job = {"police", "bcso", "doc"} -- jobs that will get the alerts
    })
end exports('GraveRobbery', GraveRobbery)

-- sv_dispatchcodes.lua
["GraveRobbery"] = { displayCode = '10-86', description = "Attempted Robbery", radius = 0, recipientList = {'police', 'bcso', 'doc'}, blipSprite = 630, blipColour = 12, blipScale = 1.5, blipLength = 2, sound = "robberysound", offset = "false", blipflash = "false" },
```

## Issues
|  Question |  Answer |
|----       |----     |
|           |         |

## Roadmap
|  Subject |  Completed? |
|----      |----         |
| Add more graves to the `Config.lua` | ❌
