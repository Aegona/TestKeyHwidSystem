local Data = {
    ["GSD-1FK4-JCSPE-SCRIPT"] = "054F6F9D-06F6-4ECC-91B0-11747437461E", 
    ["Another-Key"] = "Another-Hwid" 
}

if Data[_G.Key] and Data[_G.Key] == _G.hwid then
if game:GetService("RbxAnalyticsService"):GetClientId() == _G.hwid then
	    print("ยินดีต้อนรับ ครับ! ✅")
	game:GetService("StarterGui"):SetCore("SendNotification",{
	Title = "AEGONA HUB", 
	Text = "ยินดีต้อนรับ ครับ! ✅", 
	Icon = "rbxassetid://1000000" 
})
else
		game:GetService("StarterGui"):SetCore("SendNotification",{
	Title = "AEGONA HUB", 
	Text = "Not Found HWID ~ หรือ Reset Hwid 🚫", 
	Icon = "rbxassetid://1000000" 
})
end
elseif not Data[_G.Key] then
	game:GetService("StarterGui"):SetCore("SendNotification",{
	Title = "AEGONA HUB", 
	Text = "กรุณา ซื้อ Key ได้ที่เว็ปไซน์ AEGONASTORE.COM", 
	Icon = "rbxassetid://1000000" 
})

else
    warn("Error 🚫 ")
		game:GetService("StarterGui"):SetCore("SendNotification",{
	Title = "AEGONA HUB", 
	Text = "Wrong Hwid or Wrong Key🚫", 
	Icon = "rbxassetid://1000000" 
})
end
