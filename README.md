-- ScreenGui object
local gui = Instance.new("ScreenGui")
gui.Name = "CustomLoader"
gui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
 
-- Frame
local frame = Instance.new("Frame")
frame.Size = UDim2.new(0, 300, 0, 180)
frame.Position = UDim2.new(0.5, -150, 0.9, -280)
frame.BackgroundColor3 = Color3.new(0, 0, 0)
frame.Parent = gui
 
-- UICorner of the frame
local corner = Instance.new("UICorner")
corner.CornerRadius = UDim.new(0, 10)
corner.Parent = frame
 
-- Title 
local Title = Instance.new("TextLabel")
Title.Size = UDim2.new(0.99, 0, 0, 60)
Title.Position = UDim2.new(0.03, 0, 0.10, 0)
Title.BackgroundColor3 = Color3.new(0, 0, 0)
Title.BackgroundTransparency = 1
Title.TextColor3 = Color3.new(1, 1, 1)
Title.TextSize = 25
Title.Font = Enum.Font.SourceSansBold
Title.Text = "GHOST HUB V1 👑" -- Change to your script name
Title.Parent = frame
 
-- Loading bar frame
local loadingBarFrame = Instance.new("Frame")
loadingBarFrame.Size = UDim2.new(0, 0, 0.2, 0)
loadingBarFrame.Position = UDim2.new(0.02, 0, 0.7, 0)
loadingBarFrame.BackgroundColor3 = Color3.new(20, 0, 21)
loadingBarFrame.Parent = frame
 
-- UICorner of the loading bar frame
local corner_2 = Instance.new("UICorner")
corner_2.CornerRadius = UDim.new(0, 6)
corner_2.Parent = loadingBarFrame
 
-- Loading text
local loadingText = Instance.new("TextLabel")
loadingText.Size = UDim2.new(0.95, 0, 0, 30)
loadingText.Position = UDim2.new(0.03, 0, 0.7, 0)
loadingText.BackgroundColor3 = Color3.new(0, 0, 0)
loadingText.BackgroundTransparency = 1
loadingText.TextColor3 = Color3.new(1, 1, 1)
loadingText.TextSize = 18
loadingText.Font = Enum.Font.SourceSansBold
loadingText.Text = "Carregando.."
loadingText.Parent = frame
 
-- Function to animate the loading bar
function animateLoadingBar()
    local progress = 0
 
    while progress < 100 do
        progress = progress + 1
        updateProgress(progress)
        wait(0.05) -- Adjust the animation speed as needed
    end
 
    loadingText.Text = "Successfully Loaded"
  wait(0.5)
  gui:Destroy()
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "GHOST HUB V1", HidePremium = false, SaveConfig = false, ConfigFolder = "GHOST HUB V1"})
local Tab = Window:MakeTab({
	Name = "INFO ",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
local Section = Tab:AddSection({
	Name = "CREDITOS DO SCRIPT (Ghost/yuyuk1ng)  👑"
})
local Tab = Window:MakeTab({
	Name = "SCRIPTS HUB DE BF 💎",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
local Section = Tab:AddSection({
	Name = "AQUI TERÃO ALGUNS SCRIPTS BOM PRA FARM 🏆"
})
Tab:AddButton({
	Name = "Redz Hub 💫",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/REDzHUB/BloxFruits/main/redz9999"))()
      		print("Botão Pressionado")
  	end    
})

Tab:AddButton({
	Name = "Tsuo Hub 💫",
	Callback = function()
 loadstring(game:HttpGet("https://raw.githubusercontent.com/Tsuo7/TsuoHub/main/Tsuoscripts"))()
      		print("Botão Pressionado")
  	end    
})

Tab:AddButton({
	Name = "VECTO HUB 🏆",
	Callback = function()
loadstring(game:HttpGet("https://scriptblox.com/raw/UPDATE-20-Blox-Fruits-Vector-Hub-9090"))()
      		print("Botão Pressionado")
  	end    
})

local Tab = Window:MakeTab({
	Name = "PVP ⚔️",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
local Section = Tab:AddSection({
	Name = "ATENÇÃO! O w-azure e um bom script pra PVP (O aimbot dele Pega apenas no player mais proximo)"
})
Tab:AddButton({
	Name = "W-AZURE 👑",
	Callback = function()
getgenv().Team = "Pirates"
getgenv().FixCrash = false -- Turn it On For Hopping Server, Improve Performance But Silent Aim On Mob And Player
getgenv().FixCrash2 = false -- Turn it On For Hopping Server, Improve Performance But Will Remove Speed Changer
loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/3b2169cf53bc6104dabe8e19562e5cc2.lua"))()
      		print("button pressed")
  	end    
})

Tab:AddButton({
	Name = "HIT BOX (Bounty Hunter) [PC]",
	Callback = function()
	  loadstring(game:HttpGet("https://raw.githubusercontent.com/vkTrolls/Bounty-Hunter-Kit/main/script"))()
      		print("button pressed")
  	end    
})

local Tab = Window:MakeTab({
	Name = "ANTI LAG ❄️",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
local Section = Tab:AddSection({
	Name = "METODO FEITO POR YUYUK1NG! 👑"
})
Tab:AddButton({
	Name = "ANTI LAG ❄️",
	Callback = function()
	  _G.Settings = {
    Players = {
        ["Ignore Me"] = true, -- Ignore your Character
        ["Ignore Others"] = true-- Ignore other Characters
    },
    Meshes = {
        Destroy = false, -- Destroy Meshes
        LowDetail = true -- Low detail meshes (NOT SURE IT DOES ANYTHING)
    },
    Images = {
        Invisible = true, -- Invisible Images
        LowDetail = false, -- Low detail images (NOT SURE IT DOES ANYTHING)
        Destroy = false, -- Destroy Images
    },
    ["No Particles"] = true, -- Disables all ParticleEmitter, Trail, Smoke, Fire and Sparkles
    ["No Camera Effects"] = true, -- Disables all PostEffect's (Camera/Lighting Effects)
    ["No Explosions"] = true, -- Makes Explosion's invisible
    ["No Clothes"] = true, -- Removes Clothing from the game
    ["Low Water Graphics"] = true, -- Removes Water Quality
    ["No Shadows"] = true, -- Remove Shadows
    ["Low Rendering"] = true, -- Lower Rendering
    ["Low Quality Parts"] = true -- Lower quality parts
}
loadstring(game:HttpGet("https://raw.githubusercontent.com/CasperFlyModz/discord.gg-rips/main/FPSBooster.lua"))()
      		print("button pressed")
  	end    
})

local Tab = Window:MakeTab({
	Name = "ESTICAR TELA 🏆 ",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
local Section = Tab:AddSection({
	Name = "AQUI TERÃO OS MELHORES RESOLUÇÃO DO SCRIPT BASTA CLICAR! 👑"
})
Tab:AddButton({
	Name = "RESOLUÇÃO 55",
	Callback = function()
	  getgenv().Resolution = {
    [".gg/scripters"] = 0.55
}

local Camera = workspace.CurrentCamera
if getgenv().gg_scripters == nil then
    game:GetService("RunService").RenderStepped:Connect(
        function()
            Camera.CFrame = Camera.CFrame * CFrame.new(0, 0, 0, 1, 0, 0, 0, getgenv().Resolution[".gg/scripters"], 0, 0, 0, 1)
        end
    )
end
getgenv().gg_scripters = "Aori0001"
  	end    
})

Tab:AddButton({
	Name = "RESOLUÇÃO 65",
	Callback = function()
	  getgenv().Resolution = {
    [".gg/scripters"] = 0.55
}

local Camera = workspace.CurrentCamera
if getgenv().gg_scripters == nil then
    game:GetService("RunService").RenderStepped:Connect(
        function()
            Camera.CFrame = Camera.CFrame * CFrame.new(0, 0, 0, 1, 0, 0, 0, getgenv().Resolution[".gg/scripters"], 0, 0, 0, 1)
        end
    )
end
getgenv().gg_scripters = "Aori0001"
  	end    
})

Tab:AddButton({
	Name = "RESOLUÇÃO 73",
	Callback = function()
	  getgenv().Resolution = {
    [".gg/scripters"] = 0.73
}

local Camera = workspace.CurrentCamera
if getgenv().gg_scripters == nil then
    game:GetService("RunService").RenderStepped:Connect(
        function()
            Camera.CFrame = Camera.CFrame * CFrame.new(0, 0, 0, 1, 0, 0, 0, getgenv().Resolution[".gg/scripters"], 0, 0, 0, 1)
        end
    )
end
getgenv().gg_scripters = "Aori0001"
  	end    
})

Tab:AddButton({
	Name = "RESOLUÇÃO 82",
	Callback = function()
	  getgenv().Resolution = {
    [".gg/scripters"] = 0.82
}

local Camera = workspace.CurrentCamera
if getgenv().gg_scripters == nil then
    game:GetService("RunService").RenderStepped:Connect(
        function()
            Camera.CFrame = Camera.CFrame * CFrame.new(0, 0, 0, 1, 0, 0, 0, getgenv().Resolution[".gg/scripters"], 0, 0, 0, 1)
        end
    )
end
getgenv().gg_scripters = "Aori0001"
  	end    
})

 end
-- Function to update the loading progress
function updateProgress(progress)
    loadingBarFrame.Size = UDim2.new(progress / 105, 0, 0.2, 0)
    loadingText.Text = "Carregando... " .. progress .. "%"
end
 
-- Start the loading animation
spawn(animateLoadingBar)
