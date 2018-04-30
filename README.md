As of 30.04.2018

net module

export.lua files

typical ways of extracting data
	udp socket

LockOn

LuaExportStart
LuaExportStop
LuaExportBeforeNextFrame
LuaExportAfterNextFrame
LuaExportActivityNextEvent

--Prev Export functions.
chain export functions
local PrevExport = {}
PrevExport.LuaExportStart = LuaExportStart
PrevExport.LuaExportStop = LuaExportStop
PrevExport.LuaExportBeforeNextFrame = LuaExportBeforeNextFrame
PrevExport.LuaExportAfterNextFrame = LuaExportAfterNextFrame

	-- Chain previously-included export as necessary
	if PrevExport.LuaExportStart then
		PrevExport.LuaExportStart()
	end

LoGetModelTime() -- returns current model time (args - 0, results - 1 (sec))
LoGetMissionStartTime() -- returns mission start time (args - 0, results - 1 (sec))
LoGetPilotName() -- (args - 0, results - 1 (text string))
LoGetIndicatedAirSpeed() -- (args - 0, results - 1 (knots))
LoGetTrueAirSpeed() -- (args - 0, results - 1 (knots))
LoGetAltitudeAboveSeaLevel() -- (args - 0, results - 1 (feet))
LoGetAltitudeAboveGroundLevel() -- (args - 0, results - 1 (feet))
LoGetAngleOfAttack() -- (args - 0, results - 1 (degrees))
LoGetAccelerationUnits() -- (args - 0, results - 1 (G))
LoGetVerticalVelocity() -- (args - 0, results - 1(feet per sec))
LoGetADIPitchBankYaw() -- (args - 0, results - 3 (degrees))
LoGetMCPState() -- (args - 0, results - 1 (table of key(string).value(boolean))



LoGetWorldObjects()
LoSetCommand()

LoCreateCoroutineActivity()
https://www.lockon.ru/en/dev_journal/lua-export/



https://forums.eagle.ru/showthread.php?t=146924&page=2

mission lua environment
server lua environment

local terrain = require('terrain')

hook is run every 0.1 seconds?


