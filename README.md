# qb-present - Like Nopixel
**Give New Player a present Box with item Like Nopixel**

# Framework Support:
**This Script only support QB-CORE Framework If You Use Other Framework You Can Convert YourSelf**

# images
![box](https://i.imgur.com/zxsDgNT.png)

# Showcase
https://streamable.com/wfx22d

# Install Tutorial:
- **1.** go to `qb-inventory/html/images` put the box image to there.
- **2. go to `qbcore/shared/main.lua ` line  73 add:     `['present'] = { amount = 1, item = 'present' },`**
-  **3.** go to your `qb-core/shared/items.lua` and add:     
-  ` ["present"] 					 = {["name"] = "present", 			  			["label"] = "present box", 				["weight"] = 10, 		["type"] = "item", 		["image"] = "pr_box.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,	["combinable"] = nil,   ["description"] = "Present box for new join player."},
`
- **4.** If You Want to config what player can get after opened the item just go to `qb-present/server/main.lua` and add more or delete the 
-      Player.Functions.AddItem('sandwich', 2) -- sandwich can be change to any item you want just add more and more if you need
-      TriggerClientEvent('inventory:client:ItemBox', src, QBCore.Shared.Items['youritemname'] , "add")
- 5. **dont forget to put that client to under**

# Next To Do:
**If anyone know how to trigger and add progressbar in client pls dm my discord: `ʏɪsʜᴇɴɢᴄʜᴇᴡ#0257` I Will Be Thankful**

# recommand :
https://github.com/tnj-development/tnj-notify  --this notification will realistic like nopixel notify
