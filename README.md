# Obvilion

**Obvilion** is a custom Minecraft plugin for **Paper/Spigot 1.20.1**, developed by **BeyondLavestar**. It introduces a mysterious afterlife dimension called *Moon*, a customizable in-game menu system, and a special cursed totem mechanic.

## Features

### 🌙 Moon — Afterlife Dimension
- When a player dies, they are teleported to a separate world called **Moon**.
- Moon is an empty dimension with only a sky and a barrier floor to prevent players from falling endlessly.
- A boss bar displays a countdown: `Moon: You will return in 3 minutes`.
- If the player has a bed spawn, they return to their bed location after the countdown. Otherwise, they return to the world's default spawn.
- After three minutes, a return animation lifts the player into the sky before teleporting them back to the original world.
- The countdown and return process are handled automatically.

### 📜 Obvilion Menu
- Open the main menu using `/obvilionmenu`.
- Supports an optional custom quick-action button in Minecraft's pause screen through a compatible client-side integration.
- Menu entries and their settings can be customized through `config.yml`.
- Starts with three menu entries by default.
- Add additional entries using `/menu add <name>`.
- Includes a customizable **Totem** menu entry, replacing the default Quick RTP option.

#### Totem GUI
- Choose the desired enchantment options on the left.
- Select the quantity on the right.
- A red **Cancel** button closes the menu without giving items.
- A green **Give** button confirms the selection.

### ☠️ CurseTotem
- Custom command: `/cursetotem give <player>`.
- Gives the selected player a Totem of Undying enchanted with **Curse of Vanishing**.
- Supports selecting multiple players for a shared curse effect.
- When a selected player's totem activates, the configured curse sequence triggers for the affected players.
- The sequence includes a dramatic teleportation animation toward the void below bedrock, a lightning effect, and a large trident falling from above as a visual finishing effect.
- Players affected by the curse receive a permanent ban, with administrative controls available for managing the punishment.

## Configuration
Obvilion uses `config.yml` to customize supported menu entries and their settings. The goal is to make the plugin flexible and easy to expand without editing the source code for every menu change.

## Information
- **Plugin:** Obvilion
- **Author:** BeyondLavestar
- **Minecraft Version:** 1.20.1
- **Platform:** Paper / Spigot
- **Language:** Java
