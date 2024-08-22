# Spare Some Love To Banner Saga 1 - version 3.4

> for Banner Saga 1, Steam version 2.58.17 / GOG version 2.58.17

> Now includes **Nafeij's Pillager Submod for BS1**

**Spare Some Love To Banner Saga 1** is a legacy-support mod for Banner Saga 1, build on top of the original unofficial patch by YaK of all Trades (YaK#2186).

The mod corrects bugs, inconsistencies and typos in the video game Banner Saga 1 by Stoic Studios. It also restores some never-before-seen cut-content and features various QoL improvements.

This repo also includes **Nafeij's Pillager Submod for BS1**, an optional addon for SSLTBS1 which activates *Pillage Mode* at the start of battles; for masochists who wish to experience the challenge of *Survival Mode* with the difficulty curve of the first installment.

Many thanks to:
 - Gestaltzerfall, who updated TBSDecompiler - http://www.mediafire.com/file/wun36alp6ojlkjk/TBS_Decompiler3.2.3.air/file
 - Ratatoskr
 - Drake713
 - Nafeij
 - Aleo

Please report any bugs in [Issues](../../issues).

# Latest releases

> ## 3.4
> 6 Feb 2023
> - Fixed variation of previous Ekkill import bug where his state is not correctly set if you have Ekkill has a prisoner and release him afterwards.

> ## 3.3
> 1 Feb 2023
> - Added **Nafeij's Pillager Submod** option. Enables pillage mode at battle start.
> - Restructured folder directory to accommodate submod.

> ## 3.2
> 26 Jan 2023
> - Shifted the character sprites around in the first Vognir conversation so that Hakon isn't blocked by Ubin's fat arm.
> - Miscellaneous typos. Thanks ingman112!

---

# Installation

1. Download the archive from [Releases](../../releases).
2. Uncompress the zip archive and place the `/tbs1` folder in your game folder (e.g. `.../steamapps/common`). It will ask you to overwrite some files.

## Nafeij's Pillager Submod for BS1

1. Follow the installation steps above.
2. Additionally, download the archive `Nafeij's Pillager Submod for BS1.zip`, and patch this over the same files above.

### GOG w/ Pillager Submod only

NOTICE: The base mod does not overwrite any engine code, but the Pillager Submod does. GOG users would additinally need to download the archive `Nafeij's Pillager Submod for BS1_GOG.zip`, and patch this over the files above.

## Mod-Enabler Integration

The root folders are structured to be compatible with mod-enablers like [OvGME](jweisner/ovgme) and [JSGME](https://www.subsim.com/radioroom/showthread.php?t=204594).

Simply place the extracted root folder (**NOT** the `/tbs2` folder) in the configuration mods folder (`/MODS` in JSGME) and load the mods into your game's root directory (e.g. `.../steamapps/common`).

## To Uninstall

`Properties -> Verify the integrity of game files` in Steam or `Manage installation -> Verify / Repair...` in GOG.

# See also

- [Drake's & YaK's Fixpack for BS2](../../../Drake-s-and-YaK-s-Unofficial-Fixpack-for-BS2)
- [Nafeij's BS3 Fixpack](../../../Nafeij-s-BS3-Fixpack)
