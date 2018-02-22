Problem Areas

--[[--Clock--]]--
--[[--defineRotary("CLOCK_SET", 4, 3801, 135, "Clock", "Clock Setting")
definePushButton("STOPWATCH", 4, 3802, 0, "Clock", "Stopwatch Start/Stop")--]]--

--[[--Airbrake--]]--
--[[--Airbrake (device 12?) does not appear to be modeled in cockpit--]]--

--[[--definePotentiometer("MAINT_TEST_MODE", 18, 3913, 675, {0, 1}, "Engine Panel", "Maintenance Testing Mode")--]]--
elements["PNT_675"] = default_axis_limited(_("Maintenance Testing Mode"),devices.ENGINEPANEL, 3913, 675, 0.001, false, false, 1)

--[[--definePotentiometer("DRYSUIT_VENT_ADJUST", 18, 3917, 396, {0, 1}, "Engine Panel", "Drysuit Ventilation Adjustment")--]]--

--[[--Cabin Air Valve does not appear to be functional in cockpit--]]--

--[[--Missile Select Button does not appear to be functional in cockpit--]]--

--[[Radio volume control appears to be broken in Viggen.  Key commands work, but virtual knob does not.
definePotentiometer("RADIO_VOLUME", 18, 3112, 385, {0, 1}, "Engine Panel", "Radio Volume")--]]--

--[[Windscreen de-ice knob appears to be broken in Viggen.  Odd behavior in-cockpit.
definePotentiometer("WINDSCREEN_DEICE", 18, 3912, 286, {0, 0.9}, "Engine Panel", "Windscreen De-Ice")--]]--

--[[--IFF Code not functional in cockpit--]]--

--[[--definePotentiometer("RADAR_BRIGHTNESS", 5, 3923, 391, {0, 1}, "Radar", "Radar Brightness")--]]--

--[[--definePotentiometer("ALTIMETER_SETTING", 22, 3306, 0, {0, 1}, "Flight Data Unit", "Altimeter Setting")
Missing argument number.  Shows as 0 now.--]]--

--[[--definePotentiometer("AUTOPILOT_YAW_TRIM", 22, 3732, 211, {0, 1}, "Flight Data Unit", "Autopilot Yaw Trim")--]]--

--[[--definePushButton("BACKUP_ADI_CAGE", 22, 3720, 123, "Flight Data Unit", "Backup ADI Cage")--]]--
elements["PNT_123"] = default_button(_("Backup ADI Cage"), devices.FLIGHTDATAUNIT, 3720, -666)

--[[--definePotentiometer("HUD_BRIGHTNESS", 22, 3409, 180, {0, 1}, "Flight Data Unit", "HUD Brightness Knob")--]]--

--[[--definePushButton("MAX_G_RESET", 22, 3722, 175, "Flight Data Unit", "Max G Reset")
Button does not appear to work in cockpit.--]]--
elements["PNT_175"] = default_button(_("Max G Reset"), devices.FLIGHTDATAUNIT, 3722, -666)

--[[--definePushButton("ROLL_CENTERING", 22, 3305, 212, "Flight Data Unit", "Roll Centering")--]]--

--[[--definePushButton("SNABBRESNING", 22, 3091, 0, "Flight Data Unit", "Snabbresning")--]]--

--[[--definePotentiometer("MAG_DEC_ADJUST", 22, 3915, 1201, {-1, 1}, "Flight Data Unit", "Magnetic Declination Adjustment")
Knob does not work in cockpit.--]]--
elements["PNT_1201"] = default_axis_limited(_("Magnetic Declination Adjustment"),devices.ENGINEPANEL, 3915, 1201, 0.001, false, false, 1)
3714

{combos = {{key = "C", reformers = {"LAlt","LCtrl"}}}, down = 3314, cockpit_device_id = devices.WEAPON_SYSTEM, value_down = 1.0, name = _("IR-missile uncage"), category = _("Weapons")},
{combos = {{key = "S", reformers = {"LAlt","LCtrl"}}}, down = 3311, cockpit_device_id = devices.WEAPON_SYSTEM, value_down = 1.0, name = _("IR-missile fast select"), category = _("Weapons")},

defineFloat("OXYGEN_PRESSURE", 54, {0, 1}, "Raw Gauge Values", "Oxygen Pressure") --[[--Argument number is best guess--]]--
Can't find oxygen pressure gauge in lua files.  54 does not appear to work.  Found reference to 54 in assoication with oxygen.
Does not appear to be modelled in cockpit.

{combos = {{key = "R", reformers = {"LAlt","LCtrl"}}}, down = 3005, value_down = 0.1, cockpit_device_id = devices.RWR, name = _('Master Volume / Sidewinder Tone Up'), category = _('Countermeasures')},
{combos = {{key = "R", reformers = {"LAlt","RAlt"}}},down = 3005, value_down = -0.1, cockpit_device_id = devices.RWR, name = _('Master Volume / Sidewinder Tone Down'), category = _('Countermeasures')},

Mach meter calculation in lua file.
Thanks,
