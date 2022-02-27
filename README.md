local Config = {

    WindowName = "BEAMMODZ HUB -- [ King Legacy ]",

            Color = Color3.fromRGB(0,183,255),

                        Keybind = Enum.KeyCode.RightControl

                                    }

                                    local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/AlexR32/Roblox/main/BracketV3.lua"))()

                                    local Window = Library:CreateWindow(Config, game:GetService("CoreGui"))

local Tab1 = Window:CreateTab("Credit")

local Section1 = Tab1:CreateSection("Credit")

local Label1 = Section1:CreateLabel("Credit : BEAMMODZ")

local Label1 = Section1:CreateLabel("Discord : https://discord.gg/ZBx9X6Zw")

local Button1 = Section1:CreateButton("Copy Discord", function()

setclipboard("https://discord.gg/ZBx9X6Zw")

end)

local Button1 = Section1:CreateButton("Copy Youtube", function()

setclipboard("https://youtube.com/channel/UCdfRF1PJDgm8k6SfVgwZOdw")

end)

local Tab1 = Window:CreateTab("Menu")

local Tab7 = Window:CreateTab("Stats")

local Tab3 = Window:CreateTab("Teleport")

local Tab4 = Window:CreateTab("Players")

local Tab6 = Window:CreateTab("Esp")

local Tab5 = Window:CreateTab("Misc")

local Tab2 = Window:CreateTab("UI Settings")

local Section1 = Tab1:CreateSection("First Section")

local Section2 = Tab1:CreateSection("Second Section")

local Section3 = Tab2:CreateSection("Menu")

local Section4 = Tab2:CreateSection("Background")

local Section5 = Tab3:CreateSection("Island")

local Section6 = Tab3:CreateSection("Npc Teleport")

local Section7 = Tab4:CreateSection("Players")

local Section8 = Tab5:CreateSection("First Misc")

local Section9 = Tab5:CreateSection("Second Misc")

local Section10 = Tab6:CreateSection("Esp")

local Section11 = Tab7:CreateSection("Stats")

local Label1 = Section1:CreateLabel("Auto Farm")

Label1:UpdateText("Auto Farm")

    -------------

local Toggle1 = Section1:CreateToggle("Auto Farm", nil, function(State)

    print(State)

    end)

    -------------

local Label2 = Section1:CreateLabel("Auto Equip")

Label2:UpdateText("Auto Equip")

    -------------

Section2:CreateLabel("Auto Item")

-------------

local Weaponlist = {}

local Weapon = nil

for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do

    table.insert(Weaponlist,v.Name)

        end

        local Dropdown1 = Section1:CreateDropdown("Select Weapon", Weaponlist, function(currentOption)

            Weapon = currentOption

                end)

                local Toggle = Section1:CreateToggle("Auto Equip", " ", function(a)

                AutoEquiped = a

                end)

spawn(function()

while wait() do

if AutoEquiped then

pcall(function()

game.Players.LocalPlayer.Character.Humanoid:EquipTool(game:GetService("Players").LocalPlayer.Backpack:FindFirstChild(Weapon))

end)

end

end

end)

    -------------

    local Toggle1 = Section2:CreateToggle("Auto Sea King (Beta)", nil, function(State)

        print(State)

        end)

        -------------

    local Toggle2 = Section2:CreateToggle("Auto Bisento", nil, function(State)

        print(State)

        end)

        -------------

local Toggle3 = Section2:CreateToggle("Auto Saber", nil, function(State)

    print(State)

    end)

    -------------

local Toggle4 = Section2:CreateToggle("Auto Anubis Axe", nil, function(State)

    print(State)

    end)

    -------------

local Toggle5 = Section2:CreateToggle("Auto Enma", nil, function(State)

    print(State)

    end)

    -------------

local Toggle6 = Section2:CreateToggle("Auto Kaido", nil, function(State)

    print(State)

    end)

    -------------

local Toggle7 = Section2:CreateToggle("Auto BigMom", nil, function(State)

    print(State)

    end)

        -------------

    local Toggle1 = Section11:CreateToggle("Defense Stats", nil, function(State)

        print(State)

        end)

        -------------

    local Toggle2 = Section11:CreateToggle("Melee Stats", nil, function(State)

        print(State)

        end)

        -------------

    local Toggle3 = Section11:CreateToggle("Sword Stats", nil, function(State)

        print(State)

        end)

        -------------

    local Toggle4 = Section11:CreateToggle("Power Fruit Stats", nil, function(State)

        print(State)

        end)

        -------------

local Label1 = Section7:CreateLabel("Players")

Label1:UpdateText("Players")

-------------

    local Label1 = Section10:CreateLabel("Esp")

    Label1:UpdateText("Esp")

    -------------

local Toggle1 = Section10:CreateToggle("Esp Players", nil, function(State)

    while wait() do

         pcall(function()

                for i,v in pairs(game.Players:GetChildren()) do

                            if not v.Character.Head:FindFirstChild("ESP") then

                                            local BillboardGui = Instance.new("BillboardGui")

                                                            local TextLabel = Instance.new("TextLabel")

                                                                            BillboardGui.Parent = v.Character.Head

                                                                                            BillboardGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

                                                                                                            BillboardGui.Active = true

                                                                                                                            BillboardGui.Name = "ESP"

                                                                                                                                            BillboardGui.AlwaysOnTop = true

                                                                                                                                                            BillboardGui.LightInfluence = 1.000

                                                                                                                                                                            BillboardGui.Size = UDim2.new(0, 200, 0, 50)

                                                                                                                                                                                            BillboardGui.StudsOffset = Vector3.new(0, 2.5, 0)

                                                                                                                                                                                                            TextLabel.Parent = BillboardGui

                                                                                                                                                                                                                            TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)

                                                                                                                                                                                                                                            TextLabel.BackgroundTransparency = 1.000

                                                                                                                                                                                                                                                            TextLabel.Size = UDim2.new(0, 200, 0, 50)

                                                                                                                                                                                                                                                                            TextLabel.Font = Enum.Font.GothamBold

                                                                                                                                                                                                                                                                                            TextLabel.Text = v.Name

                                                                                                                                                                                                                                                                                                            TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)

                                                                                                                                                                                                                                                                                                                            TextLabel.TextScaled = true

                                                                                                                                                                                                                                                                                                                                            TextLabel.TextSize = 14.000

                                                                                                                                                                                                                                                                                                                                                            TextLabel.TextStrokeTransparency = 0.000

                                                                                                                                                                                                                                                                                                                                                                            TextLabel.TextWrapped = true

                                                                                                                                                                                                                                                                                                                                                                                        end

                                                                                                                                                                                                                                                                                                                                                                                                end

                                                                                                                                                                                                                                                                                                                                                                                                    end) 

                                                                                                                                                                                                                                                                                                                                                                                                    end

                                                                                                                                                                                                                                                                                                                                                                                                    end)

                                                                                                                                                                                                                                                                                                                                                                                                    -------------

local Toggle3 = Section3:CreateToggle("UI Toggle", nil, function(State)

    Window:Toggle(State)

        end)

            Toggle3:CreateKeybind(tostring(Config.Keybind):gsub("Enum.KeyCode.", ""), function(Key)

                    Config.Keybind = Enum.KeyCode[Key]

                            end)

                                    Toggle3:SetState(true)

                                            -------------

        local Button1 = Section5:CreateButton("Start Island", function()

            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2127.97607, 50.3857689, -1623.94238, 0.999503493, 1.30760014e-09, -0.0315081626, -5.96462713e-10, 1, 2.25793428e-08, 0.0315081626, -2.25493384e-08, 0.999503493)

                    end)

                    -------------

local Button2 = Section5:CreateButton("Pirate Island", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(3413.50586, 39.6031036, -477.154175, 0.357177854, -1.10997798e-08, -0.934036374, -1.86986515e-08, 1, -1.9034081e-08, 0.934036374, 2.42637732e-08, 0.357177854)

    end)

    -------------

local Button3 = Section5:CreateButton("Soldier Island", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2033.89722, 39.3365479, 206.956146, 1, 4.00744753e-08, -1.65375228e-13, -4.00744753e-08, 1, -4.71495287e-09, 1.65186278e-13, 4.71495287e-09, 1)

    end)

    -------------

local Button4 = Section5:CreateButton("Shark Island", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(3186.31079, 10.1226444, 1423.65283, 1, -2.22905836e-08, 3.90886542e-13, 2.22905836e-08, 1, -9.1914437e-08, -3.88837698e-13, 9.1914437e-08, 1)

    end)

    -------------

local Button5 = Section5:CreateButton("Chef Ship", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-100.236603, 49.7815437, 86.1034164, 1, 4.41875869e-08, 5.08051175e-14, -4.41875869e-08, 1, 7.4752684e-08, -4.7501977e-14, -7.4752684e-08, 1)

    end)

    -------------

local Button6 = Section5:CreateButton("Snow Island", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1106.19934, 18.0717258, 1718.84924, 1, 5.91690394e-08, -9.07635512e-14, -5.91690394e-08, 1, -4.46844091e-08, 8.81196158e-14, 4.46844091e-08, 1)

end)

    -------------

local Button7 = Section5:CreateButton("Desert Island", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1522.46606, 12.8860664, 2000.42065, 1, -1.0108014e-08, 8.4293053e-14, 1.0108014e-08, 1, -4.23093027e-08, -8.38653894e-14, 4.23093027e-08, 1)

end)

-------------

local Button8 = Section5:CreateButton("Sky Island", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(238.406998, 402.736725, 4078.00293, 1, -1.00379715e-07, -2.41481419e-14, 1.00379715e-07, 1, 4.17610266e-08, 1.99561809e-14, -4.17610266e-08, 1)

end)

    -------------

local Button9 = Section5:CreateButton("Bubble Island", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5649.6167, 9.74540424, 3511.44214, -0.499068797, -7.21993629e-08, -0.866562366, -2.33216273e-08, 1, -6.98856439e-08, 0.866562366, -1.46681005e-08, -0.499068797)

end)

    -------------

local Button10 = Section5:CreateButton("Lobby Island", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2914.14233, 13.0210848, 4247.37891, 1, -4.1534868e-08, 4.05887401e-13, 4.1534868e-08, 1, -9.82721957e-08, -4.01805677e-13, 9.82721957e-08, 1)

end)

    -------------

local Button11 = Section5:CreateButton("Zombie Island", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1684.14612, 15.7372208, 6579.64648, -0.846568525, -6.14040161e-08, 0.53227973, -6.50786225e-09, 1, 1.05009939e-07, -0.53227973, 8.54341096e-08, -0.846568525)

end)

    -------------

local Button12 = Section5:CreateButton("War Island", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(6538.91162, 49.6020737, 861.779053, 0.270468831, -1.27588109e-07, -0.962728739, 1.7199163e-08, 1, -1.27695643e-07, 0.962728739, 1.79795627e-08, 0.270468831)

end)

-------------

local Button13 = Section5:CreateButton("Fishland", function()

    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2868.65039, 40.2424355, 9136.1875, 1, -3.66097872e-08, 2.89412121e-15, 3.66097872e-08, 1, -5.3281396e-10, -2.87461489e-15, 5.3281396e-10, 1)

    end)
