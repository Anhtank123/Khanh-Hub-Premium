-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local Login = Instance.new("Frame")
local Submit = Instance.new("TextButton")
local Pass = Instance.new("TextBox")
local loadingscript = Instance.new("TextLabel")
local loading = Instance.new("Frame")
local text1 = Instance.new("TextLabel")
local text2 = Instance.new("TextLabel")
local text = Instance.new("TextLabel")
local text4 = Instance.new("TextLabel")
local text3 = Instance.new("TextLabel")
local main = Instance.new("Frame")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Login.Name = "Login"
Login.Parent = ScreenGui
Login.BackgroundColor3 = Color3.fromRGB(13, 13, 13)
Login.Position = UDim2.new(0.367362142, 0, 0.358282208, 0)
Login.Size = UDim2.new(0, 356, 0, 190)

Submit.Name = "Submit"
Submit.Parent = Login
Submit.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Submit.BorderColor3 = Color3.fromRGB(0, 255, 255)
Submit.Position = UDim2.new(0.334269673, 0, 0.699999988, 0)
Submit.Size = UDim2.new(0, 117, 0, 30)
Submit.Font = Enum.Font.SourceSans
Submit.Text = "Submit"
Submit.TextColor3 = Color3.fromRGB(0, 255, 255)
Submit.TextSize = 14.000
Submit.MouseButton1Down:Connect(function()
	if Pass.Text == "key" then
		Login.Visible = false
		loading.Visible = true
		text.Visible = true
		wait(1)
		text.Visible = false
		text1.Visible = true
		wait(1)
		text1.Visible = false
		text2.Visible = true
		wait(1)
		loading.Visible = false
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Anhtank123/Khanh-Hub-Paid/main/README.md"))()
	elseif
		wait(0.7)
	then  Login.Visible = false
		loading.Visible = true
		text.Visible = true
		wait(1)
		text3.Visible = true
		wait(1)
		loading.Visible = false
		game:GetService("Players").LocalPlayer:Kick("Incorrect Key.. Please Try Again")
	end 
end)

Pass.Name = "Pass"
Pass.Parent = Login
Pass.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Pass.BorderColor3 = Color3.fromRGB(0, 255, 255)
Pass.Position = UDim2.new(0.219101191, 0, 0.368421078, 0)
Pass.Size = UDim2.new(0, 200, 0, 50)
Pass.Font = Enum.Font.SourceSans
Pass.Text = "Enter Keys"
Pass.TextColor3 = Color3.fromRGB(0, 255, 255)
Pass.TextSize = 14.000

loadingscript.Name = "loading script"
loadingscript.Parent = Login
loadingscript.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
loadingscript.BorderColor3 = Color3.fromRGB(0, 255, 255)
loadingscript.Size = UDim2.new(0, 356, 0, 31)
loadingscript.Font = Enum.Font.SourceSans
loadingscript.Text = "Login To Scripts"
loadingscript.TextColor3 = Color3.fromRGB(0, 255, 255)
loadingscript.TextSize = 14.000

loading.Name = "loading"
loading.Parent = ScreenGui
loading.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
loading.Position = UDim2.new(0.391952306, 0, 0.422085911, 0)
loading.Size = UDim2.new(0, 288, 0, 100)
loading.Visible = false

text1.Name = "text1"
text1.Parent = loading
text1.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
text1.Position = UDim2.new(0.15625, 0, 0.25, 0)
text1.Size = UDim2.new(0, 200, 0, 50)
text1.Visible = false
text1.Font = Enum.Font.SourceSans
text1.Text = "Checking Key ...."
text1.TextColor3 = Color3.fromRGB(0, 255, 255)
text1.TextSize = 14.000

text2.Name = "text2"
text2.Parent = loading
text2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
text2.Position = UDim2.new(0.15625, 0, 0.25, 0)
text2.Size = UDim2.new(0, 200, 0, 50)
text2.Visible = false
text2.Font = Enum.Font.SourceSans
text2.Text = "Success"
text2.TextColor3 = Color3.fromRGB(0, 255, 255)
text2.TextSize = 14.000

text.Name = "text"
text.Parent = loading
text.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
text.Position = UDim2.new(0.15625, 0, 0.25, 0)
text.Size = UDim2.new(0, 200, 0, 50)
text.Visible = false
text.Font = Enum.Font.SourceSans
text.Text = "Checking Key ."
text.TextColor3 = Color3.fromRGB(0, 255, 255)
text.TextSize = 14.000

text4.Name = "text4"
text4.Parent = loading
text4.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
text4.Position = UDim2.new(0.15625, 0, 0.25, 0)
text4.Size = UDim2.new(0, 200, 0, 50)
text4.Visible = false
text4.Font = Enum.Font.SourceSans
text4.Text = "Incorrect Key.."
text4.TextColor3 = Color3.fromRGB(0, 255, 255)
text4.TextSize = 14.000

text3.Name = "text3"
text3.Parent = loading
text3.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
text3.Position = UDim2.new(0.15625, 0, 0.25, 0)
text3.Size = UDim2.new(0, 200, 0, 50)
text3.Visible = false
text3.Font = Enum.Font.SourceSans
text3.Text = "Checking Key ...."
text3.TextColor3 = Color3.fromRGB(0, 255, 255)
text3.TextSize = 14.000

main.Name = "main"
main.Parent = ScreenGui
main.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
main.Position = UDim2.new(0.1068376, 0, 0.0547169819, 0)
main.Size = UDim2.new(0, 100, 0, 100)
main.Visible = false

-- Scripts:

local function OBBZHSI_fake_script() -- Login.LocalScript 
	local script = Instance.new('LocalScript', Login)

	local UIS = game:GetService('UserInputService')
	
	local frame = script.Parent
	
	
	
	local dragToggle = nil
	
	local dragSpeed = 0.25
	
	local dragStart = nil
	
	local startPos = nil
	
	
	
	local function updateInput(input)
	
		local delta = input.Position - dragStart
	
		local position = UDim2.new(startPos.X.Scale, startPos.X.Offset + delta.X,
	
			startPos.Y.Scale, startPos.Y.Offset + delta.Y)
	
		game:GetService('TweenService'):Create(frame, TweenInfo.new(dragSpeed), {Position = position}):Play()
	
	end
	
	
	
	frame.InputBegan:Connect(function(input)
	
		if (input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch) then 
	
			dragToggle = true
	
			dragStart = input.Position
	
			startPos = frame.Position
	
			input.Changed:Connect(function()
	
				if input.UserInputState == Enum.UserInputState.End then
	
					dragToggle = false
	
				end
	
			end)
	
		end
	
	end)
	
	
	
	UIS.InputChanged:Connect(function(input)
	
		if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
	
			if dragToggle then
	
				updateInput(input)
	
			end
	
		end
	
	end)
	
	
end
coroutine.wrap(OBBZHSI_fake_script)()
