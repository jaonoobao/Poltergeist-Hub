local gameid = game.GameId
    local supportedGames = {
        [2753915549] = "https://raw.githubusercontent.com/berhddb/PoltergeistHub/refs/heads/main/bloxfruits?token=GHSAT0AAAAAAC63RFAQ44QG4Z54ITZ3ZFIAZ5OKXRA", -- Blox Fruits
        [5569032992] = "[https://raw.githubusercontent.com/jaonoobao/Poltergeist-Hub-DW-loader/refs/heads/main/README.md](https://raw.githubusercontent.com/jaonoobao/Poltergeist-Hub-DW/refs/heads/main/README.md)" -- DW (Dandy's World)
    }

    if supportedGames[gameid] then
        loadstring(game:HttpGet(supportedGames[gameid], true))()
        print("Game supported!")
    else
      warn("Game not supported.")
    end
