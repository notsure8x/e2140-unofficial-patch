# E2140 Unofficial Patch

## Intro
I made this patch to fix issues found in the Windows version of both **Earth 2140 Trilogy** (GOG) and **Earth 2140 HD** (Steam), which aren't present in the original DOS version of the game. Both  releases have many issues including an almost completely passive enemy AI player, non-working "virtual generals" feature, broken sound and many others. 

Further versions of this patch may introduce improvements beyond the original game content, however those will be focused on possible AI improvements rather than graphics or UI improvements. 

For a modern remake of Earth 2140, please check out and support [OpenE2140](https://github.com/OpenE2140/OpenE2140) project that is currently in development by another team!

**Newest version of the patch is 1.3.0.**

## Patch compatibility
E2140 Unofficial Patch is compatible with Earth 2140 Trilogy released on GOG platform (https://www.gog.com/en/game/earth_2140_trilogy) and Earth 2140 HD released on Steam (https://store.steampowered.com/app/253860/Earth_2140/). Patch will not work with any other releases eg. Classic XP and others.

## Getting started

Please refer to [Troubleshooting](##Troubleshooting) in case of administrator rights issues or anti-virus warnings.

**Earth 2140 Trilogy (GOG)**
1. Download the latest patch [release](https://github.com/notsure8x/e2140-unofficial-patch/releases).
2. Extract the archive and/or copy all files (e2140-patch-installer.exe + e2140-unofficial-patch.dll) to Earth 2140 Trilogy installation directory (like "C:/GOG Games/Earth 2140").
3. Run **e2140-patch-installer.exe** inside Earth 2140 Trilogy directory. You should be notified that patching was either successful or failed. SKIP THIS STEP IF YOU ARE ALREADY HAVE PREVIOUS PATCH INSTALLED, JUST OVERWRITE PREVIOUS e2140-unofficial-patch.dll FILE AND GO TO STEP 3.
4. Run the game from the GOG Galaxy client or the desktop shortcut, if you have one. Enjoy AI swarming your base in waves!

**Earth 2140 HD (Steam)**
1. Download the latest patch [release](https://github.com/notsure8x/e2140-unofficial-patch/releases).
2. Extract the zip archive and/or copy all files (e2140-patch-installer.exe + e2140-unofficial-patch.dll + SDL.dll + SDL_mixer.dll) to Earth 2140 HD installation directory (like "C:/Steam/steamapps/common/Earth 2140"). 

If your Steam game installation directory is non-standard, open Steam client, select Earth 2140 HD in your library, right click on it, open Manage menu. From Manage menu, click on "Browse Local Files". This should open game installation directory and this is where you need to put the patch files.

3. Run e2140-patch-installer.exe inside Earth 2140 HD directory. You should be notified that patching was either successful or failed. SKIP THIS STEP IF YOU ALREADY HAVE PREVIOUS PATCH INSTALLED, JUST OVERWRITE PREVIOUS e2140-unofficial-patch.dll FILE AND GO TO STEP 3.

4. Run the game from the Steam client or the desktop shortcut, if you have one. Enjoy AI swarming your base in waves!

**NOTE 1:** Old save games will not work. You either need to load your save game and restart the mission or play the campaign from the beginning.

**NOTE 2:** The patch installer creates a backup of the original game executable, running the patch installer a second time will ask the user to restore the original executable.

**NOTE 3:** Save games are not compatible between Earth 2140 Trilogy (GOG) and Earth 2140 HD (Steam) releases.

## Troubleshooting
As with many other unofficial patches, the E2140 Unofficial Patch is using process execution manipulation techniques that can be considered as harmful by anti-virus software. When running **e2140-patch-installer.exe** or the modified game executable, anti-virus software may qualify them as a false positive malware/virus/trojan. AV software might quarantine or delete both the patch installer and/or the game executable E2140.exe. In case your E2140.exe file was deleted, you can restore it using GOG Galaxy using "Manage installation -> Verify/Repair" function or Steam client "Check file integrity" feature.

Before releasing the package, all files are checked with the [VirusTotal](https://www.virustotal.com) online scanning service.

## Bug reports, feature requests
1. Go to the project's GitHub [issues](https://github.com/notsure8x/e2140-unofficial-patch/issues) and check if a similar bug has not been already reported.
2. Open an issue (New issue), describe the bug, describe your OS version and basic HW specification. Attach a savegame.
3. You can also visit discord channels to look for support from @noture_8x and other community members
- [InsideEarth Discord channel #e2140-unofficial-patch](https://discord.com/channels/572336961143177216/1179834300414296124)
- [OpenE2140 Discord channel   #earth-unofficial-patch](https://discord.com/channels/1080437044884553799/1155957226100498462) 

## Bugs status

Check [Changelog](./CHANGELOG.md) for detailed information about patch versions.

**Fixed in both GOG and Steam versions**
- **[FIXED]** AI players are not producing any units in their construction centers and factories
- **[FIXED]** Virtual generals are not working
- **[FIXED]** Minelaying units do not lay mines (MP2, UCS, The New Outpost,M01)
- **[FIXED]** Game crashes when KT30 attacks enemy building
- **[FIXED]** Game wipes out AI-related data when loaded from "save game"
- **[FIXED]** Building's windows are transparent instead of black when power is turned off - reported by michaeldgg2 :)
- **[FIXED]** Tracked units tracks are transparent instead of black
- **[FIXED]** Ocasionally, AI player stucks producing an abnormal amount of HAT, TUR or BTTI units.
- **[FIXED]** Buggy and missing sound effects for weapons and explosions especially in battles. Buggy sound effects for Heavy Lifter, WTP100, helicopters, HAT.
- **[FIXED]** Unit keyboard hotkeys (like 's' to stop) sometimes doesn't work

**Only GOG 1.0 version (not HD)**
- **[IMPROVED]** Mouse lock/unlock support when game is run in windowed mode (for streaming)
- **[IMPROVED]** ALT+F4 & close window button are now almost working correctly (except database view and when playing cutscenes)

## Special thanks
Big thanks to the Animal from InsideEarth community for helping with connecting with its members.

Special thanks to michaeldgg2 and IceReaper from OpenE2140 development team for long discussions about not very known quirks, bugs and features of the original Earth 2140 game! 

## Third party libraries

E2140 Unofficial Patch uses Microsoft [Detours](https://www.microsoft.com/en-us/research/project/detours/) and [Boost](https://www.boost.org/) third party software libraries.
Please refer to [NOTICE.txt](./NOTICE.txt) file for their copyrights and license information.

## Disclaimer

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
