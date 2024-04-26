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

# Attention

**Modlist Support: [Waking Dreams](https://discord.gg/4WwqfK5yHg)**

**You must update Skyrim to the latest version (1.6.1170) on Steam to install this modlist.**

**Ascensio does NOT require the paid AE DLC nor does it include ANY Creation Club content.**

# Contents

- [Attention](#attention)
- [Contents](#contents)
  - [Introduction](#introduction)
    - [System Requirements](#system-requirements)
  - [Installation](#installation)
    - [Pre-Installation](#pre-installation)
      - [Pagefile and Crash Prevention](#pagefile-and-crash-prevention)
      - [Setting Shader Cache Size](#setting-shader-cache-size)
      - [Steam Setup](#steam-setup)
      - [Game Language](#game-language)
    - [Wabbajack Installation](#wabbajack-installation)
      - [Installing Wabbajack](#installing-wabbajack)
      - [Downloading and Installing Ascensio](#downloading-and-installing-ascensio)
    - [Problems with installation](#problems-with-installation)
  - [Post-Installation and Optional Setup](#post-installation-and-optional-setup)
    - [Stock Game](#stock-game)
    - [Antivirus Exceptions](#antivirus-exceptions)
  - [Playing the Modlist](#playing-the-modlist)
    - [Starting the Game](#starting-the-game)
  - [Updating the Modlist](#updating-the-modlist)
  - [Removing the Modlist](#removing-the-modlist)
  - [Contact](#contact)
  - [Credits and Thanks](#credits-and-thanks)

## Introduction

Ascensio is a comprehensive visual overhaul modlist for Skyrim Special Edition (v1.5.97) that aims to upgrade just about every visual aspect of Skyrim, from the vanilla animations to the various points of interest around the game. This modlist features an array of meticulously handpicked assets, in-depth method patching for easy configuring, and custom edits and recolors for various mods to seamlessly tie everything together for an enhanced Skyrim experience.

**This modlist does not include any Creation Club Content.**

The list offers no major gameplay-changing mods, such as perk and combat overhauls, since the focus is on overhauling Skyrim's visuals primarily. However, there are some *minor* gameplay mods included, not meant to be drastically altering but to offer some QoL (Quality of Life) tweaks with [True Directional Movement](https://www.nexusmods.com/skyrimspecialedition/mods/51614) and [Verolevi's](https://www.nexusmods.com/skyrimspecialedition/users/3812151?tab=user+files) animations. Mods such as [USSEP](https://www.nexusmods.com/skyrimspecialedition/mods/266) and [USMP](https://www.nexusmods.com/skyrimspecialedition/mods/49616) are also included to fix vanilla bugs and exploits.

If you're curious about the very specific mods in the list, the full modlist can be viewed [here](https://loadorderlibrary.com/lists/ascensio-1).

*This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).*

---

### System Requirements

> Please note these specs are the best idea of a baseline that I can provide at the current moment, based on my own experiences to maintain 50-60 FPS, dipping into the 40s in heavily forested areas. In the future, this will be updated depending on feedback received.

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

 1. Install [Microsoft Visual C++ Redistributables](https://aka.ms/vs/17/release/vc_redist.x64.exe) & [.NET 7.0 Desktop Runtime x64](https://download.visualstudio.microsoft.com/download/pr/515cc796-e9f2-4b5c-be7f-b42f115a65a7/b0b146fcbf1d1c135807ff24b3d88093/windowsdesktop-runtime-7.0.13-win-x64.exe)
 2. Change Skyrim so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable)
 3. Right click on Skyrim SE and click on properties, untick the `Enable Steam Overlay while in-game` option
 4. Remove or disable any 3rd party antivirus such as Webroot or Bitdefender. These programs **will absolutely** cause issues with your Ascensio installation due to how MO2's Virtual File Staging works

---

#### Pagefile and Crash Prevention

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

  This step is **optional** but can provide some extra stability. If you have an NVIDIA GPU, please do the following:

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
 2. Click `Properties`
 3. Click the drop down box next to `Language`
 4. Set the language to English.

---

### Wabbajack Installation

#### Installing Wabbajack

Once you have completed pre-installation, follow these steps to install Wabbajack:

1. Create an empty folder named `Wabbajack` on the root of your drive, such as `C:\Wabbajack` for example. **DO NOT set the folder to Program Files, User protected folders (such as Desktop, Documents, Downloads, etc.), or in your Skyrim's Steam folder**.
   > The `Wabbajack` folder does not need to be on an SSD, but it makes installing faster. You can set this location to be an HDD for the sake of saving space.

2. Download the [latest version of Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases/latest/download/Wabbajack.exe) and place the `Wabbajack.exe` file inside the Wabbajack folder you created in Step 1.

3. Double-click the `Wabbajack.exe` file that is now inside your Wabbajack folder to set up the program.

---

#### Downloading and Installing Ascensio

Downloading and installing Ascensio can take a while depending on your internet connection, PC specs, and if you have Nexus Premium. Without Premium, you will need to manually click the `Slow Download` button for each mod.

1. Open Wabbajack and click `Browse Modlists`. Then pick the `Skyrim Special Edition` from the game filter drop-down box or use the search bar to type in the name of the list.
2. Press the download arrow on the Ascensio UI card and wait for it to download.
3. Set the `Modlist Installation Location` to a folder such as `C:\Ascensio`. **DO NOT set the folder to Program Files, User protected folders (such as Desktop, Documents, Downloads, etc.), or in your Skyrim's Steam folder**.
    > The `Resource Download Location` does not need to be on an SSD, but it makes installing faster. You can set this location to an HDD for the sake of saving space.
4. Press the play arrow to begin.
5. If the installation is successful, then rejoice and move onto the [Post Installation](#post-installation-and-optional-setup) section. If the installation is unsuccessful, use the download links and tips below or join the [discord server](https://discord.gg/WakingDreams) for support.

Sometimes Google Drive and MEGA will experience bandwidth caps, so below I have included the links to the files that require them.

- [High Poly Head](https://drive.google.com/file/d/15_0njBUjHKidNnJPmLXEygzGVWsA3Zbq)
- [Elwaps Speedtree](https://mega.nz/file/xUc0zRLY#NYwbmmHOZhpSF2hpV7hMRYejgZsL_MAIVv_DfjK9JRM)

---

### Problems with installation

It is possible that you may encounter an error with Wabbajack when installing. Some common issues are listed below:

- Could not download **X**:
  - Big files can fail to download due to connection issues or website issues. You can either run Wabbajack again or download the missing file manually. If you decide to manually download the file, make sure to place the file(s) inside the folder you set as the `Resource Download Location` in the [Downloading and Installing Ascensio](#downloading-and-installing-ascensio) section.

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

### Stock Game

Ascensio uses a Wabbajack feature called Stock Game to keep your Skyrim installation clean. Your Skyrim install for Ascensio should be self-contained and located in a folder named `Stock Game` within your Ascensio folder.

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

## Playing the Modlist

### Starting the Game

Open up the installation folder you set for Ascensio, locate an executable named `ModOrganizer.exe` and launch it.

**Before you start playing the game, I suggest reading over the [Configuration Page](https://github.com/Oghma-Infinium/Ascensio/blob/main/CONFIG.md) and checking the [FAQ](https://github.com/Oghma-Infinium/Ascensio/blob/main/FAQ.md) for any commonly asked questions for the list.**

After you have picked your preferred ENB profile and gone through the [configuration page](https://github.com/Oghma-Infinium/Ascensio/blob/main/CONFIG.md), click the run button next to the `Play Ascensio` executable in MO2. You are now free to play, have fun!

---

## Updating the Modlist

Before updating, please check the [changelog](https://github.com/Oghma-Infinium/Ascensio/blob/main/CHANGELOG.md). You may need to start a new game after certain updates and I will state so in the changelog if needed.

To update a modlist, follow these steps:

1. Open Wabbajack again
2. Download the newest Wabbajack file for your list from the `Browse Modlists` section
3. Select the same `Modlist Installation Location` and `Resource Download Location` folders you chose previously
4. Click the play button to begin installation

Backup **any** changes you have made to the modlist, such as INI tweaks and mod configs, since these will be lost upon reinstall.

**NOTE**: If you want to keep any mods you've added to your personal install, prefix those mods with **[NoDelete]** to force Wabbajack to skip those files. Note that support still won't be officially provided; use this feature at your own discretion.

---

## Removing the Modlist

Simply delete the Ascensio folder. Congratulations, you have uninstalled Ascensio.

## Contact

If you have an issue with the list, please feel free to join the [Waking Dreams](https://discord.gg/WakingDreams) discord server for support!

## Credits and Thanks

- *YOU* for reading this :D
- Curly for the original iteration of Ascensio!
- The Waking Dreams Dev team <3
- JTK for his visual academy that jumpstarted this list
- Bethesda Game Studios
- ElminsterAU and the xEdit team
- Noggog for Mutagen and Synthesis
- Halgari and the WJ Team for this amazing platform
