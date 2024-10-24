
local part = script.Parent

local function onTouch(hit)
    local character = hit.Parent
    if character and character:FindFirstChild("Humanoid") then
        part.BrickColor = BrickColor.Random()
    end
end

part.Touched:Connect(onTouch)
