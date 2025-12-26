--糍嗘葵���凒瘝⊥�廠�𣂼�
--zy

當地老
old = hookmetamethod(game:GetService("StarterGui"), "__namecall", newcclosure(function(self, ...)
        本地方法 = getnamecallmethod()
        本地參數 = {...}
        如果方法 == "SetCore" 且 args[1] == "SendNotification" 則
            本地選項 = args[2]
            如果 type(options) == "table" 且
               tostring(options.Title) == "鈭箸𣱣鈭箄�𡁏𧋦" 和
               tostring(options.Text) == "kismile��雿�"
            然後
                local modifiedOptions = table.clone(options)
                modifiedOptions.Text = "1"
            結尾
        結尾
     返回 old(self, ...)
結尾））


local main = require(game:GetService("ReplicatedStorage").Util.CameraShaker.Main)
local returnnil = function() return nil end

main.StartShake = returnnil
main.ShakeOnce = returnnil
main.ShakeSustain = returnnil
main.CameraShakeInstance = returnnil
main.Shake = returnnil
main.Start = returnnil


game:GetService("StarterGui"):SetCore("SendNotification",{
	Title = "鈭箸𣱣鈭箄�𡁏𧋦",
	Text = "kismile��雿�",
	持續時間 = 5；
})
等待(0.1)
local Players = game:GetService("Players")
本地 RunService = 遊戲:GetService("RunService")
local LocalPlayer = Players.LocalPlayer
local Camera = workspace.CurrentCamera
本地工作區 = game:GetService("工作區")  
本地玩家 = Players.LocalPlayer  
local ui = loadstring(game:HttpGet("https://raw.githubusercontent.com/ni7ykt/test1/refs/heads/main/ui"))()  
local win = ui:new("鈭箸𣱣鈭箔葉敹�")
local UITab1 = win:Tab("砍��",'7734068321')
local UITab2 = win:Tab("�𡁏𧋦",'7734068321')
local UITab3 = win:Tab("蟡𧼮�",'7734068321')
local UITab4 = win:Tab("�訛�",'7734068321')
local UITab5 = win:Tab("隡𣳇��",'7734068321')

local about = UITab1:section("�砍��",true)

關於:標籤("kismile��雿�")
關於：標籤(“�𡁏𧋦瘚貝�鎣葉”)
local about = UITab2:section("�🇨",true)
about:Slider("閫�閫垍宴會�𦆮頝生日氖", "Slider", 128, 128, 10000, false, function(Value)
    game:GetService("Players").LocalPlayer.CameraMaxZoomDistance = Value
結尾）
-- �䌊�𢆡v4

本地切換鍵 =“�䌊�𢆡v4”
local autoV4Task = nil
local Players = game:GetService("Players")
local LocalPlayer = Players.LocalPlayer

本機函數 getToggleState(key)
    如果不是 _G.ToggleStates，則 _G.ToggleStates = {} 結束
    傳回 _G.ToggleStates[key] 或 false
結尾

本地函數呼叫AwakeningRemote()
    local Backpack = LocalPlayer:FindFirstChild("背包")
    如果不是背包，則返回結束
    
    local Awakening = Backpack:FindFirstChild("Awakening")
    如果不是覺醒狀態，則回傳結束
    
    local RemoteFunc = Awakening:FindFirstChild("RemoteFunction")
    如果不是 RemoteFunc 或不是 RemoteFunc:IsA("RemoteFunction")，則回傳結束
    
    本地成功，錯誤 = pcall(function()
        RemoteFunc:InvokeServer(true)
    結尾）
    如果不是成功的話
        warn("�䌊�𢆡v4靚��鍂憭梯揖嚗�", err)
    結尾
結尾

本地函式 toggleAutoV4(啟用)
    如果 autoV4Task 則
        task.cancel(autoV4Task)
        autoV4Task = nil
    結尾
    
    如果啟用
        autoV4Task = task.spawn(function()
            while getToggleState(toggleKey)
                呼叫喚醒遠端()
                task.wait(1)
            結尾
            autoV4Task = nil
        結尾）
    結尾
結尾

about:Toggle(toggleKey, "切換", false, function(IsEnabled)
    如果不是 _G.ToggleStates，則 _G.ToggleStates = {} 結束
    _G.ToggleStates[toggleKey] = IsEnabled
    
    toggleAutoV4(IsEnabled)
結尾）

——蝻嘥��

關於:按鈕（“憌噼��”，function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/kismile236/rjrym/refs/heads/main/fly.lua"))()
結尾）

about:Button("瘜訫予鞊∪𧑐",function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/kismile36/rjrzhongxing/refs/heads/main/rjr/fatianxiangdi"))()
結尾）

about:Button("fps隡睃�吔���䭾�訫�喲嚗�",function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/kismile236/rjrym/refs/heads/main/fpsboost"))()
結尾）

關於:按鈕（“hoho”，function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI'))()
結尾）

——憭找𥕦蠘賢躹

local attackTab = UITab3:section("蟡𧼮�",true)
local Players = game:GetService("Players")
local ReplicatedStorage = game:GetService("ReplicatedStorage")
本地工作區 = game:GetService("工作區")
本地 RunService = 遊戲:GetService("RunService")
本地玩家 = Players.LocalPlayer
local _ENV = (getgenv 或 getrenv 或 getfenv)()
本機設定 = {自動點選 = true，點選延遲 = 0.3}
本地模組 = {}
local _G = _G or getfenv(0)._G
_G.FastAttack = _G.FastAttack ~= nil 且 _G.FastAttack 或 true

本地函數 SafeWaitForChild(parent, childName)
	local success, result = pcall(function() return parent:WaitForChild(childName, 10) end)
	若不成功或沒有結果則 warn("�𧊋�𪄳��蝏�隞�: " .. childName) end
	回傳結果
結尾

本地函數 CheckAndGetCoreComponents()
	本地遠程、模組、網路、註冊攻擊、註冊命中、敵人 = nil、nil、nil、nil、nil、nil、nil
	雖然確實如此
		Remotes = SafeWaitForChild(ReplicatedStorage, "Remotes")
		Modules = SafeWaitForChild(ReplicatedStorage, "Modules")
		Net = Modules 且 SafeWaitForChild(Modules, "Net") 或 nil
		RegisterAttack = Net 且 SafeWaitForChild(Net, "RE/RegisterAttack") 或 nil
		RegisterHit = Net and SafeWaitForChild(Net, "RE/RegisterHit") or nil
		Enemies = SafeWaitForChild(workspace, "Enemies")
		如果存在遙控器、模組、網路、攻擊註冊器、命中註冊器和敵人，則
			返回 Remotes、Net、RegisterAttack、RegisterHit、Enemies
		結尾
		warn("瓲敹蝏�隞嗥撩憭梧峕蝏剝�灘�鎣葉...")
		task.wait(1)
	結尾
結尾

本地函數 IsAlive(字元)
	如果不是字符，則返回 false 結束
	local humanoid = character:FindFirstChildOfClass("Humanoid")
	回 humanoid 和 humanoid.Health 且 humanoid.Health > 0
結尾

本地函數 GetRandomValidPart(target)
	local allParts = target:GetDescendants()
	local validParts = {}
	local humanoidRootPart = target:FindFirstChild("HumanoidRootPart")
	local boneParts = humanoidRootPart and humanoidRootPart.Parent:GetDescendants() or {}
	for _, part in ipairs(allParts) do
		如果 part:IsA("BasePart") 且 part.CanCollide 且 table.find(boneParts, part) 則
			table.insert(validParts, part)
		結尾
	結尾
	返回 #validParts > 0 且 validParts[math.random(1, #validParts)] 或 target:FindFirstChild("HumanoidRootPart")
結尾

Module.FastAttack = (function()
	如果 _ENV.rz_FastAttack 存在，則傳回 _ENV.rz_FastAttack。
	local FastAttack = {
		距離 = 2500，
		attackMobs = true，
		攻擊玩家 = true，
		配備=無，
		IsRunning = _G.FastAttack,
		連續失敗次數 = 0，
		最大連續失敗次數 = 5
	}

	本機函數 ProcessEnemies(OthersEnemies, Folder)
		如果資料夾不存在或 FastAttack.attackMobs 不存在，則傳回 nil。
		local BasePart = nil
		for _, Enemy in Folder:GetChildren() do
			如果敵人是玩家角色或敵人不存活，則繼續。
			local foundPart = GetRandomValidPart(Enemy)
			如果找到部件且玩家與角色之間的距離（找到部件的位置）小於快速攻擊的距離，則
				table.insert(OthersEnemies, {Enemy, foundPart})
				基礎部件 = 找到的部件
			結尾
		結尾
		返回基礎部件
	結尾

	本機函數 ProcessRealPlayers(其他敵人)
		如果不是 FastAttack.attackPlayers，則傳回 nil。
		local BasePart = nil
		for _, OtherPlayer in Players:GetPlayers() do
			如果 OtherPlayer == Player 則繼續結束
			local OtherChar = OtherPlayer.Character
			如果 IsAlive(OtherChar) 不存在，則繼續結束
			本地找到的部分 = GetRandomValidPart(OtherChar)
			如果找到部件且玩家與角色之間的距離（找到部件的位置）小於快速攻擊的距離，則
				table.insert(OthersEnemies, {OtherChar, foundPart})
				基礎部件 = 找到的部件
			結尾
		結尾
		返回基礎部件
	結尾

	函數 FastAttack:Attack(BasePart, OthersEnemies)
		local _, Net, temp_RegisterAttack, temp_RegisterHit, _ = CheckAndGetCoreComponents()
		若 (BasePart 和 OthersEnemies 皆不滿足，且 #OthersEnemies > 0，且 temp_RegisterAttack 與 temp_RegisterHit 皆不滿足) 則
			self.consecutiveFailures = self.consecutiveFailures + 1
			如果 self.consecutiveFailures >= self.maxConsecutiveFailures 則
				self.consecutiveFailures = 0
				self.Equipped = Player.Character and IsAlive(Player.Character) and Player.Character:FindFirstChildOfClass("Tool")
			結尾
			task.delay(0.5, function() self:AttackNearest() end)
			返回
		結尾
		self.consecutiveFailures = 0
		temp_RegisterAttack:FireServer(Settings.ClickDelay 或 0)
		temp_RegisterHit:FireServer(BasePart, OthersEnemies)
	結尾

	函數 FastAttack:AttackNearest()
		如果 self.IsRunning 為假，則回傳。
		local _, _, _, _, Enemies = CheckAndGetCoreComponents()
		local OthersEnemies = {}
		local Part1 = ProcessEnemies(OthersEnemies, Enemies)
		local Part2 = ProcessRealPlayers(OthersEnemies)
		如果 #OthersEnemies > 0 則
			自身：攻擊（Part1 或 Part2，其他敵人）
		別的
			task.wait(0)
		結尾
	結尾

	函數 FastAttack:BladeHits()
		如果 self.IsRunning 為假，則回傳。
		local Equipped = Player.Character and IsAlive(Player.Character) and Player.Character:FindFirstChildOfClass("Tool")
		如果裝備了武器且裝備的工具提示不等於“槍”，則
			self:AttackNearest()
		別的
			task.wait(0)
		結尾
	結尾

	task.spawn(function()
		雖然確實如此
			task.wait(Settings.ClickDelay)
			如果 Settings.AutoClick 且 FastAttack.IsRunning 則
				快速攻擊：刀刃命中()
			別的
				task.wait()
			結尾
		結尾
	結尾）

	_ENV.rz_FastAttack = FastAttack
	返回快速攻擊
結尾）（）

——UI繡隞嗥穃
attackTab:Toggle("撘���", "FastAttackToggle", _G.FastAttack, function(state)
	如果 _ENV.rz_FastAttack 則
		_ENV.rz_FastAttack.IsRunning = 狀態
		_G.FastAttack = 狀態
	結尾
結尾）

attackTab:Textbox("攻擊範圍", "2500", function(text)
	local num = tonumber(text) 或 2500
	num = math.floor(math.clamp(num, 1, 2500))
	如果 _ENV.rz_FastAttack 則
		_ENV.rz_FastAttack.Distance = num
	結尾
結尾）

attackTab:Textbox("�🤫���", "點擊延遲", "0.3", function(text)
	local num = tonumber(text) or 0.3
	num = math.round(math.clamp(num, 0.05, 2) * 100) / 100
	Settings.ClickDelay = num
結尾）

attackTab:Toggle("��𤘪�芰�", "AttackMobsToggle", true, function(state)
	如果 _ENV.rz_FastAttack 則
		_ENV.rz_FastAttack.attackMobs = 狀態
	結尾
結尾）

AttackTab:Toggle("��梶焵摰�", "AttackPlayersToggle", true, function(state)
	如果 _ENV.rz_FastAttack 則
		_ENV.rz_FastAttack.attackPlayers = state
	結尾
結尾）

——蝏�隞�w�漤�餉��
task.spawn(function()
	雖然確實如此
		task.wait(1)
		如果不是 _ENV.rz_FastAttack 則
			warn("��𩤃�� 敹恍��𤫇�稬蝏�隞嗆𧊋摰��典�㰘蝸嚗峕�蝏剖�肽�閙�W��...")
			while not _ENV.rz_FastAttack do
				task.wait(0.5)
				如果 _G.FastAttack 則
					local Remotes, Net, RegisterAttack, RegisterHit, Enemies = CheckAndGetCoreComponents()
					Module.FastAttack = Module.FastAttack 或 (function()
						local FastAttack = {
							距離=2500，
							attackMobs=true，
							attackPlayers=true，
							配備=無，
							IsRunning=_G.FastAttack，
							連續失敗次數=0，
							maxConsecutiveFailures=5
						}

						本機函數 ProcessEnemies(OthersEnemies, Folder)
							如果資料夾不存在或 FastAttack.attackMobs 不存在，則傳回 nil。
							local BasePart = nil
							for _, Enemy in Folder:GetChildren() do
								如果敵人等於玩家角色或敵人不存活，則繼續。
								local foundPart = GetRandomValidPart(Enemy)
								如果找到部件且玩家與角色之間的距離（找到部件的位置）小於快速攻擊的距離，則
									table.insert(OthersEnemies, {Enemy, foundPart})
									基礎部件 = 找到的部件
								結尾
							結尾
							返回基礎部件
						結尾

						本機函數 ProcessRealPlayers(其他敵人)
							如果不是 FastAttack.attackPlayers，則傳回 nil。
							local BasePart = nil
							for _, OtherPlayer in Players:GetPlayers() do
								如果 OtherPlayer == Player 則繼續結束
								local OtherChar = OtherPlayer.Character
								如果 IsAlive(OtherChar) 不存在，則繼續結束
								本地找到的部分 = GetRandomValidPart(OtherChar)
								如果找到部件且玩家與角色之間的距離（找到部件的位置）小於快速攻擊的距離，則
									table.insert(OthersEnemies, {OtherChar, foundPart})
									基礎部件 = 找到的部件
								結尾
							結尾
							返回基礎部件
						結尾

						函數 FastAttack:Attack(BasePart, OthersEnemies)
							local _, Net, temp_RegisterAttack, temp_RegisterHit, _ = CheckAndGetCoreComponents()
							若 (BasePart 和 OthersEnemies 皆不滿足，且 #OthersEnemies > 0，且 temp_RegisterAttack 與 temp_RegisterHit 皆不滿足) 則
								self.consecutiveFailures = self.consecutiveFailures + 1
								如果 self.consecutiveFailures >= self.maxConsecutiveFailures 則
									self.consecutiveFailures = 0
									self.Equipped = Player.Character and IsAlive(Player.Character) and Player.Character:FindFirstChildOfClass("Tool")
								結尾
								task.delay(0.5, function() self:AttackNearest() end)
								返回
							結尾
							self.consecutiveFailures = 0
							temp_RegisterAttack:FireServer(Settings.ClickDelay 或 0)
							temp_RegisterHit:FireServer(BasePart, OthersEnemies)
						結尾

						函數 FastAttack:AttackNearest()
							如果 self.IsRunning 為假，則回傳。
							local _, _, _, _, Enemies = CheckAndGetCoreComponents()
							local OthersEnemies = {}
							local Part1 = ProcessEnemies(OthersEnemies, Enemies)
							local Part2 = ProcessRealPlayers(OthersEnemies)
							如果 #OthersEnemies > 0 則
								自身：攻擊（Part1 或 Part2，其他敵人）
							結尾
						結尾

						函數 FastAttack:BladeHits()
							local Equipped = Player.Character and IsAlive(Player.Character) and Player.Character:FindFirstChildOfClass("Tool")
							如果裝備了武器且裝備的工具提示不等於“槍”，則
								self:AttackNearest()
							結尾
						結尾

						task.spawn(function()
							雖然確實如此
								task.wait(Settings.ClickDelay)
								如果 Settings.AutoClick 且 FastAttack.IsRunning 則
									快速攻擊：刀刃命中()
								別的
									task.wait(0.1)
								結尾
							結尾
						結尾）

						_ENV.rz_FastAttack = FastAttack
						返回快速攻擊
					結尾）（）
				結尾
			結尾
		結尾
	結尾
結尾）


——蝘駁斥筆蠘

AttackTab:Textbox("�筆漲", "TranslateAccelSpeed", "颲枏�仿�筆漲��", function(Value)
    本地速度 = tonumber(值)
    如果速度
        getfenv().translateSpeed = speed
    結尾
結尾）

attackTab:Toggle("��𣳇�筆���", "TranslateAccelToggle", false, function(State)
    getfenv().translateAccelEnabled = State
    
    如果州
        如果 getfenv().sudu 則
            getfenv().sudu:Disconnect()
            getfenv().sudu = nil
        結尾
        
        getfenv().translateConnection = game:GetService("RunService").Heartbeat:Connect(function()
            如果遊戲：GetService("Players").LocalPlayer.Character 和
               game:GetService("Players").LocalPlayer.Character.Humanoid 和
               game:GetService("Players").LocalPlayer.Character.Humanoid.Parent 然後
               
                local humanoid = game:GetService("Players").LocalPlayer.Character.Humanoid
                
                如果 humanoid.MoveDirection.Magnitude > 0 則
                    local moveDirection = humanoid.MoveDirection
                    局部加速度 = 移動方向 * (getfenv().translateSpeed 或 50) / 30
                    
                    game:GetService("Players").LocalPlayer.Character:TranslateBy(acceleration)
                結尾
            結尾
        結尾）
    別的
        如果 getfenv().translateConnection 則
            getfenv().translateConnection:Disconnect()
            getfenv().translateConnection = nil
        結尾
    結尾
結尾）

——訥謔蠘
local about = UITab4:section("�訛�",true)


local ESPConfig = {
    MainSwitch = false，     
    ShowNameDistance = false，
    ShowTracer = false，       
    顯示健康狀況 = false        
}

local ESPElements = {}

本地函數 CleanupPlayerESP(player)
    如果 ESPElements[player.UserId] 不存在，則傳回結束
    
    如果 ESPElements[player.UserId].NameHealthESP 為真，則
        ESPElements[player.UserId].NameHealthESP:Destroy()
        ESPElements[player.UserId].NameHealthESP = nil
    結尾
    如果 ESPElements[player.UserId].NameHealthUpdateConn 則
        ESPElements[player.UserId].NameHealthUpdateConn:Disconnect()
        ESPElements[player.UserId].NameHealthUpdateConn = nil
    結尾
    
    如果 ESPElements[player.UserId].Tracer 則
        ESPElements[player.UserId].Tracer:Remove()
        ESPElements[player.UserId].Tracer = nil
    結尾
    如果 ESPElements[player.UserId].TracerConn 存在，則
        ESPElements[player.UserId].TracerConn:Disconnect()
        ESPElements[player.UserId].TracerConn = nil
    結尾
結尾

本機函數 CreateNameDistanceHealthESP(player)
    如果玩家不是 Character 角色，或玩家不是 Head 角色，則會回傳。
    local head = player.Character.Head
    
    如果 ESPElements[player.UserId] 存在且 ESPElements[player.UserId].NameHealthESP 存在，則
        ESPElements[player.UserId].NameHealthESP:Destroy()
    結尾
    
    local billboardGui = Instance.new("BillboardGui")
    billboardGui.Name = "NameDistanceHealthESP"
    billboardGui.Adornee = head -- 蝏穃�𡁜��焵摰嗅仍��
    billboardGui.Size = UDim2.new(0, 120, 0, 50) -- 𢒰�踎憭批��
    billboardGui.StudsOffset = Vector3.new(0, 3.5, 0) -- �𢒰�踎�仇宏
    billboardGui.AlwaysOnTop = true -- 遬蝷箏銁��銝𠰴�
    billboardGui.Parent = head
    
    local nameLabel = Instance.new("TextLabel")
    nameLabel.Parent = billboardGui
    nameLabel.BackgroundTransparency = 1 -- 峕艶�𤩺��
    nameLabel.Text = 玩家.Name -- 遬蝷箇焵摰感知�滾��
    nameLabel.Size = UDim2.new(1, 0, 0.33, 0) -- ��𣳇𢒰�踎擃睃漲��1/3
    nameLabel.TextColor3 = Color3.new(1, 1, 1) -- ��滾�烾�𡏭𠧧 蝥舐蒾�𠧧
    nameLabel.TextScaled = true
    nameLabel.Font = Enum.Font.GothamSemibold -- 摮𦯀�� ��刪除�堒𢬢�鴞摮𦯀��
    
    local healthLabel = Instance.new("TextLabel")
    healthLabel.Parent = billboardGui
    healthLabel.BackgroundTransparency = 1 -- 峕艶�𤩺��
    healthLabel.Position = UDim2.new(0, 0, 0.33, 0) -- 雿瀅�𤾸�滾�埈��倌銝𧢲宮
    healthLabel.Size = UDim2.new(1, 0, 0.33, 0) -- ��𣳇𢒰�踎擃睃漲��1/3
    healthLabel.TextColor3 = Color3.new(0, 1, 0) -- 嘥�貝���誯�𡏭𠧧蝏輯𠧧
    healthLabel.TextScaled = true
    healthLabel.Font = Enum.Font.Gotham -- 摮𦯀�橒𡁏蘆�𡁜𢬢�鴞摮𦯀��
    
    local distanceLabel = Instance.new("TextLabel")
    distanceLabel.Parent = billboardGui
    distanceLabel.BackgroundTransparency = 1 -- 峕艶𤩺��
    distanceLabel.Position = UDim2.new(0, 0, 0.66, 0) -- 雿瀅館����𤩺��倌銝𧢲宮
    distanceLabel.Size = UDim2.new(1, 0, 0.33, 0) -- ��𣳇𢒰�踎擃睃漲��1/3
    distanceLabel.TextColor3 = Color3.new(1, 0.5, 0) -- 頝乙憸𡏭𠧧 璈躰𠧧
    distanceLabel.TextScaled = true -- �䌊�𢆡蝻拇指𦆮���𧋦憭批��
    distanceLabel.Font = Enum.Font.Gotham -- 摮𦯀�橒�𡁏蘆�𡁜𢬢�鴞摮𦯀��
    
    local updateConnection = RunService.RenderStepped:Connect(function()
        如果不是 billboardGui.Parent 或不是 LocalPlayer.Character 或不是 player.Character，則
            返回
        結尾
        
        local localRoot = LocalPlayer.Character:FindFirstChild("HumanoidRootPart")
        local targetRoot = player.Character:FindFirstChild("HumanoidRootPart")
        如果 localRoot 和 targetRoot 都成立
            局部距離 = (本地根位置 - 目標根位置).幅度
            distanceLabel.Text = string.format("%.1f蟬�", distance)   
        結尾
        
        local humanoid = player.Character:FindFirstChild("Humanoid")
        如果是類人生物
            本地健康 = math.floor(Humanoid.Health) -- 敶枏�灘����
            local maxHealth = math.floor(humanoid.MaxHealth) -- ��憭扯����
            
            本地健康百分比 = 健康 / 最大健康
            如果 healthPercent > 0.7 則
                healthLabel.TextColor3 = Color3.new(0, 1, 0) -- �亙螢�𠶖��嚗𡁶遛�𠧧
            否則如果健康百分比 > 0.3
                healthLabel.TextColor3 = Color3.new(1, 1, 0) -- 霅血�羓𠶖��嚗𡁻��𠧧
            別的
                healthLabel.TextColor3 = Color3.new(1, 0, 0) -- �暒�埯�𠶖��嚗𡁶滯�𠧧
            結尾
            
            healthLabel.Text = string.format("健康值：%d/%d", health, maxHealth)
        結尾
    結尾）
    
    ESPElements[player.UserId] = ESPElements[player.UserId] 或 {}
    ESPElements[player.UserId].NameHealthESP = billboardGui
    ESPElements[player.UserId].NameHealthUpdateConn = updateConnection
結尾

本地函數 CreateTracerESP(player)
    如果 ESPElements[player.UserId] 和 ESPElements[player.UserId].Tracer 都存在，則
        ESPElements[player.UserId].Tracer:Remove()
    結尾
    
    local tracer = Drawing.new("Line")
    Tracer.Color = Color3.new(1, 0, 0) -- 撠�蝥輸�𡏭嚗𡁻�𦦵滯�𠧧
    Tracer.Thickness = 2 -- 撠�蝥輻射�㛖�嚗�2�仇��
    Tracer.Transparency = 0.8 -- 撠蝥輸�𤩺�𤾸漲嚗�80%嚗��𢠃�𤩺�舉���頣��
    tracer.Visible = false -- ��嘥�钅�鞱��
    
    local renderConnection = RunService.RenderStepped:Connect(function()
        如果不是 ESPConfig.MainSwitch 或不是 ESPConfig.ShowTracer，則
            tracer.Visible = false
            返回
        結尾
        
        local localChar = LocalPlayer.Character
        local targetChar = player.Character
        如果不是 localChar 或不是 targetChar，則
            tracer.Visible = false
            返回
        結尾
        
        local targetRoot = targetChar:FindFirstChild("HumanoidRootPart")
        如果 targetRoot 則
            local screenPos, isVisible = Camera:WorldToViewportPoint(targetRoot.Position)
            如果可見則
                tracer.Visible = true
                tracer.From = Vector2.new(Camera.ViewportSize.X / 2, Camera.ViewportSize.Y / 2)
                tracer.To = Vector2.new(screenPos.X, screenPos.Y)
            別的
                tracer.Visible = false
            結尾
        別的
            tracer.Visible = false
        結尾
    結尾）
    
    ESPElements[player.UserId] = ESPElements[player.UserId] 或 {}
    ESPElements[player.UserId].Tracer = tracer
    ESPElements[player.UserId].TracerConn = renderConnection
結尾

本機函數 UpdatePlayerESP(player)
    如果 player == LocalPlayer 則回傳結束
    
    如果不是玩家角色
        CleanupPlayerESP(player)
        返回
    結尾
    
    如果玩家角色中不存在“頭部”或“人形根部件”，則
        CleanupPlayerESP(player)
        返回
    結尾
    
    如果 ESPConfig.MainSwitch 則
        創建追蹤器ESP(玩家)
        
        如果 ESPConfig.ShowNameDistance 或 ESPConfig.ShowHealth 為真，則
            建立名稱距離健康ESP(玩家)
        別的
            如果 ESPElements[player.UserId] 存在且 ESPElements[player.UserId].NameHealthESP 存在，則
                ESPElements[player.UserId].NameHealthESP:Destroy()
                ESPElements[player.UserId].NameHealthESP = nil
            結尾
            如果 ESPElements[player.UserId] 存在且 ESPElements[player.UserId].NameHealthUpdateConn 存在，則
                ESPElements[player.UserId].NameHealthUpdateConn:Disconnect()
                ESPElements[player.UserId].NameHealthUpdateConn = nil
            結尾
        結尾
    別的
        CleanupPlayerESP(player)
    結尾
結尾

本地函數 UpdateAllESP()
    for _, player in pairs(Players:GetPlayers()) do
        如果玩家不等於本地玩家，則
            UpdatePlayerESP(player)
        結尾
    結尾
結尾

本機函式 HandlePlayerRespawn(player)
    本地角色 = 玩家.角色
    如果不是角色那麼
        角色 = 玩家.角色新增:等待()
    結尾
    
    local head = character:WaitForChild("Head", 5)
    local rootPart = character:WaitForChild("HumanoidRootPart", 5)
    local humanoid = character:WaitForChild("Humanoid", 5)
    
    如果頭部、根部件和人形
        task.wait(0.5)
        UpdatePlayerESP(player)
        task.wait(1)
        UpdatePlayerESP(player)
    結尾
結尾

-- 憭����鰵�焵摰嗅�懲��
Players.PlayerAdded:Connect(function(player)
    如果 player == LocalPlayer 則回傳結束
    
    如果玩家.角色
        task.spawn(HandlePlayerRespawn, player)
    結尾
    
    player.CharacterAdded:Connect(function()
        task.spawn(HandlePlayerRespawn, player)
    結尾）
    
    玩家.角色移除:連結(function()
        CleanupPlayerESP(player)
    結尾）
結尾）

LocalPlayer.CharacterAdded:Connect(function()
    task.wait(1)
    UpdateAllESP()
結尾）

task.spawn(function()
    雖然確實如此
        task.wait(3)
        如果 ESPConfig.MainSwitch 則
            UpdateAllESP()
        結尾
    結尾
結尾）

about:Toggle("�訛��餃���", "ESP_Main", false, function(enabled)
    ESPConfig.MainSwitch = enabled
    UpdateAllESP()
結尾）

about:Toggle("遬蝷箝摰感知�滾��+頝生日氖", "ESP_NameDistance", false, function(enabled)
    ESPConfig.ShowNameDistance = enabled
    UpdateAllESP()
結尾）

about:Toggle("遬蝷箝摰嗉����", "ESP_Health", false, function(啟用)
    ESPConfig.ShowHealth = 已啟用
    UpdateAllESP()
結尾）

about:Toggle("撠蝥輯蕭頦迎���誩�鎣葉敹�嚗�", "ESP_Tracer", false, function(enabled)
    ESPConfig.ShowTracer = enabled
    UpdateAllESP()
結尾）



local TP = UITab5:section("隡𣳇��",false)


TP:Button("隡𣳇���秐銝�瘚�", function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelMain")
結尾）

TP:Button("隡𣳇���秐鈭峕絲", function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelDressrosa")
結尾）

TP:Button("隡𣳇���秐銝㗇絲", function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
結尾）

local TP1 = UITab5:section("鈭峕絲",false)
TP1:Button("隡𣳇���秐憭拼������𡢿", function()
    local Players = game:GetService("Players")
    本地玩家 = Players.LocalPlayer
    local targetPosition = Vector3.new(-287.37, 305.81, 592.98)
    
    如果 player.Character 存在且 player.Character:FindFirstChild("HumanoidRootPart") 則
        player.Character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
        print("撌脖𣳇����鞊芸:", targetPosition)
    結尾
結尾）

TP1:Button("隡𣳇���秐鞊芸�", function()
    local Players = game:GetService("Players")
    本地玩家 = Players.LocalPlayer
    local targetPosition = Vector3.new(2286.93, 15.06, 910.51)
    
    如果 player.Character 存在且 player.Character:FindFirstChild("HumanoidRootPart") 則
        player.Character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
        print("撌脖頸𣳇����憭拼������𡢿:", targetPosition)
    結尾
結尾）

TP1:Button("隡𣳇���秐擛擛潸����", function()
    local Players = game:GetService("Players")
    本地玩家 = Players.LocalPlayer
    local targetPosition = Vector3.new(-6501.06, 83.11, -123.52)
    
    如果 player.Character 存在且 player.Character:FindFirstChild("HumanoidRootPart") 則
        player.Character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
        print("撌脖頸𣳇����擛潸����:", targetPosition)
    結尾
結尾）

TP1:Button("隡𣳇���秐擛擛擛憭�憭�", function()
    local Players = game:GetService("Players")
    本地玩家 = Players.LocalPlayer
    local targetPosition = Vector3.new(922.78, 123.96, 32842.40)
    
    如果 player.Character 存在且 player.Character:FindFirstChild("HumanoidRootPart") 則
        player.Character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
        print("撌脖�𣳇����擛潸�憭�:", targetPosition)
    結尾
結尾）
local TP2 = UITab5:section("銝㗇絲",false)

TP2:Button("隡𣳇���秐瘚瑟�見�𤾸歲", function()
    local Players = game:GetService("Players")
    本地玩家 = Players.LocalPlayer
    local targetPosition = Vector3.new(-12463.60, 376.26, -7566.08)
    
    如果 player.Character 存在且 player.Character:FindFirstChild("HumanoidRootPart") 則
        player.Character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
        print("撌脖�𣳇����瘚瑟�見�𤾸歲:", targetPosition)
    結尾
結尾）

TP2:Button("隡𣳇���秐瘚琿�蠘不敢摰�", function()
    local Players = game:GetService("Players")
    本地玩家 = Players.LocalPlayer
    local targetPosition = Vector3.new(-5060.41, 316.43, -3192.30)
    
    如果 player.Character 存在且 player.Character:FindFirstChild("HumanoidRootPart") 則
        player.Character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
        print("撌脖�𣳇����瘚琿�謔害怕摰�:", targetPosition)
    結尾
結尾）

TP2:Button("隡𣳇���秐�虯瘜�", function()
    local Players = game:GetService("Players")
    本地玩家 = Players.LocalPlayer
    local targetPosition = Vector3.new(-5096.48, 316.43, -3177.91)
    
    如果 player.Character 存在且 player.Character:FindFirstChild("HumanoidRootPart") 則
        player.Character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
        print("撌脖�𣳇�����虯瘜�:", targetPosition)
    結尾
結尾）

TP2:Button("隡𣳇���秐銋嘥仍���", function()
    local Players = game:GetService("Players")
    本地玩家 = Players.LocalPlayer
    local targetPosition = Vector3.new(-5027.03, 316.43, -3206.07)
    
    如果 player.Character 存在且 player.Character:FindFirstChild("HumanoidRootPart") 則
        player.Character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
        print("撌脖�𣳇����銋嘥仍���:", targetPosition)
    結尾
結尾）




task.spawn(function()
    task.wait(2)
    UpdateAllESP()
結尾）

game:GetService("StarterGui"):SetCore("SendNotification",{
	Title = "鈭箸𣱣鈭箄�𡁏𧋦",
	Text = "��㰘蝸摰峕��蟡心血管其另一頭�鍂�匧翰",
	持續時間 = 5；
})
