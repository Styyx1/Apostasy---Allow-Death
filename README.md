
![](https://raw.githubusercontent.com/Oghma-Infinium/Apostasy/main/images/Banner.png)



---

**Modlist Support: [Aetherius Modding](https://www.youtube.com/watch?v=QB7ACr7pUuE)**

>[!IMPORTANT]
>Apostasy - Allow Death requires the four free AE mods (Fishing, Rare Curios, Survival Mode, and Saints and Seducers) included in the Skyrim Anniversary Edition update from November 2021.

>[!WARNING]
>You must update Skyrim to the latest version (1.6.1170) on Steam to install this list.


## Introduction

Apostasy - Allow Death is a fork of the Apostasy modlist with disabled Death Alternative mods and some minor visual changes, specifically to armors. It's enough to be a standalone list and thank you Aljo for allowing me to fork the list and keep the name as is.
Here's the Original introduction to Apostasy as i wanted to keep it as is as some form of credit.
Apostasy is a modlist for Skyrim Special Edition offering high-fidelity visuals, expanded and enhanced locations, new quests, and modern, action-oriented gameplay. Developed over the course of thousands of hours, with input from an experienced group of modlist creators and curators—known for lists like [Arisen](https://github.com/The-Animonculory/Curseadelica/blob/main/README.md), [Ascensio](https://github.com/The-Animonculory/Curseadelica/blob/main/README.md), [Fahluaan](https://github.com/The-Animonculory/Curseadelica/blob/main/README.md), and [Vagabond](https://github.com/The-Animonculory/Curseadelica/blob/main/README.md)—Apostasy brings a refined and immersive Skyrim experience like never before.

A full list of the mods used in this modlist can be viewed [here](https://www.youtube.com/watch?v=QB7ACr7pUuE).

You can find a summary of all relevant gameplay changes and notable mods on the [Gameplay Guide](https://github.com/The-Animonculory/Curseadelica/blob/main/README.md).

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

## Installation

Installing Apostasy - Allow Death is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the modlist, you can safely skip to the [updating section](#wabbajack-installation).

### Pre-Installation

These steps are only required for installing the modlist for the first time. Additionally, many of these steps may be covered in other modlist installs, for new users I suggest reading through here regardless.

#### Installing Microsoft Visual C++ and .NET

 1. Install [Visual C++ x64](https://aka.ms/vs/17/release/vc_redist.x64.exe).
 2. Install [.NET Runtime 9.X.X Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/9.0).
 3. Install [.NET 6.0 Runtime Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.30-windows-x64-installer).

>[!WARNING]
>If you already have Visual C++ installed, please make sure you install it again and use the `Repair` option to get the latest version of the redistributables. **Do NOT skip this step or MO2 and the game may fail to launch.**

#### Pagefile and Crash Prevention

>[!WARNING]
>Larger Skyrim modlists require a significant amount of memory, running out of memory **will** result in crashes and other potential issues. Due to Apostasy's size and number of files, this step is **NOT** optional. I do not care how much RAM or VRAM you have, please do this step.

**To set up a Pagefile:**

 1. Press `Win Key + R`
 2. Type `sysdm.cpl ,3` and hit `ENTER`
 3. Navigate to **Performance** and click the box `Settings...`
 4. Click the **Advanced** tab at the top
 5. Under **Virtual Memory** click the box `Change...`
 6. Uncheck `Automatically Manage` if it is checked
 7. Select your disk drive, ideally your fastest solid state drive
 8. Click `Custom Size:`
 9. In the box next to **Initial Size (MB)**, type `40960`
 10. In the box next to **Maximum Size (MB)**, type `40960`
 11. Click `Set`.
 12. Click `OK`.
 13. Click `Apply`.
 14. Click `OK`.
 15. **Restart your PC**.

>[!TIP]
> Your pagefile does not need to be on the same drive as your Wabbajack install or Steam install.

<Details>
<summary>ICYWW: Why do we need a Pagefile?</summary>

Skyrim is a very old game (originally released in 2011) that is built on the [Creation Engine](https://en.wikipedia.org/wiki/Creation_Engine), a engine based off of the [Gamebryo](https://en.wikipedia.org/wiki/Gamebryo) engine that was originally used for Morrowind (released in 2002, *before I was born*).  

Through lots of experience and trial-and-error, we have discovered that increasing the window's pagefile can fix certain types of Skyrim crashes, the two most common examples being `Unhandled native exception occurred at 0x7FF6ADC8DDDA` and `Unhandled native exception occurred at 0x0`.  

But why is this? Skyrim appears to use system memory in very unexpected ways, for example it will frequently dip into the pagefile memory despite there being available RAM. Skyrim heavily favors high speed, low latency RAM (the best you can get as of writing this is 6000MHz and CL30 for DDR5).  

</Details>

#### Steam Setup

>[!WARNING]
>If you have your Steam Library in Program Files, read [this article](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) by LostDragonist. Locations such as Desktop, Documents, Downloads, OneDrive, etc. *will* cause issues with installing and playing the list.

 1. Change Skyrim so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
 2. Right click on Skyrim SE and click on properties, untick the `Enable Steam Overlay while in-game.`
 3. Please ensure you follow the steps outlined in the [Installing Rare Curios Files](#wabbajack-installation) section. **DO NOT SKIP THIS STEP OR YOUR INSTALL WILL FAIL.**

#### Changing the Game Language

>[!WARNING]
>**The English Steam version of Skyrim SE is the only supported version.**

I understand that this may be frustrating for non-English speaking users or users with the GOG/Bethesda.net versions, but due to the core file differences between the different versions, I am only able to support one game version.

To change your Skyrim SE's language:

 1. Right click on Skyrim SE in Steam
 2. Click `Properties`
 3. Click `Language`
 4. Set the Language to `English`

### Wabbajack Installation

#### Installing Wabbajack

If you made it this far, this tells me at least one thing. You haven't clicked a single link and that makes me sad, now enjoy [this](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
and move to the actual Readme of the list you currently install: [The one and only, Cursedelica](https://github.com/The-Animonculory/Curseadelica/blob/main/README.md)

## Credits and Thanks

- aljo for allowing me to pull this off :)
