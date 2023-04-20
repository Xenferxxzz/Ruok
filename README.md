if game.CoreGui:FindFirstChild("ToggleUI") then
	game.CoreGui:FindFirstChild("ToggleUI"):Destroy()
end
local ToggleUI = Instance.new("ScreenGui")
local ToggleButton = Instance.new("TextButton")
local ToggleButtonHUI = Instance.new("UICorner")
ToggleUI.Name = "ToggleUI"
ToggleUI.Parent = game.CoreGui
ToggleUI.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

ToggleButton.Name = "ToggleButton"
ToggleButton.Parent = ToggleUI
ToggleButton.BackgroundColor3 = Color3.fromRGB(30,20,20)
ToggleButton.BackgroundTransparency = 0.1
ToggleButton.BorderSizePixel = 0
ToggleButton.Position = UDim2.new(0.120833337, 0, 0.0952890813, 0)
ToggleButton.Size = UDim2.new(0, 50, 0, 50)
ToggleButton.Font = Enum.Font.Creepster
ToggleButton.Text = "N"
ToggleButton.TextColor3 = Color3.fromRGB(102, 178, 255)
ToggleButton.TextSize = 30.000
ToggleButton.Draggable = true
ToggleButton.MouseButton1Click:Connect(function()
	game.CoreGui:FindFirstChild("Kenei").Enabled = not game.CoreGui:FindFirstChild("Kenei").Enabled
end)
