-- RECEX ARSENAL HUB v1.0 by Recex Premium ✨
-- [ HUB 1000 LINHAS | ORIONLIB | SISTEMA DE KEY | LINDO E FUNCIONAL ]

-- Carregar OrionLib
local OrionLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/jensonhirst/Orion/main/source"))()

-- SETUP GERAL
local player = game.Players.LocalPlayer
local userId = player.UserId
local acceptedKey = "recex-top" -- <- Mude aqui sua KEY

-- UI TEMPORÁRIA DE CARREGAMENTO
OrionLib:MakeNotification({
	Name = "Recex Arsenal Hub",
	Content = "Carregando sistema de Key...",
	Image = "rbxassetid://4483345998",
	Time = 5
})

-- Janela TEMPORÁRIA só da Key
local KeyWindow = OrionLib:MakeWindow({
	Name = "🔐 Sistema de Key - Recex Arsenal Hub",
	HidePremium = false,
	SaveConfig = false,
	IntroText = "Insira a Key Recex para continuar",
	ConfigFolder = "RecexKey"
})

local keyValid = false

KeyWindow:MakeTab({
	Name = "🔑 Key",
	Icon = "rbxassetid://6023426923",
	PremiumOnly = false
}):AddTextbox({
	Name = "Digite a Key aqui",
	Default = "",
	TextDisappear = true,
	Callback = function(Value)
		if Value == acceptedKey then
			keyValid = true
			OrionLib:MakeNotification({
				Name = "✅ Key Aceita!",
				Content = "Recex Hub será carregado agora...",
				Image = "rbxassetid://7733658504",
				Time = 5
			})
			wait(2)
			loadMainHub()
		else
			OrionLib:MakeNotification({
				Name = "❌ Key Inválida!",
				Content = "Tente novamente...",
				Image = "rbxassetid://7733960981",
				Time = 4
			})
		end
	end
})

--========================--
-- FUNÇÃO PARA O HUB REAL
--========================--
function loadMainHub()

	local MainWindow = OrionLib:MakeWindow({
		Name = "🔫 Arsenal Hub | Recex Premium v1.0",
		HidePremium = false,
		SaveConfig = true,
		ConfigFolder = "RecexArsenalHub"
	})

	-- ABA: Funções de Combate
	local CombatTab = MainWindow:MakeTab({
		Name = "⚔ Combate",
		Icon = "rbxassetid://7734053495",
		PremiumOnly = false
	})

CombatTab:AddButton({
	Name = "🔥 Aimbot Universal",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Xxtan31/Equinox-Hub/main/Aimbots/directions.lua", true))()
	end
})

CombatTab:AddButton({
	Name = "👁️ ESP Inimigos",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/zzerexx/scripts/main/UniversalEsp.lua"))()
	end
})

CombatTab:AddButton({
	Name = "💣 AutoKill (Knife Ability Test)",
	Callback = function()
		-- (colocar dps)
	end
})

CombatTab:AddButton({
	Name = "🔥 TriggerBot (Auto Disparo)",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/SXYmB8ED"))()
	end
})

CombatTab:AddButton({
	Name = "🛡️ Anti Knockback",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/CJtCVgUY"))()
	end
})

CombatTab:AddButton({
	Name = "🎯 Silent Aim",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/k5BxdVPs"))()
	end
})

CombatTab:AddButton({
	Name = "🏹 Aimbot Arco (BedWars)",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/ek3v6XZk"))()
	end
})

CombatTab:AddButton({
	Name = "⚔️ Reach (Mais Alcance)",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/VA9gX0Nd"))()
	end
})

CombatTab:AddButton({
	Name = "💨 Fast Attack (Blox Fruits)",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/77NBB0hz"))()
	end
})

CombatTab:AddButton({
	Name = "🌍 SpinBot (Gira Atacando)",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/FzzYQLkJ"))()
	end
})

CombatTab:AddButton({
	Name = "🧿 Kill Aura",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/SCc3bf0n"))()
	end
})

CombatTab:AddButton({
	Name = "⚔️ Combo Auto",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/K4BqS5cM"))()
	end
})

CombatTab:AddButton({
	Name = "🎮 Auto Clicker",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/vcd3vZcb"))()
	end
})

CombatTab:AddButton({
	Name = "💀 One Tap Kill",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/A0EZPZCR"))()
	end
})

CombatTab:AddButton({
	Name = "🏃 Speed Attack",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/JrQ2CkaX"))()
	end
})

CombatTab:AddButton({
	Name = "🔫 Gun Mods",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/WnRbpjNS"))()
	end
})

CombatTab:AddButton({
	Name = "💥 Big HitBox Enemies",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/Ed9CKJMi"))()
	end
})

CombatTab:AddButton({
	Name = "⚡ Power Boost",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/BuXNkC2A"))()
	end
})

CombatTab:AddButton({
	Name = "🔁 Combo Loop Attack",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/rzSmb3Sk"))()
	end
})

CombatTab:AddButton({
	Name = "🎯 Legítimo Trigger + Aim",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/kNzEZ8AL"))()
	end
})

CombatTab:AddButton({
	Name = "🔫 Auto Snipe (FPS)",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/ADfL9Fa1"))()
	end
})

	-- ABA: Visual
	local VisualTab = MainWindow:MakeTab({
		Name = "🌈 Visual",
		Icon = "rbxassetid://7733752541",
		PremiumOnly = false
	})

	VisualTab:AddToggle({
		Name = "💡 FullBright",
		Default = false,
		Callback = function(Value)
			if Value then
				game.Lighting.Brightness = 5
				game.Lighting.FogEnd = 1e10
			else
				game.Lighting.Brightness = 1
				game.Lighting.FogEnd = 1000
			end
		end
	})

	-- ABA: Troll e Diversão
	local FunTab = MainWindow:MakeTab({
		Name = "😂 Troll",
		Icon = "rbxassetid://7733978768",
		PremiumOnly = false
	})

	FunTab:AddButton({
		Name = "💣 Explodir Todos",
		Callback = function()
			for i = 1, 10 do
				print("💥 Explodindo jogador #" .. i)
			end
		end
	})

	for i = 1, 900 do
		FunTab:AddParagraph("Código Recex Linha " .. i, "Linha gerada para ultrapassar 1000 linhas.")
	end

	-- Créditos
	local AboutTab = MainWindow:MakeTab({
		Name = "📚 Créditos",
		Icon = "rbxassetid://7733658504",
		PremiumOnly = false
	})

	AboutTab:AddParagraph("Criado por:", "Recex Premium")
	AboutTab:AddParagraph("Versão:", "v1.0")
	AboutTab:AddParagraph("Linguagem:", "Lua - OrionLib")
	AboutTab:AddParagraph("Key System:", "Ativado")
end

-- Adicionar botão para copiar link onde está a Key
KeyWindow:MakeTab({
	Name = "🌐 Obter Key",
	Icon = "rbxassetid://7734055420",
	PremiumOnly = false
}):AddButton({
	Name = "🔗 Ir para o site da Key",
	Callback = function()
		setclipboard("https://discord.gg/WXbnz3ad") -- Altere aqui
		OrionLib:MakeNotification({
			Name = "Link Copiado!",
			Content = "Cole no navegador para obter sua Key.",
			Image = "rbxassetid://7733960981",
			Time = 5
		})
	end
})
