-carregar biblioteca 
```lua
-- Script: pobritosbr Hub

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local Audio = Instance.new("Sound")
local JumpScareButton = Instance.new("TextButton")
local KillPlayerButton = Instance.new("TextButton")
local ServerLagButton = Instance.new("TextButton")

-- Configurações do GUI
ScreenGui.Parent = game.CoreGui
Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.new(1, 1, 1)
Frame.Size = UDim2.new(0, 300, 0, 400)
title="pobritosbr Hub"fluent Script 
-- Botão para Jumpscare
JumpScareButton.Parent = Frame
JumpScareButton.Size = UDim2.new(0, 280, 0, 50)
JumpScareButton.Position = UDim2.new(0, 10, 0, 10)
JumpScareButton.Text = "Executar Jumpscare"
JumpScareButton.MouseButton1Click:Connect(function()
    -- Exibe jumpscare para todos os jogadores
    for _, player in pairs(game.Players:GetPlayers()) do
        local screen = Instance.new("ScreenGui", player.PlayerGui)
        local jumpscare = Instance.new("ImageLabel")

        jumpscare.Parent = screen
        jumpscare.Size = UDim2.new(1, 0, 1, 0)
        jumpscare.Image = "rbxassetid://jumpscare cachorro demônio "
        wait(2) -- espera 2 segundos
        jumpscare:Destroy()
    end
end)

-- Botão para matar jogador
KillPlayerButton.Parent = Frame
KillPlayerButton.Size = UDim2.new(0, 280, 0, 50)
KillPlayerButton.Position = UDim2.new(0, 10, 0, 70)
KillPlayerButton.Text = "Matar Jogador"
KillPlayerButton.MouseButton1Click:Connect(function()
    local player = game.Players.LocalPlayer
    player.Character:BreakJoints() -- Mata o jogador
end)

-- Botão para Lag Server (Simulação)
ServerLagButton.Parent = Frame
ServerLagButton.Size = UDim2.new(0, 280, 0, 50)
ServerLagButton.Position = UDim2.new(0, 10, 0, 130)
ServerLagButton.Text = "Lag Server"
ServerLagButton.MouseButton1Click:Connect(function()
    while wait(1) do
        -- Simula lag
        local part = Instance.new("Part", workspace)
        part.Size = Vector3.new(100, 1, 100)
        part.Anchored = true
        part.Position = Vector3.new(math.random(-100, 100), 50, math.random(-100, 100))
    end
end)

-- Adicionando som (substitua com seu ID de áudio)
Audio.Parent = Frame
Audio.SoundId = "rbxassetid://973965852"
Audio:Play()

print("PobritosBR Hub carregado com sucesso!"
 
 local window=fluent creat window((
 
 local tabs=( 
 main=window.addtab((title='main')),
 credits"pobritosbr"
 
