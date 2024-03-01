-- create By FRITE
while true do
    wait()
    
    local args1 = {
        [1] = {
            ["multiply"] = 5,
            ["action"] = "hit",
            ["enemyHum"] = workspace.dummies.TrainingDummy5.Humanoid
        }
    }

    game:GetService("ReplicatedStorage").DamageEvent:FireServer(unpack(args1))

    local args2 = {
        [1] = {
            ["multiply"] = 5,
            ["action"] = "damage",
            ["enemyChar"] = workspace.dummies.TrainingDummy5
        }
    }

    game:GetService("ReplicatedStorage").Events.WaterbeamEvent:FireServer(unpack(args2))
end
