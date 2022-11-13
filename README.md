# nyula
i work on nyula on my freetime, contact me at my [discord server](https://www.discord.gg/AKvFNhfmYk)
## Scripts
### Untitled Hood / Da Hood / Hood Customs V4.1
```loadstring(game:HttpGet("https://raw.githubusercontent.com/nyulachan/nyula/main/nyulauh", true))()```
### Hood Modded V4.1
```loadstring(game:HttpGet("https://raw.githubusercontent.com/nyulachan/nyula/main/nyuladhm", true))()```
## Other Scripts
### SouthWest Florida
```loadstring(game:HttpGet("https://raw.githubusercontent.com/nyulachan/nyula/main/Games/SouthwestFlorida", true))()```
### Fov Sil Aim
```
_G.settings = { 
    -- Script Only Executes Once But The Settings Can Execute Multiple Times
    prediction = 0.14284, -- [ Lower Prediction: Lower Ping | Higher Prediction: Higher Ping  ]
    autoprediction = false, -- [ Sets Prediction Value For You ]
    circlesize = 75, -- [ Size Of The Fov Circle ]
    togglekey = "q", -- [ Key To Toggle ]
    visiblecircle = true, -- [ Toggle If The Circle Is Visible ]
    filledcircle = false, -- [ Toggle If The Circle Is Filled ]
    circlethickness = 2, -- [ How Thick The Outside Of The Circle Is ]
    circletransparency = 1, -- [ How Transparent The Circle Is ]
    colorR = 255, -- [ R Value Of The RGB (0-255) ]
    colorG = 255, -- [ G Value Of The RGB (0-255) ]
    colorB = 255, -- [ B Value Of The RGB (0-255) ]
    randopos = false, -- [ Randomizes Pos That The Silent Aim Targets (Not Too Far As To Miss) ]
    limiters = false, -- [ Toggle The Up And Down Limiters ]
    uplimit = 9, -- [ How Up From The Person The Silent Aim Can Be Before Aiming At Torso Level ]
    downlimit = 9, -- [ How Down From The Person The Silent Aim Can Be Before Aiming At Torso Level ]
    notifications = true, -- [ Shows Notification At The Bottom Left When FOV SIL Toggled ]
}
loadstring(game:HttpGet("https://raw.githubusercontent.com/nyulachan/nyula/main/Standalones/FovSilentAim"))()
```
### Smooth Aim
```
_G.config = {
    -- Aimlock,
    aimlockpred = 0.14824,
    aimlocktogglemode = true,
    aimlocktogglekey = "e",
    aimlockpart = "HumanoidRootPart",
    smoothing = true,
    smoothamount = 2
}
if not _G.isloaded then
    loadstring(game:HttpGet("https://raw.githubusercontent.com/nyulachan/nyula/main/smooth"))()
end
```
### Standalone Aimlock
```
_G.aimlock = {
    ["Key"] = "e",
    ["Mode"] = "Toggle", -- "Toggle" or "Hold"
    ["Prediction"] = 0.14284, -- Lower for Lower Ping, Higher for Higher Ping
    ["Auto-Prediction"] = true, -- Kinda iffy
    ["Aimpart"] = "HumanoidRootPart", -- "Head", or any body part
    ["Smoothing"] = false,
    ["Smoothing-Amount"] = 0.7, -- Classic and New use different types of smoothing so you will have to adjust for each one
    ["Smoothing-Style"] = "New", -- "Classic" or "New" | WARNING: DONT USE NEW ON HOOD DUELS
    ["Airshot-Function"] = false,
    ["Airshot-Aimpart"] = "LowerTorso", -- "HumanoidRootPart", or any body part
    ["Resolver-V1"] = false,
    ["Resolver-Delay"] = 0.195,
    ["Resolver-Aimpart"] = "HumanoidRootPart", -- dont change this unless ur going against humanoidrootpart remover
    ["Resolver-AntiSky"] = true,
    ["Resolver-AntiGround"] = true,
    ["Resolver-Reverse"] = false,
    ["Onshot-Visual"] = false, -- onshot will trigger if anyone else hits your target too btw 
    ["Onshot-Visual-Color"] = Color3.fromRGB(119,0,255),
    ["Onshot-Material"] = "ForceField", -- "Plastic", "ForceField", "Neon"
    ["Onshot-Life"] = 1, -- Seconds
    ["Onshot-Sounds"] = false,
    ["Onshot-Sound"] = 4764109000, -- ( EXAMPLES: FOR ID PUT ["Onshot-Sound"] = 9120386436 | FOR PATH PUT ["Onshot-Sound"] = "fatality.wav" <- FILE WOULD BE LOCATED AT executor/workspace/fatality.wav )
    ["Check-For-Part"] = "HumanoidRootPart", -- dont change this unless ur going against humanoidrootpart remover
    ["FOV-Check"] = true,
    ["FOV-Check-Color"] = Color3.fromRGB(119,0,255),
    ["FOV-Size"] = 100,
    ["Circle-Thickness"] = 2,
    ["Filled-Circle"] = false,
    ["Circle-Transparency"] = 1, --Invisible
    ["Visible-Check"] = false,
    ["Down-Check"] = false, -- Tested on Hood Customs and Untitled Hood, dk if it works on da hood or any other game
    ["Hood-Duels"] = false, -- use if hood duels
}

loadstring(game:HttpGet("https://raw.githubusercontent.com/nyulachan/nyula/main/Standalones/Aimlock", true))()
```
### Standalone SilentAim
```
_G.TargetAim = {
    ["Key"] = "e",
    ["Mode"] = "Toggle", -- "Toggle" or "Hold"
    ["Prediction"] = 0.12831, -- Lower if Lower Ping, Higher if Higher Ping
    ["Auto-Prediction"] = false,
    ["Aimpart"] = "HumanoidRootPart",
    ["Face-Target"] = false,
    ["Notif-Toggle"] = false,
    ["Chat-Toggle"] = false,
    ["View-Toggle"] = false,
    ["Resolver-V1"] = false,
    ["Resolver-Delay"] = 0.195,
    ["Resolver-Aimpart"] = "HumanoidRootPart",
    ["Resolver-AntiSky"] = false,
    ["Resolver-AntiGround"] = false,
    ["Resolver-Reverse"] = false,
    ["Orbit-Toggle"] = false,
    ["Orbit-Speed"] = 8,
    ["Orbit-Size"] = 8,
    ["Orbit-Height"] = 0, -- No Negatives
    ["Vertical-Velocity-Toggle"] = false,
    ["Vertical-Velocity"] = 0,
    ["Horizontal-Velocity-Toggle"] = false,
    ["Horizontal-Velocity"] = 0,
    ["Onshot-Visual"] = false,
    ["Onshot-Visual-Color"] = Color3.fromRGB(119,0,255),
    ["Onshot-Visual-Material"] = "ForceField", -- "Plastic", "ForceField", "Neon"
    ["Onshot-Visual-Life"] = 1, -- Seconds
    ["Onshot-Sound"] = false,
    ["Onshot-Sound-Sound"] = 12413331,
    ["Check-For-Part"] = "HumanoidRootPart",
    ["FOV-Check"] = true,
    ["FOV-Check-Color"] = Color3.fromRGB(119,0,255),
    ["FOV-Size"] = 100,
    ["Circle-Thickness"] = 2, 
    ["Filled-Circle"] = false,
    ["Circle-Transparency"] = 1, --Invisible
    ["Visible-Check"] = false,
    ["Down-Check"] = false, -- For Hood Customs and Untitled Hood
    ["Dot"] = true,
    ["Dot-Color"] = Color3.fromRGB(119,0,255),
    ["Tracer"] = false,
    ["Tracer-Color"] = Color3.fromRGB(119,0,255),
    ["Highlight"] = false,
    ["Highlight-Color"] = Color3.fromRGB(119,0,255),
}
loadstring(game:HttpGet("https://raw.githubusercontent.com/nyulachan/nyula/main/Standalones/SilentAim", true))()
```
### Nyula UH V4
```loadstring(game:HttpGet("https://raw.githubusercontent.com/nyulachan/nyula/main/nyulauhv4", true))()```
### Nyula UH V3
```loadstring(game:HttpGet("https://raw.githubusercontent.com/nyulachan/nyula/main/nyulauhv3", true))()```
### Nyula DHM V3
```loadstring(game:HttpGet("https://raw.githubusercontent.com/nyulachan/nyula/main/nyuladhmv3", true))()```
