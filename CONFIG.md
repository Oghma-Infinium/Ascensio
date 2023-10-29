![](https://raw.githubusercontent.com/Oghma-Infinium/Ascensio/main/Media/Ascensio%20Header.png)

<p align="center">
  [ <a href="https://www.nexusmods.com/skyrimspecialedition/mods/89138">Nexus Page</a> | <a href="https://github.com/Oghma-Infinium/Ascensio/blob/main/README.md">Installation</a> |
  <a href="https://github.com/Oghma-Infinium/Ascensio/blob/main/CHANGELOG.md">Changelog</a> |
  <a href="https://github.com/Oghma-Infinium/Ascensio/main/CONFIG.md">Configuration</a> |
  <a href="https://github.com/Oghma-Infinium/Ascensio/main/FAQ.md">FAQ</a> |
  <a href="https://loadorderlibrary.com/lists/ascensio-1">Load Order</a> |
  <a href="https://discord.gg/WakingDreams"> Modlist Discord</a> ]
</p>

---

# Optional Addons

The following sections detail the **supported** modifications to the list at bottom of MO2's left pane. Any other modifications should be discussed in the `#🌟│ascensio-modifications` channel of the [Waking Dreams](https://discord.gg/wakingdreams) discord server.

Please note that if you do any of these tweaks, it is in your best interest to share this information when reporting any potential bugs that you encounter when playing the modlist.

## ENB Profiles
After launching MO2, you have a choice of playing the game with either [NAT ENB](https://www.nexusmods.com/skyrimspecialedition/mods/27141) or [Rudy ENB (Zangdar's Edit)](https://www.nexusmods.com/skyrimspecialedition/mods/39113) for Cathedral Weathers. Use the `Profiles` drop down box at the top of MO2 to pick your preferred ENB profile.

## Performance Mode

This section will cover the `Performance Mode` section of the modlist. If you find yourself struggling with running the list, various mods such as performance LOD outputs, tweaked grass settings to reduce grass density, and edited ENB presets (for your chosen ENB profile) have been provided for you to switch on.
  >**DO NOT** switch on the Performance LOD Outputs *mid-save*. I cannot guarantee that you will face zero visual bugs from doing so.

In order to use these Performance tweaks, activate the mods you wish to use under the `Performance Mode` separator. These mods should consist of:
 - `Ascensio - Performance DynDOLOD Output`
 - `Rudy ENB CW - Zangdar's Edit Performance Edits`
 - `NAT.ENB - ENB PRESET Performance Edits`
 - `Performance Grass INI`

## Insects Begone

For those with arachnophobia and/or entomophobia, the `Insects Begone` separator contains a couple of mods to remove most of the spider and insect adjacent meshes and enemies from the list. Some aspects of the list's vision are compromised to support these tweaks.

Tick these mods on if you wish to utilize them:
- `Ascensio - Insects Begone`
- `Insects Begone - Modularly Removing Spiders and Chaurus`

## Ultrawide Patches

At the bottom of the left pane in MO2, there is an `Ultrawide Patches` separator you can expand. Here you can enable the respective widescreen fixes for your monitor if needed.
  > I do not own an ultrawide monitor, so no testing has been done with these unfortunately. Please let me know if any of these patches need to be changed in some way to accommodate ultrawide users.

These mods should consist of:
- `Race Menu SE - Widescreen Fix`
- `The Elder Scrolls Legends - Loading Screens - 21x9 Fix by Stormhand`
- `Dear Diary Dark Mode (Ultrawide Fix for 21x9)`
- `Dear Diary Dark Mode (Ultrawide Fix for 32x9)`

## Changing Resolution

By default, Wabbajack will set the resolution in your `SkyrimPrefs.ini` to match the native resolution of your monitor. However, Skyrim scales very poorly at resolutions above 1080p (`1920x1080`) and depending on your hardware, it might be difficult to achieve consistent FPS on higher resolutions.

If you wish to change your resolution, the preferred way is to find the `SSEDisplayTweaks.ini` located within the `SSE Display Tweaks` mod with these steps:
1. Open the INI
2. Navigate to line 66 where `#Resolution=1920x1080` is
3. Change to your desired resolution

After changing the resolution line, remove the `#` in order for the settings to take affect when launching the game.

Example for how the .ini line should look:
- **Before:** `#Resolution=1920x1080`  
- **After:** `Resolution=2560x1440`

## Skyrim Upscaler

While [Skyrim Upscaler](https://www.nexusmods.com/skyrimspecialedition/mods/80343) is an unsupported addition, I figured I'd mention it here due to the questions we receive about it on the Waking Dreams server. I've set up the `SSEDisplayTweaks.ini` inside the `SSE Display Tweaks` mod to automatically accommodate PureDark's Patreon DLSS mod in case users wish to use it. 

If for whatever reason your Display Tweaks settings have been reset, below I have included the lines you must change in order to make sure your Upscaler works.

In the `SSEDisplayTweaks.ini`, edit these lines 
- Line 39: `Fullscreen = false`
- Line 48: `Borderless = true`
- Line 58: `BorderlessUpscale = false`

## In-Game MCM options

Your MCMs will come pre-configured for you and there are not many to begin with due to the focus of this modlist, but below I have explained what each MCM is for and if you can safely edit them.

 - **LOD Reload Bug Fix**: Tick on **one** of the options under the `Options` section if you find yourself experiencing this bug pretty often.
 - **MCM Recorder**: This MCM is for recording your MCM options for you. I don't recommend touching this unless you explicity know what to do with it.
 - **Mists of Tamriel**: Here you can change any settings with Mists of Tamriel if you'd like. I don't recommend switching on the `Medium` or `Dense` options since those cause seams with the fog.
 - **Photo Mode**: Feel free to mess with the keybinds and settings for po3's Photo Mode. I don't recommend turning on the `Compress Textures` option since it seem to cause crashes when screenshotting.
 - **Quest Journal Limit Bug Fixer**: Click the `Start` option under this MCM if you need to fix your Quest Journal
 - **Sky UI**: Font Size is set to `Medium` by default, but you can change different UI elements here
 - **True Directional Movement**: This MCM was left with the default settings mostly, but you can change TDM settings here
 - **Ultimate Immersion Toggle**: Handles what key hides the UI. This is set to X by default.

## BethINI

If you wish to rerun BethINI, please make sure that you close MO2 beforehand and that your paths are correctly set within the `Setup` tab of the program, like so:

 - **Game**: `Skyrim Special Edition`
 - **Game Path**: `[Path to Modlist]\Stock Game`
   > example: `F:\Ascensio\Stock Game`
 - **Mod Organizer**: `[Path to Modlist]\ModOrganizer.exe` 
   > example: `F:\Ascensio\ModOrganizer.exe`
 - **INI Path**: `Mod Organizer > Ascensio - NAT ENB` or `Mod Organizer > Ascensio - CW Rudy ENB`

To squeeze out some more FPS, tweak the following value in the `Detail` tab within BethINI.

- `Shadow Resolution`: 1024
- `Ambient Occlusion`: Either use this version within BethINI or the ENB version. The ENB version is more intensive. **Do not have both turned on.**
- `Remove Shadows`: I really don’t recommend turning this on, but if you must, then you can.

