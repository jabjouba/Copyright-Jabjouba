
-- JABJOUBA Timer V2.7
-- Place in StarterPlayer > StarterPlayerScripts

local Players = game:GetService("Players")
local player = Players.LocalPlayer

local screenGui = Instance.new("ScreenGui")
screenGui.Name = "JABJOUBA_Timer"
screenGui.ResetOnSpawn = false
screenGui.IgnoreGuiInset = true
screenGui.Parent = player:WaitForChild("PlayerGui")

-- Copyright Bar
local copyrightBar = Instance.new("TextLabel")
copyrightBar.Name = "CopyrightBar"
copyrightBar.AnchorPoint = Vector2.new(0.5, 0)
copyrightBar.Position = UDim2.new(0.5, 0, 0, 80)
copyrightBar.Size = UDim2.new(0, 600, 0, 27)
copyrightBar.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
copyrightBar.BorderSizePixel = 0
copyrightBar.Text = "Copyright JABJOUBA © 2026 | Devloped By Jabjouba"
copyrightBar.TextColor3 = Color3.fromRGB(255, 255, 255)
copyrightBar.TextSize = 14
copyrightBar.Font = Enum.Font.GothamBold
copyrightBar.TextXAlignment = Enum.TextXAlignment.Center
copyrightBar.TextYAlignment = Enum.TextYAlignment.Center
copyrightBar.Parent = screenGui

-- Main Timer Bar
local bar = Instance.new("Frame")
bar.Name = "MainBar"
bar.AnchorPoint = Vector2.new(0.5, 0)
bar.Position = UDim2.new(0.5, 0, 0, 117)
bar.Size = UDim2.new(0, 330, 0, 34)
bar.BackgroundColor3 = Color3.fromRGB(15, 18, 17)
bar.BackgroundTransparency = 0.28
bar.BorderSizePixel = 0
bar.Parent = screenGui

-- Outline
local stroke = Instance.new("UIStroke")
stroke.Color = Color3.fromRGB(110, 110, 110)
stroke.Thickness = 1
stroke.Parent = bar

-- Centered Text
local mainText = Instance.new("TextLabel")
mainText.Name = "MainText"
mainText.BackgroundTransparency = 1
mainText.Position = UDim2.new(0, 5, 0, 0)
mainText.Size = UDim2.new(1, -10, 1, 0)
mainText.Font = Enum.Font.GothamBold
mainText.TextSize = 15
mainText.RichText = true
mainText.TextXAlignment = Enum.TextXAlignment.Center
mainText.TextYAlignment = Enum.TextYAlignment.Center
mainText.TextColor3 = Color3.fromRGB(255, 255, 255)
mainText.TextWrapped = false
mainText.Parent = bar

-- Format countdown
local function formatTime(seconds)
    local minutes = math.floor(seconds / 60)
    local remainingSeconds = seconds % 60
    return string.format("%02d:%02d", minutes, remainingSeconds)
end

-- Countdown repeats every 60 seconds
while true do
    for seconds = 59, 0, -1 do
        mainText.Text =
            '<font color="rgb(0,75,255)">JABJOUBA</font>' ..
            '<font color="rgb(255,255,255)">-V2.7 </font>' ..
            '<font color="rgb(0,75,255)">|</font>' ..
            '<font color="rgb(255,255,255)"> Timer: ' ..
            formatTime(seconds) .. '</font>'

        task.wait(1)
    end
end
