# Configuration

[Home](README.md)

FarmerFrank's Robotics has two config files in the `config` folder. Both are created the first time the game starts.

## `farmerfranks_robotics-local.toml`: which robots are in the game
```toml
[robots]
	transporter = true
	collector = true
	lumberjack = true
	killer = true
	planter = true
	harvester = true
	fisher = true
	breeder = true
	butcher = true
	power_porter = true
	fluid_porter = true
	miner = true
```
When a robot is set to `false`:
- its Neural Chip has no recipe;
- it is hidden from the creative menu and JEI;
- its chip cannot be put in at the Robot Workshop;
- robots of that kind already in a world stand still. They can still be picked up.

**Restart the game, or the server, after changing it.** A server and its players should use the same file, as a modpack does.

## `farmerfranks_robotics-synced.toml`: balance
The server sends these values to every player, so only the server's file counts. A world can override them with a file of the same name in its `syncedconfig` folder.

| Setting | Default | Range | What it does |
|---|---|---|---|
| `energy.energy_per_coal` | 10000 | 100 – 1 000 000 | FE from one coal in a generator. Other fuels give energy in proportion. |
| `energy.stone_generator_fe_per_tick` | 25 | 1 – 10 000 | Stone Generator output |
| `energy.iron_generator_fe_per_tick` | 50 | 1 – 10 000 | Iron Generator output |
| `energy.robot_energy_use` | 1.0 | 0.0 – 10.0 | How much energy robots use: 0.5 is half, 2.0 is twice |
| `robots.max_area_size` | 32 | 4 – 128 | Biggest work area, in blocks along each side |
| `robots.range_upgrade_area_size` | 48 | 4 – 256 | Biggest work area with a Range Upgrade |
| `robots.breeder_max_animals_per_kind` | 16 | 2 – 256 | A Breeder stops feeding a kind of animal at this many |
| `robots.butcher_default_keep` | 8 | 1 – 256 | Animals of each kind a Butcher keeps, until changed with the Inspector |
| `robots.porter_cargo` | 25000 | 1 000 – 10 000 000 | FE a Power Porter carries at a time (twice with a Capacity Upgrade) |
| `robots.fluid_porter_cargo` | 4000 | 100 – 1 000 000 | mB a Fluid Porter carries at a time; 1000 is a bucket (twice with a Capacity Upgrade) |
| `robots.miner_max_area_size` | 16 | 2 – 64 | Biggest area a Miner digs out, in blocks along each side (twice with a Range Upgrade) |
| `robots.nearby_charger_range` | 16 | 0 – 64 | A robot that needs charging uses a station this close (in blocks) if it is closer than its own. 0 means always its own |

The numbers in the [Robotics Manual](Robotics-Manual.md) and the item tooltips are the defaults, so they do not change with the config.
