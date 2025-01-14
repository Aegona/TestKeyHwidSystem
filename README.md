local Data = {
    ["GSD-1FK4-JCSPE-SCRIPT"] = "054F6F9D-06F6-4ECC-91B0-11747437461E", 
    ["Another-Key"] = "Another-Hwid" 
}

if Data[_G.Key] and Data[_G.Key] == _G.hwid then
    print("ยินดีต้อนรับ ครับ! ✅")
	game:GetService("StarterGui"):SetCore("SendNotification",{
	Title = "AEGONA HUB", 
	Text = "ยินดีต้อนรับ ครับ! ✅", 
	Icon = "rbxassetid://1000000" 
})
else
    warn("กรุณา ซื้อ Key ได้ที่เว็ปไซน์ AEGONASTORE.COM หรือ Reset Hwid 🚫 ")
		game:GetService("StarterGui"):SetCore("SendNotification",{
	Title = "AEGONA HUB", 
	Text = "กรุณา ซื้อ Key ได้ที่เว็ปไซน์ AEGONASTORE.COM หรือ Reset Hwid 🚫", 
	Icon = "rbxassetid://1000000" 
})
end
