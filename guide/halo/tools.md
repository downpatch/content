---
title: Speedrun Tools and Helpful Links
description: Useful tools, setup resources, and links to help with Halo speedrunning.
leaderboard: https://haloruns.com
discord: https://haloruns.com/discord
---

Halo speedrunning tools greatly enhance practice by enabling features like trigger volume viewers, checkpoint control, and AI freezing. These tools let runners efficiently practice difficult sections, refine strategies, and improve consistency, speeding up overall skill development and time improvement.

## Global Tools

The below sections will link and describe tools that can be used in any game category.

### Halo Checkpoint Manager

A practice tool for Halo: The Master Chief Collection

Features:

- Back up (dump) to file the games checkpoints, so you can inject them again at any later time.
- UI for managing your checkpoint collection (ordering, sorting, renaming etc).
- Single-player cheats to help you practice and route the games, such as
- Force custom checkpoints & back them up
- Invincibility
- Speedhack (both slow-down and fast-forward)
- Block the games natural checkpoints
- Teleport and Launch the player
- And more (specific games have different features)
- Support for multiple downpatched versions of MCC - Season 7 (2448), Season 8 (2645), and of course current patch.

You can find a link to the most recent Halo Checkpoint Manager (HCM) version [here.](https://github.com/Burnt-o/HaloCheckpointManager/releases)

### LiveSplit

LiveSplit displays real-time splits for different segments of a game, allowing runners to compare their current performance to personal bests, previous runs, or world records.

To enable LiveSplit for MCC, Type "Halo: The Master Chief Collection" under Game Name, and launch Halo MCC with EAC Off.

[Download Link](https://livesplit.org/)

### HR Patcher

A tool developed by Scales to fix various game crashes that occur on the MCC. Must use with EAC Off.

[Download Link.](https://github.com/Scaless/HRPatcherReleases/releases)

### CheatEngine

[CheatEngine](https://github.com/cheat-engine/cheat-engine) is a development environment used for modding games. While most features are now obsolete thanks to HCM, there is still some applicable use cases for strategy development.

### AutoHotKey

A tool to rebind keyboard keys that are unable to be remapped in-game. Most runners use this to rebind the key that skips the cutscene, swapping Space for T. Use the following code line for AHK (MCC rebind).

    #IfWinActive ahk_exe
    MCC-Win64-Shipping.exe

    Space::t
    t::Space

AutoHotkey can [compile the above script](https://www.howtogeek.com/208224/how-to-add-a-program-to-startup-in-windows/) into an exe which you can then add as a startup program for convenience.

### MCC Downpatching

Work in Progress!

### FlowTimer

FlowTimer is a metronome tool used for timing ultra-precise inputs. This primary has applications in [Halo: Combat Evolved](haloce/index.md); however, it is useful for strategy development in other titles.

[Github Link](https://github.com/stringflow/FlowTimer)

### Reclaimer

[Reclaimer](https://github.com/Gravemind2401/Reclaimer) is a tool for viewing and exporting assets from game files. While it's designed for Halo games, its also possible for developers to create plugins which could support other games, or add additional features related to Halo. In the speedrunning community, we often use this to view map files.

Note: While obsolete for most titles at this point, it can still be useful when mod tools break, which happens.

### Assembly

[Assembly](https://github.com/XboxChaos/Assembly) is a free, open-source Halo cache file (.map) editor that was built from the ground up. It allows users to create and distribute creative patches for game content. This tool is best used to view asset information, such as weapon damage, map assets, and enemy health.

### Halo MCC Mod Tools

Official tools released by 343 Industries that allow players to create, edit, and share custom content for Halo titles included in MCC. These tools are primarily based on the same development kits used by the original Bungie and 343 dev teams, and include access to powerful editors for maps, game logic, scripting, and assets. Currently available for titles like Halo: Reach, Halo: CE, and Halo 2, the tools include:

Tag Editor: For modifying game objects, effects, weapons, and more.

Sapien: A level and scenario editor for placing objects and setting gameplay elements.

Guerilla: A data editor used for tweaking game tags.

Tool: A command-line utility for compiling maps and processing game assets.

These tools can be found in [Steam.](https://store.steampowered.com/app/1532190/Halo_CE_Mod_Tools__MCC/)

### Foobar2000

[Foobar2000](https://www.foobar2000.org/) is used to extract audio files from Halo MCC. This is important for strategy development when measuring dialogue duration.

### Avidemux

[Avidemux](https://avidemux.sourceforge.net/download.html) is a free video editor designed to make simple cuts and tweaks to video clips. This program is great for quick retiming of a run that uses the Real-Time-Attack (RTA) timing method.

## Game-Specific Tools

The below sections will link and describe tools that are used for one specific game or category, including checkpoint libraries.

## Halo: Combat Evolved

### Legendary Practice Saves

The following resource is a collection of checkpoints used for [practicing the game on legendary.](https://drive.google.com/file/d/1TNvm8ZY6kpACNyizkqYCCzGjnZ4AaZrD/view?usp=sharing)

Place the files in the Halo 1 folder for HCM in the following Structure:

    Halo 1
      3251
        Legendary
          Level 
            Classic (For PoA and Two Betrayals)
            Camo Route (For TnR)
            RSS (For 343)
            First Floor Skip (For Library)
            OOB IL Route (For Maw)

### Individual Level Timing Guide

[Resource](https://youtu.be/t364z7XrqlQ) for learning how to retime Halo: Combat Evolved IL runs, as the autosplitter can be inaccurate.

### Halo CE Classic MCC Mod

[Halo CE Classic](https://steamcommunity.com/sharedfiles/filedetails/?id=3249878452) does have different geometry compared to the MCC version, as well as some other game mechanic differences. This mod fixes these dependencies.

### Halo CE Gearbox Port Autosplitters

LiveSplit autosplitters for the Gearbox port of Halo CE. You can download them [here.](https://cdn.discordapp.com/attachments/83062860023861248/1035393227051761714/Halo-IL-Splitters.zip?ex=67fa8556&is=67f933d6&hm=e29db30d11fd3f7af638852a4b6296620ac24eb414fd252d21ab13b2ba0a471d&)

### Halo CE Custom Edition

Work in Progress!

## Halo 2

### Legendary Checkpoint Library

[Checkpoint library](https://www.dropbox.com/scl/fo/wjl7849hy9t1h4df1gz3o/APy522GE8XrDEiIpIaaFqvI?rlkey=1pop0dtiu411kbb5mlnvlt0d3&st=w4v44nuj&dl=0) for practice, to be used with HCM. Note: You must use [HCM v3.1.7.](https://github.com/Burnt-o/HaloCheckpointManager/releases/tag/3.1.7)

### Easy Checkpoint Library

[Checkpoint library](https://www.dropbox.com/scl/fo/qd1ljxfkykg8z9q81zr2j/AJ3Fc19KIH0scKx4ckq7YFw?rlkey=0qa1o7gzid702bkxh2r9dzx8l&st=9uw2zajs&dl=0) for practice, to be used with HCM. Note: You must use [HCM v3.1.7.](https://github.com/Burnt-o/HaloCheckpointManager/releases/tag/3.1.7)

### Language Comparison List

Halo 2 Classic levels are faster or slower depending on the version of the game you play on, and the associated language. The differences can be found [here.](https://pastebin.com/wgpkrKAP)

## Halo 3

### Easy Practice Checkpoints

[Checkpoint library](https://github.com/Burnt-o/HaloCheckpointManager/releases/tag/3.1.6) for practice, to be used with HCM. Note: You must use [HCM v3.1.6.](https://github.com/Burnt-o/HaloCheckpointManager/releases/tag/3.1.7)

### Coordinates Button Combo

Controller Only.

Jump + Crouch + Flashlight + Switch Nades + Reload Hold all at the same time for up to 4 seconds.
