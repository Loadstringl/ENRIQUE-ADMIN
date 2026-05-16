-- ENRIQUE ADMIN - 彻底清理版

local original = game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source")

local customized = original

-- 彻底清理版本和旧名字
customized = customized:gsub("Infinite Yield", "ENRIQUE ADMIN")
customized = customized:gsub("InfiniteYield", "ENRIQUE ADMIN")
customized = customized:gsub("IY", "ENRIQUE")
customized = customized:gsub("v6%.4%.1", "")
customized = customized:gsub("FE v6%.4%.1", "")
customized = customized:gsub("FE", "")
customized = customized:gsub("EdgeIY", "ENRIQUE")
customized = customized:gsub("6%.4%.1", "")
customized = customized:gsub("v6", "")

-- 改变颜色
customized = customized:gsub("255, 255, 255", "0, 255, 200")
customized = customized:gsub("0, 170, 255", "0, 255, 180")
customized = customized:gsub("170, 0, 170", "0, 200, 255")

loadstring(customized)()

game:GetService("StarterGui"):SetCore("SendNotification", {
    Title = "ENRIQUE ADMIN",
    Text = "加载成功",
    Duration = 8
})

print("ENRIQUE ADMIN 已加载")
