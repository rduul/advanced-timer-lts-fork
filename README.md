# Advanced Timer — Fabric 26.3 Fork

A highly customizable in-game timer for Minecraft. Place it around your HUD, choose its colors and format, use it as a stopwatch or countdown, and let it pause automatically on selected events. The timer is rendered directly on the HUD and does not use the action bar.

This fork ports the Fabric version of Advanced Timer 1.0.6 to **Minecraft 26.3** while keeping its 26.2 behavior. The fork has been tested in Minecraft 26.3 by its maintainer.

## Features

- Count-up and configurable countdown modes
- Timer saved separately for each world or server
- HUD placement presets and custom coordinates
- Multiple time formats
- Solid colors, two-color gradients, animated gradients, and adjustable gradient visibility
- Optional bold text and paused-state indicators
- Automatic pause on player death, leaving a world, or defeating the Ender Dragon, Wither, Elder Guardian, or Warden
- Countdown end actions: chat message, title, or none
- In-game configuration screen powered by YetAnotherConfigLib (YACL)
- Optional Mod Menu integration for opening the configuration screen
- Commands for starting, pausing, continuing, restarting, showing, hiding, and adjusting the timer

## Compatibility

| | Supported version |
|---|---|
| Minecraft | 26.3 |
| Mod loader | Fabric |
| Java | 25 |

This is a **client-side** mod. Install the following in your Fabric profile:

- Fabric Loader 0.19.5 or newer
- Fabric API
- Fabric Language Kotlin
- YetAnotherConfigLib (YACL)
- Mod Menu (optional)

## Installation

1. Install Minecraft 26.3 with Fabric Loader.
2. Install the required dependencies listed above.
3. Download the Fabric 26.3 JAR from this fork's GitHub Releases or Modrinth project page.
4. Put the JAR in the profile's `mods` folder and launch the game.

## Commands

| Command | Description |
|---|---|
| `/timer start` | Start or resume the timer |
| `/timer pause` | Pause the timer |
| `/timer continue` | Resume the timer |
| `/timer restart` | Reset and start the timer |
| `/timer show` | Show the timer HUD |
| `/timer hide` | Hide the timer HUD |
| `/timer config` | Open the configuration screen |
| `/timer help` | Show command help |
| `/timer time add <time>` | Add time to the timer |
| `/timer time set <time>` | Set the timer value |

Time arguments use seconds, minutes, and hours as separate values. For example, `/timer time add 0 30` adds 30 minutes, and `/timer time add 0 0 2` adds 2 hours.

## Building from source

Build the Minecraft 26.3 Fabric JAR with JDK 25:

```bash
./gradlew :26.3-fabric:jar
```

On Windows:

```powershell
.\gradlew.bat :26.3-fabric:jar
```

The built JAR is produced in the `26.3-fabric/build/libs/` directory.

## Credits and license

Advanced Timer is based on [L3-N0X/advanced-timer](https://github.com/L3-N0X/advanced-timer) by L3-N0X. The upstream project and this fork are distributed under the [MIT License](LICENSE). This fork is an independent community port and is not an official release by the original author.
