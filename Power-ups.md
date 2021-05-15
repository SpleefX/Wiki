
This page documents the new power-ups feature introduced in SpleefX v4.5.5

Note that power-ups require **[Holographic Displays](https://dev.bukkit.org/projects/holographic-displays)**, otherwise they will not work.

# Overview
Power-ups are simple buffs (or de-buffs) that appear randomly in an arena on a fixed interval. When they spawn, there will be a **floating item (icon)**, and above it a **hologram (display text)** surrounded by a colorful particles vortex (purely aesthetic reasons)

![Example power-ups](https://i.imgur.com/G6TpjNq.png)

When taken, each power-up has its own capabilities. Some power-ups can also be used as power-downs, as in, the player that takes them gets a negative effect. This can be as simple as slowness effect, nausea effect, or even switching positions with other players.

# Setting up power-ups for an arena

**To add power-ups to an arena, follow the steps below**:
1. Go to the center of the arena
2. Run the following command:
> /\<mode> arena powerupscenter \<arena>
>
> **Example**: /spleef arena powerupscenter test
3. Run `/<mode> arena settings <arena>` and configure the spawning radius for the arena

![Settings UI](https://i.imgur.com/0M5kxBk.png)

4. Configure the arena power-ups in `/<mode> powerups <arena>`:

![Powerups GUI](https://i.imgur.com/K3cUJF4.png)

Done! Power-ups should now spawn in your arena. 

# Configure power-ups
Each power-up has its own file in **/SpleefX/power-ups/**. 

![power-ups folder](https://i.imgur.com/kV1M85c.png)

**I want to clone a power-up but with different settings!**

We got you! You can clone any power-up as long as you maintain the **PowerupType** property. Simply clone the power-up file, change the name of the power-up and then customize it freely.

# The interval of spawning power-ups
1. Go to **config.yml**
2. Scroll down to the **Powerups** section and edit the **SpawnEvery** option.

![SpawnEvery option](https://i.imgur.com/Tgwzm9I.png)
