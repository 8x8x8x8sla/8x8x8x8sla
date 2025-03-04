

```lua
getgenv().PobritosBR_Yield = {}

local function cmd(command)
    -- Aqui você pode adicionar o que cada comando fará
    if command == "ping" then
        print("PobritosBR Yield: Pong!")
    elseif command == "fly" then
        -- Lógica para voar
    else
        print("Comando não reconhecido.")
    end
end

local function inputHandler()
    while true do
        local input = io.read() -- obtem entrada do usuário
        cmd(input) -- chama a função de comando
    end
end

print("Bem-vindo ao PobritosBR Yield!")
print("Digite um comando:")

inputHandler()
