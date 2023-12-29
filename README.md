local Spawner = 

loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors%20Entity%20Spawner/Source.lua"))()

-- Create entity
                local entity5 = Creator.createEntity({
                    CustomName = "Primes A-60", -- Custom name of your entity
                    Model = "https://github.com/Johnny39871/assets/blob/main/A-60%20refined.rbxm?raw=true", -- Can be GitHub file or rbxassetid
                    Speed = 60000, -- Percentage, 100 = default Rush speed
                    DelayTime = 0.1, -- Time before starting cycles (seconds)
                    HeightOffset = 4,
                    CanKill = true,
                    KillRange = 100000,
                    BreakLights = true,
                    BackwardsMovement = false,
                    FlickerLights = {
                        true, -- Enabled/Disabled
                        0.1, -- Time (seconds)
                    },
                    Cycles = {
                        Min = 1,
                        Max = 1,
                        WaitTime = 0,
                    },
                    CamShake = {
                        true, -- Enabled/Disabled
                        {200.5, 20, 0.1, 1}, -- Shake values (don't change if you don't know)
                        100, -- Shake start distance (from Entity to you)
                    },
                    Jumpscare = {
                        true, -- Enabled/Disabled
                        {
                            Image1 = "rbxassetid://11131703032", -- Image1 url
                            Image2 = "rbxassetid://3413871766", -- Image2 url
                            Shake = true,
                            Sound1 = {
                                3537873683, -- SoundId
                                { Volume = 10 }, -- Sound properties
                            },
                            Sound2 = {
                                5263560566, -- SoundId
                                { Volume = 10 }, -- Sound properties
                            },
                            Flashing = {
                                true, -- Enabled/Disabled
                                Color3.fromRGB(255,0,0), -- Color
                            },
                            Tease = {
                                true, -- Enabled/Disabled
                                Min = 1,
                                Max = 1,
                            },
                        },
                    },
                    CustomDialog = {"You died to who you call PrimesA-60...", "Try your best to out-run him.", "I really don't have nothing else", "Just try your best to Hide when you can."}, -- Custom death message
                })

                ------------------------
                Creator.runEntity(entity5)
                -- Run the created entity
Spawner.runEntity(entityTable)
