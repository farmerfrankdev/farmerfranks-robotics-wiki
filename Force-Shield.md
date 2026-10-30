# Force Shield and Scrap Pile

[Home](README.md) · [Robots](Robots.md)

The [Killerbot](Killerbot.md) and the [ArcBot](ArcBot.md) fight, and mobs fight back. Hostile mobs nearby go after them, not only after players. All the other robots are machines that mobs leave alone, as before.

## The force shield
- A combat robot has a **force shield of 20** on top of **20 health** (twice what other robots have).
- Every hit takes the shield first. It flashes blue around the robot, and goes down with a crack of glass when it is empty. Only then does the robot's body take damage.
- **3 seconds after the last hit**, the shield charges back up from the robot's battery: **200 FE per point**, so a full shield costs 4 000 FE. A hard fight drains the battery faster, and the robot has to charge more often.
- While it charges at its station, its body mends a point every two seconds.
- Right-click it or use the [Robot Panel](Inspector.md) to see its shield and health.

## Creepers
Creepers never go after robots, so they will not walk up to them and blow up your base. Your robots still hunt creepers as before, and an ArcBot gets them from afar.

## Scrap Pile
If a combat robot is beaten, it does not drop or vanish: it becomes a **Scrap Pile** where it fell. The pile never despawns, and creepers and the Wither cannot blow it away.

- Break it with a pickaxe to pick it up. It still holds the whole robot: its chip, battery, upgrade, filter, name and setup.
- Put it in an **anvil** with **4 Coppersteel Ingots** (and 3 levels of experience), and you get the robot back as it was.

## Turning it off
In the config, `robots.combat_robots_take_damage = false` makes mobs leave all robots alone again, as in older versions. See [Configuration](Configuration.md).
