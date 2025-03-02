local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()


local Window = Fluent:CreateWindow({
    Title = "menu free" .. Fluent.Version,
    TabWidth = 160, Size = UDim2.fromOffset(580, 460), Theme = "Dark"
})


local Tabs = {
    Main = Window:AddTab({ Title = "tp gas" }),
    Settings = Window:AddTab({ Title = "by cezar", Icon = "by cezar" })
}
  

Tabs.Main:AddButton({ Title = "pegar gas", Callback = function() 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-489.0975646972656, 4.777997016906738, -49.132545471191406)
 end })


Tabs.Main:AddButton({ Title = "loc 1 ", Callback = function() 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-61.63109588623047, 5.763457298278809, 657.1148071289062)
 end })


Tabs.Main:AddButton({ Title = "loc 2", Callback = function() 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-242.37612915039062, 6.760883808135986, -104.35148620605469)
 end })

Tabs.Main:AddButton({ Title = "loc 3", Callback = function() 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-804.6704711914062, 6.7268571853637695, 49.57543182373047)
 end })



Window:SelectTab(1)
Fluent:Notify({ Title = "Fluent", Content = "The script has been loaded." })
