# Fireteam

Networked 2-player tactical co-op for *XCOM 2: War of the Chosen*.

Fireteam lets two players play missions together over the network without the need of screen sharing or Parsec. Players share one XCOM squad against the AI on the current Steam build (no beta branch needed).

> Work in progress (`v0.8.5`). Core tactical co-op over Steam and LAN is playable through campaign missions.

Host runs the strategy layer and launches missions from their campaign. The partner joins tactical missions directly, and all results (XP, wounds, deaths, loot) stay in the host's campaign.

## Requirements

* *XCOM 2: War of the Chosen* (current Steam build).
* [X2WOTCCommunityHighlander](https://github.com/X2CommunityCore/X2WOTCCommunityHighlander) (`v1.32.0` or compatible).
* Matching DLC and mod lists on both machines.
* Clean launch arguments: Do not enable the developer console (`-allowConsole`), as it breaks XCOM 2's networking.

## How to Play

### Hosting a Mission

1. Load into any tactical mission.
2. Click the Co-op icon in the top-right HUD bar.
3. Click HOST (STEAM) to open a private Steam session and invite your partner via the Steam overlay (or HOST BY IP for LAN).
4. Open the Co-op Squad screen from the Co-op menu to assign soldiers to your partner.

### Joining a Mission

1. Launch the game and stay on the Main Menu.
2. Accept your host's Steam invite directly to join.
3. *(For LAN / Direct IP)* Click CO-OP on the main menu bar, choose JOIN BY IP, and enter the host's IPv4 address.

## Known Limitations

* Hardcoded engine networking limits prevent more than two players.
* Some narrative events currently only play on the host's machine.
* Do not add or remove this mod mid-mission. Adding or removing it between missions on the strategy layer is safe.

## Building

This repository contains only the mod's UnrealScript source.

* Built with the XCOM 2: War of the Chosen SDK (Unreal Engine 3 / UnrealScript).
* Standard ModBuddy / [X2ModBuildCommon](https://github.com/X2CommunityCore/X2ModBuildCommon) project structure (`X2TacticalCoop.x2proj`).

## Disclaimer

Fireteam (`X2TacticalCoop`) is a free, fan-made mod. It is not official and is not affiliated with, endorsed by, or supported by Firaxis Games or 2K.
