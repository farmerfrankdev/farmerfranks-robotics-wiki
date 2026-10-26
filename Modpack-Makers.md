# Modpack Makers

[Home](README.md)

You are welcome to use FarmerFrank's Robotics in any modpack. A link back to the [CurseForge page](https://www.curseforge.com/members/farmerfrank/projects) is appreciated. The mod is All Rights Reserved, so please do not re-upload it on its own.

## Turning robots off and tuning balance
See [Configuration](Configuration.md). Ship `config/farmerfranks_robotics-local.toml` and `config/farmerfranks_robotics-synced.toml` with your pack.

## Changing recipes
- **Override a recipe.** Every crafting recipe is a plain JSON file in `data/farmerfranks_robotics/recipe/`. Override one with a datapack, KubeJS or CraftTweaker by using the same recipe id, for example `farmerfranks_robotics:robot_frame`.
- **Change an ingredient through tags.** Recipes use common tags instead of fixed items, so materials from other mods work, and you can change an ingredient everywhere by editing a tag:

| Tag | Used for |
|---|---|
| `c:ingots/coppersteel` | Coppersteel Ingots (this mod adds its own ingot to the tag) |
| `c:ingots/iron`, `c:ingots/copper`, `c:ingots/gold` | ingots |
| `c:nuggets/iron`, `c:nuggets/gold` | nuggets |
| `c:dusts/redstone`, `c:storage_blocks/redstone` | redstone |
| `c:storage_blocks/iron` | iron blocks |
| `c:glass_panes`, `c:glass_blocks`, `c:chests/wooden`, `c:cobblestones/normal`, `c:ender_pearls` | other ingredients |

- **Use the robot condition.** Neural Chip recipes only load while their robot is turned on. Use the same condition in your own recipes:

```json
{
  "neoforge:conditions": [
    { "type": "farmerfranks_robotics:robot_enabled", "robot": "lumberjack" }
  ],
  "type": "minecraft:crafting_shaped",
  "...": "..."
}
```

Robot names: `transporter`, `collector`, `lumberjack`, `killer`, `planter`, `harvester`, `fisher`, `breeder`, `butcher`, `power_porter`, `fluid_porter`.

## Not changeable yet
The Alloy Furnace recipe (iron + copper into Coppersteel) is built into the mod and cannot be changed with a datapack yet.

## Recipe ids
| Item | Recipe id |
|---|---|
| Alloy Furnace | `farmerfranks_robotics:alloy_furnace` |
| Stone / Iron Generator | `farmerfranks_robotics:stone_generator`, `farmerfranks_robotics:iron_generator` |
| Battery | `farmerfranks_robotics:battery` |
| Charging Station | `farmerfranks_robotics:charging_station` |
| Robot Workshop | `farmerfranks_robotics:robot_workshop` |
| Robot Frame | `farmerfranks_robotics:robot_frame` |
| Neural Chips | `farmerfranks_robotics:<robot>_chip`: `transporter_chip`, `collector_chip`, `lumberjack_chip`, `killer_chip`, `planter_chip`, `harvester_chip`, `fisher_chip`, `breeder_chip`, `butcher_chip`, `courier_chip` (Power Porter), `fluid_porter_chip` |
| Battery Modules | `farmerfranks_robotics:copper_battery_module`, `farmerfranks_robotics:coppersteel_battery_module` |
| Upgrades | `farmerfranks_robotics:speed_upgrade`, `range_upgrade`, `efficiency_upgrade`, `capacity_upgrade`, `magnet_upgrade`, `combat_upgrade` |
| Filter Chips | `farmerfranks_robotics:white_filter_chip`, `farmerfranks_robotics:black_filter_chip` |
| Tools | `farmerfranks_robotics:robot_linker`, `farmerfranks_robotics:inspector`, `farmerfranks_robotics:robotics_manual` |
| Blocks | `farmerfranks_robotics:robot_door`, `farmerfranks_robotics:fertilized_dirt`, `farmerfranks_robotics:glass_tank` |
| Coppersteel Sword | `farmerfranks_robotics:coppersteel_sword` |

## Compatibility
- **Mod loader:** NeoForge for Minecraft 26.3.
- **Energy:** standard FE, so pipes and cables from other mods work.
- **JEI (optional):** shows Alloy Furnace recipes, generator fuels and Robot Workshop builds.
- **Multiplayer:** works on dedicated servers.
