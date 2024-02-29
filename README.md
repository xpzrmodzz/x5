--create by FRITE--
while true do wait()
local args = {
    [1] = {
        ["multiply"] = 5,
        ["action"] = "hit",
        ["enemyHum"] = workspace.dummies.TrainingDummy5.Humanoid
    }
}

game:GetService("ReplicatedStorage").DamageEvent:FireServer(unpack(args))
end
