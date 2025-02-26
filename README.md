# Minecraft Prop-Hunt

## What is Minecraft Prop-Hunt?

Minecraft Prop-Hunt is a plugin that introduces the classic Prop-Hunt game mode into Minecraft.

### Built for

- **Paper/Spigot 1.20.2**

**⚠️ Only the [official map](https://www.mediafire.com/file/jadzdjcb6ovfi5d/Map_Minecraft_Prop-Hunt.zip/file) is supported for now.**

### Gameplay

Props can take control of any block, armor stand, or item frame. By crouching, they blend into their surroundings by aligning and placing the block they are using at their current position.

Hunters, on the other hand, are equipped with a trident that they can throw to hit the props.

### Available Game Modes

- **Hide and Seek**: The classic game mode where hunters search for hidden props.
- **Sardine**: One player hides while all others seek. When a hunter finds the hidden player (the "sardine"), they must hide with them until only one seeker remains.

### Features

- **Achievements**: Unlockable in-game and in the lobby.
- **Discord Bot Integration**:
  - Assigns roles in the Discord server when a player earns a new achievement.
  - Moves players between voice channels based on their game mode.
- **Dedicated Map Lobby**:
  - Provides an introduction explaining everything players need to know.
  - Allows players to test being a prop before the first game starts.
- **Two Playable Maps**:
  - The Manor
  - The Arena
- **Multi-language Support**:
  - English
  - French

### Customizable Settings

- Preparation time before hunters begin searching.
- Game duration.
- Choice between props becoming hunters or spectators upon elimination.
- Option to separate props and hunters in Discord voice channels.
- Prop health regeneration toggle.
- Adjustable number of starting hunters.
- And more...

### Installation and Configuration

- <ins>**You need to add all necessary information to the plugin file in `plugins/-plugin-` (e.g., bot token, server channel IDs, world name, etc.) or it will crash when booting up**</ins>
- You can configure the server yourself with the instructions below or download the [pre-configured server with the plugin](https://www.mediafire.com/file/vgguiq30qpfn3ym/Minecraft-Prop-Hunt-preconfigured-server.zip/file)

### File placement

- Place the script file in `plugins/Skript/scripts`.

### Dependencies (Do not attempt to update them)

- [**Skript 2.7.1**](https://github.com/SkriptLang/Skript/releases/download/2.7.1/Skript.jar)
- [**Skbee 3.0.0**](https://github.com/ShaneBeee/SkBee/releases/download/3.0.0/SkBee-3.0.0.jar)
- [**Skhttp 1.5**](https://cdn.modrinth.com/data/4PKsHCki/versions/N5RqZp5W/SkHttp-1.5-all.jar)
- [**DiSky 4.12.1**](https://cdn.modrinth.com/data/4KA72Zn8/versions/EZDu9ptL/DiSky%204.12.1.jar)
- [**skript-gui 1.3**](https://github.com/APickledWalrus/skript-gui/releases/download/1.3/skript-gui-1.3.jar)
- [**Skent 3.3.1**](https://github.com/Olyno/skent/releases/download/3.3.1/Skent.jar)
- [**ViewDistanceTweaks 1.5.7**](https://www.spigotmc.org/resources/view-distance-tweaks.75164/download?version=516594)
- [**Skript-Translations 1.0.0**](https://github.com/Gabanger/Skript-Translations/releases/tag/v1.0.0) (also needs to be placed in `plugins/Skript/scripts`)

If you don't want the plugins to check for updates, you can modify their configuration files in `plugins/-plugin-`.

### Server Configuration

#### Changes to `server.properties`

Modify the following lines:

```
allow-flight=true
broadcast-console-to-ops=false
gamemode=adventure
level-type=flat
generate-structures=false
simulation-distance=32
spawn-protection=0
view-distance=32
```

#### Changes to `plugins/Skript/config.sk`

Change line **143** to:

```
disable variable will not be saved warnings: true
```
