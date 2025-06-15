# Lume Library V2

Loadstring
```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/ItzzAvi535/Lume-Library-V2/refs/heads/main/Library", true))()
```
Create Window:
```lua
local window = library:AddWindow("My Awesome Script", {
    main_color = Color3.fromRGB(41, 74, 122),
    main_size = Vector2.new(600, 340),
    Key_system = true, -- Set to false to disable key system
    Key = "Avi"
})
```

AddLabel:
```lua
Main:AddLabel("This is a test label")
```

AddTab:
```lua
local Main = window:AddTab("Main")
```
AddButton:
```lua
Main:AddButton("Test Button", function()
    -- your code here
end)
```
AddToggle:
```lua
local Toggle = Main:AddToggle("Test Toggle", function(state)
    print("Toggle state:", state)
end)
```
AddTextBox:
```lua
Main:AddTextBox("Test Textbox", function(text)
    print("Text entered:", text)
end)
```
AddSlider:
```lua
local slider = Main:AddSlider("Test Slider", function(value)
    print("Slider value:", value)
end, {
    min = 16,
    max = 100
})
slider:Set(16)
```
AddDropdown:
```lua
local dropdown = Main:AddDropdown("Test Dropdown", function(text)
    print("Dropdown selected:", text)
end)
local Option1 = dropdown:Add("Option1")
local Option2 = dropdown:Add("Option2")
local Option3 = dropdown:Add("Option3")
```
