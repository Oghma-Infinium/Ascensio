![](https://raw.githubusercontent.com/Oghma-Infinium/Ascensio/main/Media/Ascensio%20Header.png)

<p align="center">
  [ <a href="https://www.nexusmods.com/skyrimspecialedition/mods/89138">Nexus Page</a> | <a href="https://github.com/Oghma-Infinium/Ascensio/blob/main/README.md">Installation</a> |
  <a href="https://github.com/Oghma-Infinium/Ascensio/blob/main/CHANGELOG.md">Changelog</a> |
  <a href="https://github.com/Oghma-Infinium/Ascensio/blob/main/CONFIG.md">Configuration</a> |
  <a href="https://github.com/Oghma-Infinium/Ascensio/blob/main/FAQ.md">FAQ</a> |
  <a href="https://loadorderlibrary.com/lists/ascensio-1">Load Order</a> |
  <a href="https://discord.gg/WakingDreams"> Modlist Discord</a> ]
</p>

---

**Modlist Support: [Waking Dreams](https://discord.gg/WakingDreams)**

- [Introduction](#introduction)
  - [System Requirements](#system-requirements)
- [Installation](#installation)
  - [Pre-Installation](#pre-installation)
    - [Pagefile and crash prevention](#pagefile-and-crash-prevention)
    - [Setting Shader Cache Size](#setting-shader-cache-size)
    - [Steam Setup](#steam-setup)
    - [Game Language](#game-language)
  - [Wabbajack Installation](#wabbajack-installation)
    - [Installing Wabbajack](#installing-wabbajack)
    - [Downloading and Installing Ascensio](#downloading-and-installing-ascensio)
  - [Problems with installation](#problems-with-installation)
- [Post-Installation and Optional Setup](#post-installation-and-optional-setup)
  - [Game Folder](#game-folder)
  - [Antivirus Exceptions](#antivirus-exceptions)
- [Playing the List](#playing-the-list)
  - [Starting the Game](#starting-the-game)
- [Updating the modlist](#updating-the-modlist)
- [Removing the Modlist](#removing-the-modlist)
- [Contact](#contact)
- [Credits and Thanks](#credits-and-thanks)


---

## Introduction

Ascensio is a labor of love from 3 Skyrim modders, who care a little bit *too* much about visuals, to provide an expansive graphical package that covers animations, provides custom recolors for various mods to seamlessly tie everything together, and a plethora of handpicked assets for an enhanced Skyrim experience. **This modlist does not offer the full Creation Club Content suite.**

There are minor gameplay changes within the list, which are nothing too drastically altering, but consist of QOL mods such as [True Directional Movement](https://www.nexusmods.com/skyrimspecialedition/mods/51614) to fix janky vanilla movement. Also included are unofficial patches, such as [USSEP](https://www.nexusmods.com/skyrimspecialedition/mods/266) and [USMP](https://www.nexusmods.com/skyrimspecialedition/mods/49616), to fix exploits and bugs. 

If you're curious about the specific mods in the list, the full modlist can be viewed [here](https://loadorderlibrary.com/lists/ascensio-1).


*This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).*

---

### System Requirements

> Please note these specs are the best idea of a baseline that I can provide at the current moment, based on my own experiences to maintain 50-60 FPS, dipping into the 40s in heavily forested areas. In the future this will be updated depending on feedback received.


**My Specs (1080p):**
- i7-9700k
- RTX 2070s
- 32GB RAM (2x16)
- 980 NVMe

**Recommended Specs (1080p)**
- R7 3700x / i5 10600k
- 3060 Ti / 2070 / 6700 XT
- 16GB RAM (2x8)
- SATA SSD


**Modlist Size:**
- Downloads: ~110 GB
- Install: ~137 GB (actual final size may vary)
- **TOTAL:** ~247 GB

 > Wabbajack requires some extra space on your main OS drive for temporary and working files during the installation. This space is not counted towards the total install space of the list for sake of this guide, however Wabbajack roughly accounts for it in the UI.
---
## Installation

Installing Ascensio is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the modlist, you can safely skip to the [updating section](#updating-the-modlist).

---

### Pre-Installation

These steps are only required for installing the modlist for the first time. Many of these steps may be covered in other modlist installs, but for new users I suggest reading through here regardless.

 1. Install [Microsoft Visual C++ Redistributables](https://aka.ms/vs/17/release/vc_redist.x64.exe) & [.Net Runtime v6 desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime).
 2. Change Skyrim so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
 3. Right click on Skyrim SE and click on properties, untick the `Enable Steam Overlay while in-game` option.
---
#### Pagefile and crash prevention

Larger Skyrim modlists require a significant amount of memory, running out of memory **will** result in crashes and other potential issues. This step is **NOT** optional. Regardless of how much RAM or VRAM you have, please do this step.

 To set up your pagefile:
 1. Press **Win Key + R**
 2. Type *sysdm.cpl ,3* and hit **ENTER**
 3. Navigate to *Performance* and click the box "Settings..."
 4. Click the *Advanced* tab at the top
 5. Under *Virtual Memory* click the box "Change..."
 6. Uncheck *Automatically manage* if it is checked
 7. Select your disk drive, ideally your fastest solid state drive
 8. Click the **Custom size:** button
 9. In the box next to **Initial Size (MB)** type `20480`
 10. In the box next to **Maximum Size (MB)** type `20480`
 11. Click the *Set* button
 12. Click *OK*
 13. Click *Apply*
 14. Click *OK*
 15. Restart your computer in order for your new pagefile to take effect.

---

#### Setting Shader Cache Size
 Additionally, if you have an NVIDIA GeForce Graphics Card, please do the following:
 This step is **optional** but can provide some extra stability.

 1. Right-click on your desktop and select **NVIDIA Control Panel**
 2. Navigate and click on **Manage 3D settings**. It is the 2nd one to the top.
 3. Scroll down in Global Settings until you see **Shader Cache Size**
 4. Double Click **Driver Default** to the right of Shader Cache Size and select **10 GB**
 5. Click **Apply** in the bottom right hand corner.
 6. You may exit out of the application.
![](https://raw.githubusercontent.com/iAmMe27/Tahrovin/main/img/ShaderCache.png)

---

#### Steam Setup

 If you have your Steam Library in Program Files, read [this](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) and move it elsewhere. Locations such as Desktop, Documents, Downloads, OneDrive, etc. will cause issues with installing and playing the list.

---

#### Game Language

The English Steam version of Skyrim is the only supported version. I understand that this may be frustrating for non-English speaking users or users with the GOG versions, but due to the core file differences between the different versions, I am only able to support one game version.

 1. Right click on your Skyrim in Steam
 2. Click *Properties*
 3. Click *Language*
 4. Set the Language to English.

---

### Wabbajack Installation

#### Installing Wabbajack

Once you have completed pre-installation, download the [latest version of Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases) from the Wabbajack Github. Extract the contents of the Wabbajack archive and place it in a folder such as `C:\Wabbajack` for example. **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), or in your Skyrim's Steam folder**. I recommend placing it on an SSD as it will work quicker on there.

---

#### Downloading and Installing Ascensio

Downloading and installing Ascensio can take a while depending on your internet connection and computer. To install Ascensio, complete the following steps.

1. Open Wabbajack and click `Browse Modlists`. Then pick the `Skyrim Special Edition` from the game filter drop-down box or use the search bar to type in the name of the list.
2. Press the download arrow on the Ascensio UI card and wait for it to download.
3. Set the installation folder to be a path such as `C:\Games\Ascensio`. **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, etc.), or in your Skyrim's Steam folder**
> The download location does not need to be on a SSD, but it makes installing faster. The downloads location does not need to be on the same drive as the installation folder path either.
1. Press the play button to begin.
2. Turn on your favorite show or a nice long video essay as Wabbajack does its thing. Alternatively read through this readme again :D
3. If the installation is successful, then rejoice and move onto [post installation](#post-installation-and-optional-setup). If the installation is unsuccessful, follow some of the pointers below or join the [discord server](https://discord.gg/WakingDreams) for support.

Sometimes Google Drive and MEGA will experience bandwidth caps, so below I have included the links to the files that require them.
- [High Poly Head](https://drive.google.com/file/d/15_0njBUjHKidNnJPmLXEygzGVWsA3Zbq)
- [Elwaps Speedtree](https://mega.nz/file/xUc0zRLY#NYwbmmHOZhpSF2hpV7hMRYejgZsL_MAIVv_DfjK9JRM)

---

### Problems with installation

It is possible that you may encounter an error with Wabbajack when installing. Some common issues are listed below:

- Could not download **X**:
	- Big files can fail to download due to connection issues. You can either run Wabbajack again or download the file manually. If you decide to manually download it, make sure to place the archive in the downloads folder that was specified in the [Downloading and Installing Ascensio](#downloading-and-installing-ascensio) section.

- **X** is not a whitelisted download:

	 - This may happen when I update the modlist. Please check if there is a new update or wait until you see a release ping on the discord server!

- Wabbajack could not find my game folder:

	- Either buy the game or go back to the [Pre-Installation](#pre-installation) step.

- Antivirus reports a virus:
	- Windows 10/11 may automatically quarantine a key file which is needed for Mod Organizer. You can fix this by [adding an exclusion for Mod Organizer in Windows Defender](https://www.thewindowsclub.com/exclude-a-folder-from-windows-security-scan).

- Unable to download `Skyrim_Default.ini`:
  - This error means you failed to follow the readme. Go back to the [Game Language](#game-language) section and set your game's language to English.

---

## Post-Installation and Optional Setup

### Game Folder

Ascensio uses a Wabbajack feature called Stock Game to keep your Skyrim installation clean. Your Skyrim install for Ascensio should be self-contained and located in a folder named `Stock Game` within your Acsensio folder.

---

### Antivirus Exceptions

Generally speaking, using Windows Defender is advised as it is a solid antivirus software that will have minimal interference with the game. Antivirus programs can be notorious for false flagging MO2's VFS as problematic, causing crashes or other problems. Antivirus programs like BitDefender, Norton, and Webroot are especially aggressive, and you will very likely need to fully remove them from your PC in order to actually launch the game through MO2.

If you use Windows Defender, it is advised that you set up an exception for the modlist. To do this, follow these steps:
 1. Press the Windows Key.
 2. Type "Windows Defender" in the search bar and select "Windows Security".
 3. Click on "Virus & threat protection" in the left pane.
 4. Click the "Manage settings" option under "Virus & threat protection settings".
 5. Scroll down to "Exclusions" and click "Add or remove exclusions".
 6. Windows Defender will prompt you with a run as administrator screen, just hit yes.
 7. Click the "Add an exclusion" button at the top and choose "Folder".
 8. Navigate to your Install folder for the list and click "Select Folder".
 9. **(OPTIONAL)** You can repeat these steps for the other executables:
    - ModOrganizer.exe (`[Path to Modlist]\ModOrganizer.exe`)
    - Nemesis Unlimited Behavior Engine.exe (`[Path to Modlist]\mods\Project New Reign - Nemesis Unlimited Behavior Engine\Nemesis_Engine\Nemesis Unlimited Behavior Engine.exe`)
    - Synthesis.exe (`[Path to Modlist]\tools\Synthesis\Synthesis.exe`)

---

## Playing the List

### Starting the Game

Open up the installation folder you set for Ascensio, locate an executable named `ModOrganizer.exe` and launch it.

**Before you start playing the game, I suggest reading over the [Configuration Page](https://github.com/Oghma-Infinium/Ascensio/blob/main/CONFIG.md) and checking the [FAQ](https://github.com/Oghma-Infinium/Ascensio/blob/main/FAQ.md) for any commonly asked questions for the list.**

After you have picked your preferred ENB profile and gone through the [configuration page](https://github.com/Oghma-Infinium/Ascensio/blob/main/CONFIG.md), click the run button next to the `Play Ascensio` executable in MO2. You are now free to play, have fun!

---

## Updating the modlist

Before updating, please check the [changelog](https://github.com/Oghma-Infinium/Ascensio/blob/main/CHANGELOG.md). You may need to start a new game after certain updates.

Updating is like installing the list. Simply make sure your install/downloads paths are the same wihtin Wabbajack and tick on the `overwrite installation` button.

**Note**: Any mods you have added will be deleted when updating. To make sure that Wabbajack does not delete your added mods upon updating, prefix your mods with **[NoDelete]**.

---

## Removing the Modlist
Simply delete the Ascensio folder. Congratulations, you have uninstalled Ascensio.

## Contact

If you have an issue with the list, please feel free to join the [Waking Dreams](https://discord.gg/WakingDreams) discord server for support!

## Credits and Thanks

- _YOU_ for reading this :D
- Curly for the original iteration of Ascensio!
- The Waking Dreams server <3
- JTK for his visual academy that jumpstarted this list
- Bethesda Game Studios
- ElminsterAU and the xEdit team
- Noggog for Mutagen and Synthesis
- Halgari and the WJ Team for this amazing platform
