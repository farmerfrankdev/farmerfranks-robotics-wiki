# Robots

[Home](README.md)

Every robot is a [Robot Frame](Robot-Workshop.md) with a **Neural Chip** in it, built at the Robot Workshop. The chip decides what kind of robot it is. All robots are set up with the [Robot Linker](Robot-Linker.md), and walk back to their own [Charging Station](Charging-Station.md) when their battery drops to 10 %.

| Robot | What it does | Linker asks for | Energy use |
|---|---|---|---|
| ![](images/robot.png) [Transporter](Transporter.md) | Carries items from one inventory to another | pickup chest, delivery chest, charger | 1× |
| ![](images/robot_collector.png) [Collector](Collector.md) | Picks up items on the ground in its area | area, delivery chest, charger | 1× |
| ![](images/robot_lumberjack.png) [Lumberjack](Lumberjack.md) | Fells trees and replants saplings | area, sapling chest, charger | 2× |
| ![](images/robot_killer.png) [Killerbot](Killerbot.md) | Hunts hostile mobs | area, charger | 4× |
| ![](images/robot_planter.png) [Planter](Planter.md) | Tills ground near water and sows seeds | area, seed chest, charger | 1× |
| ![](images/robot_harvester.png) [Harvester](Harvester.md) | Harvests ripe crops | area, delivery chest, charger | 1× |
| ![](images/robot_fisher.png) [Fisher](Fisher.md) | Fishes in water | area with water, delivery chest, charger | 1× |
| ![](images/robot_breeder.png) [Breeder](Breeder.md) | Feeds animals so they breed | area, feed chest, charger | 1× |
| ![](images/robot_butcher.png) [Butcher](Butcher.md) | Keeps a set number of animals, butchers the rest | area, delivery chest, charger | 2× |
| ![](images/robot_courier.png) [Power Porter](Power-Porter.md) | Carries energy between batteries | source battery, target battery, charger | 1× |
| ![](images/robot_fluid_porter.png) [Fluid Porter](Fluid-Porter.md) | Carries fluids between tanks | source tank, target tank, charger | 1× |
| ![](images/robot_miner.png) [Miner](Miner.md) | Digs out its area layer by layer, all the way down | area, chest (with ladders), charger | 2× |
| ![](images/robot_shearer.png) [Wool-E](Wool-E.md) | Shears the sheep and delivers the wool | area, delivery chest, charger | 1× |
| ![](images/robot_arc.png) [ArcBot](ArcBot.md) | Shoots arcs of electricity at hostile mobs from afar | area, charger | 2× |

## Things every robot does
- **Right-click** a robot with an empty hand to see its type, battery and what it is doing.
- **Shift + right-click** it with an empty hand to pick it up. It keeps its charge, modules and setup, so you can put it down somewhere else.
- A robot holds **10 000 FE** on its own, more with a [Battery Module](Battery-Modules.md). Even standing still uses a little energy, so robots charge now and then.
- A robot without power stops and slumps over.
- Mobs never target or hurt robots.
- Robots walk straight through a [Robot Revolving Door](Robot-Revolving-Door.md), so they can work inside pens and mob farms.
- An area can be up to **32 × 32** blocks, or **48 × 48** with a [Range Upgrade](Upgrades.md). Servers can change both in the [config](Configuration.md).

## Good combinations
- **Tree farm:** a Lumberjack fells the trees and a Collector picks up the logs. Put the saplings on [Fertilized Dirt](Fertilized-Dirt.md) to make them grow four times as fast.
- **Crop farm:** a Planter sows and a Harvester harvests. Give the Planter the Harvester's chest as its seed chest, and the farm runs by itself.
- **Animal farm:** a Breeder breeds and a Butcher keeps the numbers down. Add Wool-E to shear the sheep.
- **Mob farm:** a Killerbot in a dark room, with a Collector for the drops. Add an ArcBot for spiders, blazes and other mobs a Killerbot cannot reach.
- **Remote base:** a Power Porter carries energy from your generators to a battery far away.
- **Quarry:** a Miner digs a shaft down to bedrock and fills its chest with ores. Give it a Blacklist Filter for stone and dirt.
- **Fluids without pipes:** a Fluid Porter carries water, lava or other mods' fluids between [Glass Tanks](Glass-Tank.md) and machines.
