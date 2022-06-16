wait (0.8)

game.StarterGui:SetCore("SendNotification", {
    Title = "Ur a nice farmer?";
    Text = "Let's see!";
    Duration = "15";
    })

wait (0.8)

game.StarterGui:SetCore("SendNotification", {
    Title = "MattTheFarmer";
    Text = "Loading!";
    Duration = "15";
    })

wait (0.8)

game.StarterGui:SetCore("SendNotification", {
    Title = "MattTheFarmer";
    Text = "Executed!";
    Duration = "15";
    })

wait (0.7)

    local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
    local Window = Library.CreateLib("FarmerHub", "Sentinel")

    --Main
    local Main = Window:NewTab("Main")
    local MainSection = Main:NewSection("Main")

    MainSection:NewButton("Shader", "Shader", function()

        game.StarterGui:SetCore("SendNotification", {
            Title = "FarmerHub";
            Text = "Cradit to it 1tsJustgp";
            Duration = "15";
            })

            wait (1.3)

        game.StarterGui:SetCore("SendNotification", {
            Title = "FarmerHub";
            Text = "Shaders Loading";
            Duration = "15";
            })
            
            wait (1.5)
            
            local runDummyScript = function(f,scri)
            local oldenv = getfenv(f)
            local newenv = setmetatable({}, {
            __index = function(_, k)
            if k:lower() == 'script' then
            return scri
            else
            return oldenv[k]
            end
            end
            })
            setfenv(f, newenv)
            ypcall(function() f() end)
            end
            cors = {}
            mas = Instance.new("Model",game:GetService("Lighting")) 
            mas.Name = "CompiledModel"
            o2 = Instance.new("BloomEffect")
            o3 = Instance.new("BlurEffect")
            o4 = Instance.new("ColorCorrectionEffect")
            o5 = Instance.new("SunRaysEffect")
            o2.Parent = mas
            o2.Size = 56
            o2.Threshold = 0.98000001907349
            o3.Parent = mas
            o3.Size = 1.2199997901917
            o4.Parent = mas
            o4.Contrast = 0.52999997138977
            o4.Saturation = 0.098999999463558
            o4.Brightness = 0.070000000298023
            o5.Parent = mas
            o5.Intensity = 0.090000003576279
            mas.Parent = workspace
            mas:MakeJoints()
            local mas1 = mas:GetChildren()
            for i=1,#mas1 do
            mas1[i].Parent = game:GetService("Lighting") 
            ypcall(function() mas1[i]:MakeJoints() end)
            end
            mas:Destroy()
            for i=1,#cors do
            coroutine.resume(cors[i])
            end
            game:GetService("RunService").RenderStepped:Connect(function()
            game:GetService("Lighting").Ambient = Color3.new(0, 0, 0)
            game:GetService("Lighting").Brightness = 1
            game:GetService("Lighting").ColorShift_Bottom = Color3.new(0, 0, 0)
            game:GetService("Lighting").ColorShift_Top = Color3.new(0, 0, 0)
            game:GetService("Lighting").GlobalShadows = false
            game:GetService("Lighting").OutdoorAmbient = Color3.new(0.529412, 0.529412, 0.501961)
            game:GetService("Lighting").Outlines = true
            game:GetService("Lighting").GeographicLatitude = 41.733299255371
            game:GetService("Lighting").TimeOfDay = TimeOfDay
            game:GetService("Lighting").FogColor = Color3.new(0.75, 0.75, 0.75)
            game:GetService("Lighting").FogEnd = 7777777
            game:GetService("Lighting").FogStart = 7777777
            end)
    end)

    MainSection:NewButton("God Mode (only earth)", "God modeMode rejoin for remove it", function()
		local Plr = game.Players.LocalPlayer
local GodModeBool = true

game:GetService("RunService").RenderStepped:connect(function()
if  GodModeBool  then
game.Workspace.Touchy.Part.CFrame = Plr.Character.HumanoidRootPart.CFrame + Vector3.new(0,0,1)
if Plr.PlayerGui:FindFirstChild("Popup") then
Plr.PlayerGui.Popup.Enabled = false
end
if not GodModeBool  then
return
end end end)
	end)

    MainSection:NewButton("Infiniti yield", "Infiniti yield", function()
        loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
end)

    local Main = Window:NewTab("PvP")
    local PvPSection = Main:NewSection("PvP")

    PvPSection:NewButton("Noslow", "Sciaffi Tremonici" function()
        (getgenv()).noslow = true;
        
        repeat
            wait();
        until game:IsLoaded();
        game.Players.LocalPlayer.PlayerGui:WaitForChild("HUD");
        (game:GetService("RunService")).RenderStepped:Connect(function()
            for _, v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
                if (getgenv()).noslow then
                    if v.Name == "Action" or (v.Name == "Attacking") or 
                            (v.Name == "Using") or (v.Name == "hyper") or 
                            (v.Name == "Hyper") or (v.Name == "heavy") or 
                            (v.Name == "KiBlasted") or (v.Name == "Tele") or 
                            (v.Name == "tele") or (v.Name == "Killed") or 
                            (v.Name == "Slow") then
                        v:Destroy();
                    end;
                    if game.Players.LocalPlayer.Character.Block.Value then
                        game.Players.LocalPlayer.Character.Block.Value = false;
                    end;
                end;
            end;
        end);
        
            end)

    PvPSection:NewButton("Dragon Throw Glich", "Dragon Throw Glich", function()
        local player = game.Players.LocalPlayer
        local Character = player.character
        while wait(0.3) do
            player.Backpack:WaitForChild("Dragon Throw")
            player.Backpack["Dragon Throw"].Activator:WaitForChild("Flip")
            wait()
            if (player.Backpack:FindFirstChild("Dragon Throw")) then
                repeat
                    wait()
                until player.Character:FindFirstChild("Dragon Throw")
    
                repeat
                    wait()
                until Character.Ki.Value < Character.Ki.MaxValue
            end
            repeat
                wait()
                Character["Dragon Throw"].Activator:FindFirstChild("Flip"):Destroy()
            until not Character["Dragon Throw"].Activator:FindFirstChild("Flip")
        end
    end)

    PvPSection:NewButton("Dragon Crush Glich", "Dragon Crush Glich", function()
        local player = game.Players.LocalPlayer
        local Character = player.character
        while wait(0.3) do
            player.Backpack:WaitForChild("Dragon Crush")
            player.Backpack["Dragon Crush"].Activator:WaitForChild("Flip")
            wait()
            if (player.Backpack:FindFirstChild("Dragon Crush")) then
                repeat
                    wait()
                until player.Character:FindFirstChild("Dragon Crush")
    
                repeat
                    wait()
                until Character.Ki.Value < Character.Ki.MaxValue
            end
            repeat
                wait()
                Character["Dragon Crush"].Activator:FindFirstChild("Flip"):Destroy()
            until not Character["Dragon Crush"].Activator:FindFirstChild("Flip")
        end
    
    end)

    PvPSection:NewButton("Bone Crush Glich", "Pressing V while bone crush equipped will", function()
        wait()
game:GetService("StarterGui"):SetCore("SendNotification", {Title = "FarmerHub", Text = "After glich Hard Reset For Moves  ",})

wait (1.5)

game:GetService("StarterGui"):SetCore("SendNotification", {Title = "1tsJustgp", Text = "Credits for this:1tsJustgp  ",})

local mouse = game.Players.LocalPlayer:GetMouse()
mouse.KeyDown:connect(function(key)
if key == "v" then
    local lplr = game.Players.LocalPlayer
    lplr.Character["Bone Crush"].Activator.Crash:Destroy()
end
end)

    end)

    PvPSection:NewToggle("Anchor", "Anchor Charapter", function(state)
        if state then
            game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = true 
        else
            game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = false 
        end
    end)

    local Main = Window:NewTab("Respawn")
    local RespawnSection = Main:NewSection("Respawn")

    RespawnSection:NewKeybind("Hard Reset", "Press N", Enum.KeyCode.N, function()
		print("Injected!")
print("Fast Hard Reset")
wait(0.1)

local Player = game:GetService("Players").LocalPlayer
local Mouse = Player:GetMouse()

Mouse.KeyDown:connect(function(Key)
   Key = Key:lower()
   if Key == 'n' then
       Player.Character.Humanoid.Health = 0
end
end)
	end)


    local Main = Window:NewTab("Character")
    local CharacterSection = Main:NewSection("Character")

    CharacterSection:NewButton("Hide LvL", "Hide ur Hide LvL", function()
        if not game:IsLoaded() then
			game.Loaded:Wait()
			end
			wait(2)
			game.Players.LocalPlayer.Character:FindFirstChildOfClass("Model"):Destroy()
    end)

    CharacterSection:NewButton("Hide Wings", "Hide ur Wings", function()
                

getgenv().enabler = true  


if (not game:IsLoaded()) then
    game.Loaded:Wait();
end;
local lplr=game:GetService('Players').LocalPlayer;
local char=game:GetService('Workspace'):waitForChild('Live'):waitForChild(lplr.Name);
function xd(char)
    lmfao=false;
    if (getgenv().enabler==false) then
        ran:Disconnect();
    else
        repeat wait();
            if (char:findFirstChild('RebirthWings')) then
                x=char.HumanoidRootPart.CFrame.X;
                y=char.HumanoidRootPart.CFrame.Y;
                z=char.HumanoidRootPart.CFrame.Z;
                char.HumanoidRootPart.CFrame=CFrame.new(x,y,z) + Vector3.new(0,-200,0);
                char.RebirthWings.Handle.AccessoryWeld:Destroy();
                char.HumanoidRootPart.CFrame=CFrame.new(x,y,z);
                x,y,z=nil;
                char.RebirthWings:Destroy();
                lmfao=true;
            end;
            if (char:findFirstChild('RealHalo')) then
                x=char.HumanoidRootPart.CFrame.X;
                y=char.HumanoidRootPart.CFrame.Y;
                z=char.HumanoidRootPart.CFrame.Z;
                char.HumanoidRootPart.CFrame=CFrame.new(x,y,z) + Vector3.new(0,-200,0);
                char.RealHalo.Handle.AccessoryWeld:Destroy();
                char.HumanoidRootPart.CFrame=CFrame.new(x,y,z);
                x,y,z=nil;
                char.RealHalo:Destroy();
                lmfao=true;
            end;
        until lmfao==true or getgenv().enabler==false;
    end;
end;
repeat wait()
    for i,v in pairs(char:getChildren()) do
        if v:IsA('Model') then
            lmao=true;
            xd(char);
            break;
        end;
    end;
until lmao==true;
lmao=false;
lplr.CharacterRemoving:connect(function() lmfao=true;end);
lplr.CharacterAdded:connect(function(v)
    char=v;
    xd(char);
    print('reconnected');
end);
    end)



    local Main = Window:NewTab("Info")
    local CreditsSection = Main:NewSection("Credits:")

    local DsgSection = Main:NewSection("gp1tsJust#3203")
    local DsmSection = Main:NewSection("MattiaXD#7826")

    local InfoSection = Main:NewSection("Info:")

    InfoSection:NewKeybind("Hide Farmer Hub", "Hide Farmer Hub", Enum.KeyCode.RightAlt, function()
        Library:ToggleUI()
    end)


    local OtherSection = Main:NewSection("Other Scripts")

    OtherSection:NewButton("1tsJustHub", "Use 1tsJustHub", function()
        --1tsJustHub

loadstring(game:HttpGet(("https://raw.githubusercontent.com/gp1tsJust/1tsJustHub-V2-DBZ/main/README.md"), true))()
    end)


