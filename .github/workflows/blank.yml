-- Создаем интерфейс
local ScreenGui = Instance.new("ScreenGui")
local Button = Instance.new("TextButton")

ScreenGui.Parent = game.CoreGui
ScreenGui.Name = "TestNotifierGui"

Button.Parent = ScreenGui
Button.Position = UDim2.new(0.4, 0, 0.4, 0)
Button.Size = UDim2.new(0, 200, 0, 50)
Button.Text = "Проверка уведомления"
Button.BackgroundColor3 = Color3.fromRGB(50, 150, 255)
Button.TextColor3 = Color3.fromRGB(255, 255, 255)
Button.Font = Enum.Font.SourceSansBold
Button.TextSize = 20
Button.BorderSizePixel = 0
Button.Active = true
Button.Draggable = true

-- Функция при нажатии
Button.MouseButton1Click:Connect(function()
    game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(
        "Это тестовое сообщение из GUI", "All"
    )
end)
