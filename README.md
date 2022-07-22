getgenv().TextColor = Color3.fromRGB(0,201,255)
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/GreenDeno/Venyx-UI-Library/main/source.lua"))()
local venyx = library.new("REBIRTH HUB | Ninja Legends", 5013109572)
--a
-- themes
local themes = {
Background = Color3.fromRGB(24, 24, 24),
Glow = Color3.fromRGB(0, 0, 0),
Accent = Color3.fromRGB(10, 10, 10),
LightContrast = Color3.fromRGB(20, 20, 20),
DarkContrast = Color3.fromRGB(14, 14, 14), 
TextColor = Color3.fromRGB(0,201,255),
}   
-- first page
local page = venyx:addPage("Main", 5012544693)
local section1 = page:addSection("Farming")
section1:addToggle("AutoFarm", nil, function(v)
_G.AutoFarm = v
while _G.AutoFarm do wait()
game:GetService("Players").LocalPlayer.ninjaEvent:FireServer("swingKatana")
wait(.1)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(84.60150909423828, 91254.140625, 143.71116638183594)
wait(.1)
       pcall(function()
for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
    if v:IsA ("Tool") then
         game.Players.LocalPlayer.Character.Humanoid:EquipTool(game:GetService("Players").LocalPlayer.Backpack:FindFirstChild(v.Name))
          end
       end
   end)
    end
end)

section1:addToggle("Auto Buy Sword", nil, function(xdd)
_G.BuyAllSword = xdd
while _G.BuyAllSword do wait()
game:GetService("Players").LocalPlayer.ninjaEvent:FireServer("buyAllSwords","Blazing Vortex Island")
    end
end)

section1:addToggle("Auto Buy Belts", nil, function(lol)
_G.BuyAllBelts = lol
while _G.BuyAllBelts do wait()
game:GetService("Players").LocalPlayer.ninjaEvent:FireServer("buyAllBelts","Blazing Vortex Island")
    end
end)

section1:addToggle("Auto Collect Coin,Yin", nil, function(omg)
_G.AutoCollect = omg
while _G.AutoCollect do wait(0.5)
for i,v in pairs(game:GetService("Workspace").spawnedCoins.Valley:GetChildren()) do
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
       end
    end
end)

section1:addToggle("Auto Buy Skill", nil, function(bakaa)
_G.ByAllSkill = bakaa
while _G.ByAllSkill do wait()
       game:GetService("Players").LocalPlayer.ninjaEvent:FireServer("buyAllSkills","Blazing Vortex Island")
    end
end)

section1:addToggle("Auto Buy Rank", nil, function(ahhh)
_G.BuyAllRank = ahhh
while _G.BuyAllRank do wait()
game:GetService("Players").LocalPlayer.ninjaEvent:FireServer("buyAllRanks","Blazing Vortex Island")
    end
end)



section1:addButton("Redeem All Code", function(a)
    local code = {"epictrain15","roboninja15","christmasninja500"}
for i,v in pairs(code) do
game:GetService("ReplicatedStorage").rEvents.codeRemote:InvokeServer(v)
   end
end)
-- page 2 teleport
local page2 = venyx:addPage("Teleport", 5012544693)
local section2 = page2:addSection("Teleport Island")
section2:addButton("Unlock All Island", function(bruh)
    for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Enchanted Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Astral Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Mystical Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Space Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
--XD
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Tundra Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Eternal Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Sandstorm" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Thunderstorm" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Acient Inferno Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Midnight Shadow Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Mythical Souls Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Winter Wonder Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Golden Master Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Dragon Legend Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Cybernetic Legends Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Skystorm Ultraus Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Chaos Legends Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Soul Fusion Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Dark Elements Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Inner Peace Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
    end
end
wait(.1)
for i,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
    if v.Name == "Blazing Vortex Island" then
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
       end
    end
end)
-- page 3 setting --
local page3 = venyx:addPage("Setting", 5012544693)
local section3 = page3:addSection("Setting")


section3:addKeybind("Toggle UI", Enum.KeyCode.RightControl, function()
print("Activated Keybind")
venyx:toggle()
end, function()
print("Changed Keybind")
end)

section3:addToggle("Anti AFK", nil, function(afk)
_G.AFK = afk
while _G.AFK do wait(20)
       game:GetService'VirtualUser':CaptureController()
   game:GetService'VirtualUser':Button1Down(Vector2.new(569, 371))
    end
end)


-- four page
local theme = venyx:addPage("Theme", 5012544693)
local colors = theme:addSection("Colors")

for theme, color in pairs(themes) do -- all in one theme changer, i know, im cool
colors:addColorPicker(theme, color, function(color3)
venyx:setTheme(theme, color3)
end)
end

-- load
venyx:SelectPage(venyx.pages[1], true)
