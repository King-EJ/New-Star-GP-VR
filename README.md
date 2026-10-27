# New-Star-GP-VR
VR Mod for New Star GP "broken for test play"


NEW STAR GP VR11 - Fixed cockpit / Quest driving key mapping

Changes from VR10:
- Fixed cockpit position relative to PlayerCarTemplate: local (0,0.38,-0.45) meters.
  No longer captures chase camera position, which could put player in front of car or sky.
- Reset Seat in headset settings clears user seat offsets and uses fixed baseline.
- Quest driving now defaults to WASD keys; selectable WASD / ARROWS in settings.
  Right trigger W/up = accelerate, left trigger S/down = brake/reverse.
  Left stick A/D or left/right arrows = steer.
- VR10 debug-canvas cleanup and left thumbstick-click settings preserved.
- Xbox gamepad code unchanged.

TEST: Enable QUEST KEYBOARD DRIVING in headset settings. Try WASD first,
then ARROWS if game uses arrow bindings. If neither works, the game likely
uses Rewired or gamepad-only driving and will need native input injection.

BUILD: Run BUILD.bat on Windows with .NET SDK installed. Copy resulting
NSGPVR.dll into BepInEx/plugins, replacing previous version.
OpenXR.dll remains required from existing installation.

NOTE: This build is source-only, not compiled/tested in-game here.
