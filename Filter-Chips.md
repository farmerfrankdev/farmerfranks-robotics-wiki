# Filters

[Home](README.md)

![Whitelist Filter](images/white_filter_chip.png) ![Blacklist Filter](images/black_filter_chip.png)

A Filter decides what a robot works with. (Before 0.23.0 they were called White and Black Filter Chips.)
- A **Whitelist Filter** is a whitelist: the robot only works with the picked items.
- A **Blacklist Filter** is a blacklist: the robot works with everything but them.

## Using one
1. Right-click with the chip to open it.
2. Shift + click items in your inventory, or click a slot with an item, to add up to 5. Click a slot to remove its item.
   - **Mobs** for a Killerbot, ArcBot, Breeder or Butcher: click **Mobs…** at the top of the screen and pick up to 16 from the list. It has a tab for hostile mobs and one for animals, a search box, and mobs from other mods too. No spawn eggs needed (a spawn egg in a slot still counts as its mob).
   - **Bosses**: the Wither and the Ender Dragon are at the end of the hostile list, marked **Boss**. Robots leave them alone unless you ask: pick one in a Whitelist Filter, or tick **Also bosses** under the list in a Blacklist Filter to hunt everything but what the blacklist lists, bosses too. An empty Blacklist Filter with **Also bosses** ticked hunts every hostile mob.
3. Put the chip into the robot in the filter slot of the [Robot Workshop](Robot-Workshop.md).

## What the filter means for each robot
| Robot | The filter picks |
|---|---|
| [Transporter](Transporter.md) | which items it carries |
| [Collector](Collector.md) | which items it picks up |
| [Lumberjack](Lumberjack.md) | which saplings it plants |
| [Planter](Planter.md) | which seeds it sows |
| [Harvester](Harvester.md) | which crops it harvests, by what they give (wheat) or their seeds |
| [Fisher](Fisher.md) | which catches it keeps |
| [Killerbot](Killerbot.md) | which mobs it hunts, picked with **Mobs…** |
| [ArcBot](ArcBot.md) | which mobs it hunts, picked with **Mobs…** |
| [Breeder](Breeder.md) | which food it uses, or which animals it breeds, picked with **Mobs…** |
| [Butcher](Butcher.md) | which animals it butchers, picked with **Mobs…** |
| [Wool-E](Wool-E.md) | which sheep it shears, by wool color |
| [Fluid Porter](Fluid-Porter.md) | which fluids it carries, by bucket (a lava bucket for lava) |
| [Miner](Miner.md) | which of the blocks it digs it keeps; the rest are thrown away |

## Recipes
![Whitelist Filter recipe](images/recipes/white_filter_chip.png)
![Blacklist Filter recipe](images/recipes/black_filter_chip.png)
