# Change log

All notable changes to this project will be documented in this file.

## 1.1.0

Key feature of this version is sound effects improvement, game should sound closer to the vanilla DOS version now. 

All detailed information about 1.1 release can be found here https://github.com/notsure8x/e2140-unofficial-patch/milestone/1

### Fixed
- Heavy Lifters, WTP100, helicopters, HAT transporters sound effect is played either too often or doesn't stop if the unit landed, stopped moving or was destroyed
- Explosion, weapon fire, UCS mech units walking sound effects are partially missing, especially during battles
- Sometimes keyboard hotkeys doesn't work for unit commands, like stopping unit with 's' key
- Restored 'm' hotkey functionality to the vanilla version - switching between mines/walls for miner units. You can no longer use 'm' key as shortcut for moving units.
- Two bug fixes related to the AI that should result in less/no glitching of AI with inifite unit production

### Improvements
- ALT+F4 and close window button are now working correctly in main menu and game screens (except unit/building database view and during playing cutscenes)

## 1.0.0-alpha

Works only with Earth 2140 Trilogy published on GOG platform!
This version's primary purpose is to get community feedback regarding patch installation. Main concern is Windows administration rights requirement and anti-virus software interactions. From gameplay standpoint, almost all AI issues are resolved, however AI player sometimes can stuck in producing infinite number of TUR/HAT units.

### Fixed
- AI players are not producing any units in their construction centers and factories (unless they are hit and repaired!)
- Virtual generals are not working
- Minelaying units do not lay mines
- Game crashes when KT30 attacks enemy building
- Game wipes out AI-related data when loaded from "save game"
- Building windows get transparent instead of black when power is turn off
- Tracked units tracks are transparent instead of black