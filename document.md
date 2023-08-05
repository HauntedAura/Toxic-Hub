# Toxic Library
Use this document to help create a UI useing Toxic UI.

## Booting the Library
``` lua
local ToxicLib = loadstring(game:HttpGet(("https://raw.githubusercontent.com/HauntedAura/Toxic-Hub/main/source")))()
```

## Creating a Window

``` lua
local Window = ToxicLib:CreateLib("TITLE", "DarkTheme")

--[[
Themes:
  DarkTheme
  MercuryTheme
  CherryTheme
  GrapeTheme
  Ocean
  Midnight
 ]]--
```

## Creating a Tab
``` lua
local Tab = Window:CreateTab("Tab Name")
```

## Creating a Section
``` lua
local Section = Tab:CreateSection("Section Name")
```

## Creating a Label
``` lua
local Label = Tab:CreateLabel("Label")
```

## Creating a Button
``` lua
local Button = Tab:CreateButton("Button Name", function()
    print("Clicked")
end)
```

## Creating a Slider
``` lua
local Slider = Tab:CreateSlider("Tab Name", 0, 100, function(v) -- 0 (Min value) | 100 (Max value)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = v
end)
```

## Creating a Toggle
``` lua
local Toggle = Tab:CreateToggle("Tab Name", function(state)
    if state then
      print("On")
    else
      print("Off")
     end
end)
```

## Creating a Dropdown
``` lua
local Dropdown = Tab:CreateDropdown("Tab Name", {"Option 1", "Option 2", "Option 3"}, function(currentoption)
    print(currentoption)
end)
```
