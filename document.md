# Toxic Library
Use this document to help create a UI useing Toxic UI.

## Booting the Library
``` lua
Local ToxicLib = loadstring(game:HttpGet(("https://raw.githubusercontent.com/HauntedAura/Toxic-Hub/main/source")))()
```

## Creating a Window

``` lua
Local Window = ToxicLib:CreateLib("TITLE", "DarkTheme")

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
Local Tab = Window:CreateTab("Tab Name")
```

## Creating a Section
``` lua
Local Section = Tab:CreateSection("Section Name")
```

## Creating a Label
``` lua
Local Label = Tab:CreateLabel("Label")
```

## Creating a Button
``` lua
Local Button = Tab:CreateButton("Button Name", function()
    print("Clicked")
end)
```

## Creating a Slider
``` lua
Local Slider = Tab:CreateSlider("Tab Name", 0, 100, function(v) -- 0 (Min value) | 100 (Max value)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = v
end)
```

## Creating a Toggle
``` lua
Local Toggle = Tab:CreateToggle("Tab Name", function(state)
    if state then
      print("On)
    else
      print("Off")
     end
end)
```

## Creating a Dropdown
``` lua
Local Dropdown = Tab:CreateDropdown("Tab Name", {"Option 1", "Option 2", "Option 3"}, function(currentoption)
    print(currentoption)
end)
```
