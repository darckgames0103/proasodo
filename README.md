
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Shadow Hub", "BloodTheme")
local TabA = Window:NewTab("Dupes")
local SectionC = TabA:NewSection("Safety")
SectionC:NewToggle("Safe Spot", "Use this when duping.", function(state)
	if state then
		_G.ss = state
	else
		_G.ss = state
		wait(0.6)
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.SpawnLocation.CFrame + Vector3.new(0,5,0)
		game.Players.LocalPlayer.Character.HumanoidRootPart.Velocity = Vector3.new(0,0,0)
	end
end)
_G.Speed = 16
game:GetService("Workspace").Map.leaderboard.SurfaceGui.ServerVersion.Text = "kode's dupes loaded\ncheat version: 1.5\ndiscord.gg/7c9QBaC6GV"
local SectionA = TabA:NewSection("Normal Dupes")
local SectionB = TabA:NewSection("Custom")
SectionA:NewButton("Auto Dupe $100 --> $10B", "This always starts from 100$.", function()
	for i = 1,10 do 
		task.wait(0.5)
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Gem Green")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Gem Green")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Gem Green")
	end
	for i = 1,15 do
		task.wait(0.5)
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Amogus Cyan")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Amogus Cyan")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Amogus Cyan")
	end
	for i = 1,30 do
		task.wait(0.5)
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Pop It Blue!")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Pop It Blue!")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Pop It Blue!")
	end
	for i = 1,20 do
		task.wait(0.5)
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Gummy Orange")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Gummy Orange")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Gummy Orange")
	end
	for i = 1,35 do
		task.wait(0.5)
		gaame:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Rainbow Cat")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Rainbow Cat")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Rainbow Cat")
	end
	for i = 1,35 do
		task.wait(0.5)
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Sheriff Cat")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Sheriff Cat")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Sheriff Cat")
	end
	for i = 1,20 do
		task.wait(0.5)
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Tulsa rainbow")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Tulsa rainbow")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Tulsa rainbow")
	end
	for i = 1,35 do
		task.wait(0.5)
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("eTruck")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("eTruck")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("eTruck")
	end
	for i = 1,20 do
		task.wait(0.5)
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Rainbow Banana")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Rainbow Banana")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Rainbow Banana")
	end
	for i = 1,15 do
		wait(0.5)
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Lolly Rainbow")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Lolly Rainbow")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Lolly Rainbow")
	end
	for i = 1,25 do
		task.wait(0.5)
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Pop It Rainbow!")
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Pop It Rainbow!")
		game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Pop It Rainbow!")
	end
end)

SectionA:NewToggle("Dupe Banana", "You need 2T to dupe this item.", function(state)
	_G.banana = state
end)
SectionA:NewToggle("Dupe Rainbow Pop It", "You need 1.2B to dupe this item.", function(state)
	_G.rbpopit = state
end)
SectionB:NewTextBox("Custom Item Name", "Go to the shop for item names.", function(txt)
	_G.txt = txt
end)
SectionB:NewToggle("Dupe Custom Item", "No information provided.", function(state)
	_G.custom = state
end)
local TabB = Window:NewTab("Buy Items")
local SectionD = TabB:NewSection("Normal Items")
local SectionE = TabB:NewSection("Custom")
SectionD:NewTextBox("Buy Banana", "Type the amount.", function(txt)
	for i = 1,txt do
		wait(0.01)
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("The banana")
	end
end)
SectionD:NewTextBox("Buy Rainbow Pop It", "Type the amount.", function(txt)
	for i = 1,txt do
		wait(0.01)
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Pop It Rainbow!")
	end
end)
SectionD:NewTextBox("Buy Ben (NFT)", "Type the amount.", function(txt)
	for i = 1,txt do
		wait(0.01)
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Trading Ben")
	end
end)
SectionD:NewTextBox("Buy Money (NFT)", "Type the amount.", function(txt)
	for i = 1,txt do
		wait(0.01)
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Munneh")
	end
end)
SectionD:NewTextBox("Buy Mom (NFT)", "Type the amount.", function(txt)
	for i = 1,txt do
		wait(0.01)
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Mommeh Long Legs")
	end
end)
SectionD:NewTextBox("Buy Watermelon", "Type the amount.", function(txt)
	for i = 1,txt do
		wait(0.01)
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Watermelon")
	end
end)
SectionE:NewTextBox("Enter Item Name", "Type the name.", function(txt)
	_G.custombuy = txt
end)
SectionE:NewTextBox("Buy Custom item", "Type the amount.", function(txt)
	for i = 1,txt do
		wait(0.01)
		game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer(_G.custombuy)
	end
end)
local TabC = Window:NewTab("Anti Reaper")
local SectionF = TabC:NewSection("Reaper Protection")
SectionF:NewToggle("Anti Reaper (uses watermelons)", "You can buy lots of watermelons from the buy items tab.", function(state)
	_G.AR = state
end)

local TabD = Window:NewTab("Misc")
local SectionG = TabD:NewSection("Misc")
SectionG:NewButton("Trade Value", "Also known as X-RAY, allows you to check the value of a trade", function()
	game.Players.LocalPlayer.XRay.Value = true
end)
SectionG:NewButton("Night Mode", "Eye rest. (Only you see the night)", function()
	local Info = TweenInfo.new(3, Enum.EasingStyle.Exponential)
	if game:GetService("Players").LocalPlayer:GetAttribute("IsDay") then
		game:GetService("TweenService"):Create(game:GetService("Lighting"), Info, {ClockTime = 12}):Play()
		game:GetService("Players").LocalPlayer:SetAttribute("IsDay", false)
	else
		game:GetService("TweenService"):Create(game:GetService("Lighting"), Info, {ClockTime = 0}):Play()
		game:GetService("Players").LocalPlayer:SetAttribute("IsDay", true)
	end
end)
SectionG:NewButton("Anti Afk", "Removes the afk kick", function()
	local VirtualUser=game:service'VirtualUser'
	game:service('Players').LocalPlayer.Idled:connect(function()
		VirtualUser:CaptureController()
		VirtualUser:ClickButton2(Vector2.new())
	end)
end)
SectionG:NewButton("Rejoin", "Leaves and joins the same server, use this if you're lagging", function()
	local tpservice = game:GetService("TeleportService")
	local plr = game.Players.LocalPlayer
	tpservice:Teleport(game.PlaceId, plr)
end)
SectionG:NewButton("Anti Lag", "this doesnt work ", function()
	-- need to improve this later.
	for i,v in pairs(workspace:GetDescendants()) do
		if v.ClassName == "Part" or v.ClassName == "WedgePart" then
			v.Material = "SmoothPlastic"
		end
	end
end)
SectionG:NewButton("scam", "THIS scam",function ()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(68.7329941, 19.9683781, -326.633057, -0.997881889, -2.25651622e-08, 0.0650515035, -1.70088512e-08, 1, 8.59678408e-08, -0.0650515035, 8.46793e-08, -0.997881889)
	wait(0.2)
	game.Players.LocalPlayer.Character.Humanoid.Jump = true
	wait()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(53.0703354, 19.9683781, -326.738068, -0.999940038, -1.07354312e-08, 0.0109490538, -1.03423989e-08, 1, 3.59531214e-08, -0.0109490538, 3.58377257e-08, -0.999940038)
	wait(0.3)
	game.Players.LocalPlayer.Character.Humanoid.Jump = true
	wait(0.95)
	game.Players.LocalPlayer.Character.Humanoid.Jump = true	
    wait(0.95)
	game.Players.LocalPlayer.Character.Humanoid.Jump = true
    wait(0.95)
	game.Players.LocalPlayer.Character.Humanoid.Jump = true  
end)
	

local TabG = Window:NewTab("Destroy Map")
local SectionH = TabG:NewSection("REMINDER: ONLY YOU SEE THIS.")
SectionH:NewButton("Destroy Pads", "Only you see this", function()
	game:GetService("Workspace").Map.GroupReward:Destroy()
	game:GetService("Workspace").Map.CodePad:Destroy()
end)
SectionH:NewButton("Destroy Clothing", "Only you see this", function()
	game:GetService("Workspace").Map.ClothingRack:Destroy()
end)
SectionH:NewButton("Destroy Mystery Box", "Only you see this", function()
	game:GetService("Workspace").Map.WeeklyDrop:Destroy()
end)
SectionH:NewButton("Destroy Bubbles", "Only you see this", function()
	game:GetService("Workspace").Map.Decorations:Destroy()
end)
SectionH:NewButton("Destroy Group Wall", "Only you see this", function()
	game:GetService("Workspace").Map.GroupReward.Field:Destroy()
end)
SectionH:NewButton("Destroy Featured Item", "Only you see this", function()
	game:GetService("Workspace").Map.FeaturedItem:Destroy()
end)

local TabE = Window:NewTab("Character")
local SectionI = TabE:NewSection("Modification")
SectionI:NewTextBox("Speed", "Type the amount. Default is 16.", function(txt)
	_G.Speed = txt
	game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = txt
end)
SectionI:NewButton("Inf Jump", "Allows you to jump in air.", function()
	_G.infinjump = true
	local Player = game:GetService("Players").LocalPlayer
	local Mouse = Player:GetMouse()
	Mouse.KeyDown:connect(function(k)
		if _G.infinjump then
			if k:byte() == 32 then
				Humanoid = game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Humanoid")
				Humanoid:ChangeState("Jumping")
				wait(0.1)
				Humanoid:ChangeState("Seated")
			end
		end
	end)
end)

SectionI:NewButton("Fly (Press G to toggle)", "I think you know what flying is.", function()
	local players = game:GetService("Players")
	local lp = players.LocalPlayer
	local Mouses = lp:GetMouse()
	mouse = Mouses
	local workspace = game.Workspace
	function sFLY(vfly)
		FLYING = false
		speedofthefly = 1.5
		speedofthevfly = 1
		while not lp or not lp.Character or not lp.Character:FindFirstChild('HumanoidRootPart') or not lp.Character:FindFirstChild('Humanoid') or not mouse do
			wait()
		end 
		local T = lp.Character.HumanoidRootPart
		local CONTROL = {F = 0, B = 0, L = 0, R = 0, Q = 0, E = 0}
		local lCONTROL = {F = 0, B = 0, L = 0, R = 0, Q = 0, E = 0}
		local SPEED = 0
		local function FLY()
			FLYING = true
			local BG = Instance.new('BodyGyro', T)
			local BV = Instance.new('BodyVelocity', T)
			BG.P = 9e4
			BG.maxTorque = Vector3.new(9e9, 9e9, 9e9)
			BG.cframe = T.CFrame
			BV.velocity = Vector3.new(0, 0, 0)
			BV.maxForce = Vector3.new(9e9, 9e9, 9e9)
			spawn(function()
				while FLYING do
					if not vfly then
						lp.Character:FindFirstChild("Humanoid").PlatformStand = true
					end
					if CONTROL.L + CONTROL.R ~= 0 or CONTROL.F + CONTROL.B ~= 0 or CONTROL.Q + CONTROL.E ~= 0 then
						SPEED = 50
					elseif not (CONTROL.L + CONTROL.R ~= 0 or CONTROL.F + CONTROL.B ~= 0 or CONTROL.Q + CONTROL.E ~= 0) and SPEED ~= 0 then
						SPEED = 0
					end
					if (CONTROL.L + CONTROL.R) ~= 0 or (CONTROL.F + CONTROL.B) ~= 0 or (CONTROL.Q + CONTROL.E) ~= 0 then
						BV.velocity = ((workspace.CurrentCamera.CoordinateFrame.lookVector * (CONTROL.F + CONTROL.B)) + ((workspace.CurrentCamera.CoordinateFrame * CFrame.new(CONTROL.L + CONTROL.R, (CONTROL.F + CONTROL.B + CONTROL.Q + CONTROL.E) * 0.2, 0).p) - workspace.CurrentCamera.CoordinateFrame.p)) * SPEED
						lCONTROL = {F = CONTROL.F, B = CONTROL.B, L = CONTROL.L, R = CONTROL.R}
					elseif (CONTROL.L + CONTROL.R) == 0 and (CONTROL.F + CONTROL.B) == 0 and (CONTROL.Q + CONTROL.E) == 0 and SPEED ~= 0 then
						BV.velocity = ((workspace.CurrentCamera.CoordinateFrame.lookVector * (lCONTROL.F + lCONTROL.B)) + ((workspace.CurrentCamera.CoordinateFrame * CFrame.new(lCONTROL.L + lCONTROL.R, (lCONTROL.F + lCONTROL.B + CONTROL.Q + CONTROL.E) * 0.2, 0).p) - workspace.CurrentCamera.CoordinateFrame.p)) * SPEED
					else
						BV.velocity = Vector3.new(0, 0, 0)
					end
					BG.cframe = workspace.CurrentCamera.CoordinateFrame
					wait()
				end
				CONTROL = {F = 0, B = 0, L = 0, R = 0, Q = 0, E = 0}
				lCONTROL = {F = 0, B = 0, L = 0, R = 0, Q = 0, E = 0}
				SPEED = 0
				BG:destroy()
				BV:destroy()
				lp.Character.Humanoid.PlatformStand = false
			end)
		end
		mouse.KeyDown:connect(function(KEY)
			if KEY:lower() == 'w' then
				if vfly then
					CONTROL.F = speedofthevfly
				else
					CONTROL.F = speedofthefly
				end
			elseif KEY:lower() == 's' then
				if vfly then
					CONTROL.B = - speedofthevfly
				else
					CONTROL.B = - speedofthefly
				end
			elseif KEY:lower() == 'a' then
				if vfly then
					CONTROL.L = - speedofthevfly
				else
					CONTROL.L = - speedofthefly
				end
			elseif KEY:lower() == 'd' then
				if vfly then
					CONTROL.R = speedofthevfly
				else
					CONTROL.R = speedofthefly
				end
			elseif KEY:lower() == 'y' then
				if vfly then
					CONTROL.Q = speedofthevfly*2
				else
					CONTROL.Q = speedofthefly*2
				end
			elseif KEY:lower() == 't' then
				if vfly then
					CONTROL.E = -speedofthevfly*2
				else
					CONTROL.E = -speedofthefly*2
				end
			end
		end)
		mouse.KeyUp:connect(function(KEY)
			if KEY:lower() == 'w' then
				CONTROL.F = 0
			elseif KEY:lower() == 's' then
				CONTROL.B = 0
			elseif KEY:lower() == 'a' then
				CONTROL.L = 0
			elseif KEY:lower() == 'd' then
				CONTROL.R = 0
			elseif KEY:lower() == 'y' then
				CONTROL.Q = 0
			elseif KEY:lower() == 't' then
				CONTROL.E = 0
			end
		end)
		FLY()
	end

	mouse.KeyDown:connect(function(KEY)
		if KEY:lower() == 'g' then
			if FLYING == false then
				sFLY()
			else
				FLYING = false
				lp.Character.Humanoid.PlatformStand = false
			end
		end
	end)
end)

local TabG = Window:NewTab("Auto Drop")
local SectionJ = TabG:NewSection("Normal Items")
SectionJ:NewButton("Drop Banana (x15)", "Drops the banana 15 times.", function()
	for i = 1,15 do
		game:GetService("ReplicatedStorage").RemoteEvents.Equip:FireServer("The banana")
		wait(0.35)
		game:GetService("ReplicatedStorage").RemoteEvents.Drop:FireServer("The banana")
		wait(0.35)
	end
end)
SectionJ:NewButton("Drop Rainbow Pop It (x15)", "Drops Rainbow Pop It 15 times.", function()
	for i = 1,15 do
		game:GetService("ReplicatedStorage").RemoteEvents.Equip:FireServer("Pop It Rainbow!")
		wait(0.35)
		game:GetService("ReplicatedStorage").RemoteEvents.Drop:FireServer("Pop It Rainbow!")
		wait(0.35)
	end
end)
SectionJ:NewButton("Drop Ben(x15)", "Drops Ben 15 times.", function()
	for i = 1,15 do
		game:GetService("ReplicatedStorage").RemoteEvents.Equip:FireServer("Trading Ben")
		wait(0.35)
		game:GetService("ReplicatedStorage").RemoteEvents.Drop:FireServer("Trading Ben")
		wait(0.35)
	end
end)
SectionJ:NewButton("Drop Munneh (x15)", "Drops Munneh 15 times.", function()
	for i = 1,15 do
		game:GetService("ReplicatedStorage").RemoteEvents.Equip:FireServer("Munneh")
		wait(0.35)
		game:GetService("ReplicatedStorage").RemoteEvents.Drop:FireServer("Munneh")
		wait(0.35)
	end
end)
Section:NewKeybind("Aperta b nessa mizera", "KeybindInfo", Enum.KeyCode.F, function()
	Library:ToggleUI()
end)
SectionJ:NewButton("Drop Mom (x15)", "Drops Mom 15 times.", function()
	for i = 1,15 do
		game:GetService("ReplicatedStorage").RemoteEvents.Equip:FireServer("Mommeh Long Legs")
		wait(0.35)
		game:GetService("ReplicatedStorage").RemoteEvents.Drop:FireServer("Mommeh Long Legs")
		wait(0.35)
	end
end)
local SectionK = TabG:NewSection("Custom Items")
SectionK:NewTextBox("Item Name", "This will drop 15 of the custom item", function(txt)
	_G.dropcustom = txt
	for i = 1,15 do
		game:GetService("ReplicatedStorage").RemoteEvents.Equip:FireServer(_G.dropcustom)
		wait(0.35)
		game:GetService("ReplicatedStorage").RemoteEvents.Drop:FireServer(_G.dropcustom)
		wait(0.35)
	end
end)
coroutine.wrap(function()
	while wait(0.1) do
		if _G.ss then
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(math.random(20000,100000),math.random(20000,100000),math.random(20000,100000))
		end
	end
end)()
coroutine.wrap(function()
	while wait(0.5) do
		if _G.banana then
			game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("The banana")
			game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("The banana")
			game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("The banana")
		end
	end
end)()

coroutine.wrap(function()
	while wait(0.5) do
		if _G.rbpopit then
			game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Pop It Rainbow!")
			game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer("Pop It Rainbow!")
			game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer("Pop It Rainbow!")
		end
	end
end)()

coroutine.wrap(function()
	while wait(0.5) do
		if _G.custom then
			game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer(_G.txt)
			game:GetService("ReplicatedStorage").RemoteEvents.BuyItemCash:FireServer(_G.txt)
			game:GetService("ReplicatedStorage").RemoteEvents.Sell:FireServer(_G.txt)
		end
	end
end)()

coroutine.wrap(function()
	while wait(0.01) do
		if _G.AR then
			game:GetService("ReplicatedStorage").RemoteEvents.Equip:FireServer("Watermelon")
		end
	end
end)()

coroutine.wrap(function()
	while wait(0.01) do
		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = _G.Speed
	end
end)()
