# Sharing Robots

[Home](README.md)

A robot belongs to the player who puts it down. On a server, only its owner can:
- pick it up,
- set it up with the [Robot Linker](Robot-Linker.md),
- open its [Robot Panel](Robot-Linker.md#the-robot-panel) (Ctrl + right-click),
- change it with the [Inspector](Inspector.md) (Shift + right-click a Butcher),
- rename it, or hit it.

Anyone else can still right-click it to see what it is doing and whose it is, for example "Collector Robot – 78% battery – Delivering – Belongs to FarmerFrank", and look at it with the Inspector.

## Letting a friend use your robots
| Command | What it does |
|---|---|
| `/robotics trust <player>` | The player can use all your robots, also while you are away. |
| `/robotics untrust <player>` | Takes them off your list again. |
| `/robotics trusted` | Shows who is on your list. |

Two friends who want to share everything just trust each other once.

## FTB Teams
With [FTB Teams](https://www.curseforge.com/minecraft/mc-mods/ftb-teams-forge) installed, your teammates can use your robots too, with nothing to set up. Someone who leaves the team can no longer use them, unless they are on your trust list. Without FTB Teams, the trust list is all there is.

## Good to know
- **Operators** can always use every robot.
- Robots from before robots had owners belong to the **first player who uses them**.
- A robot you pick up and put down again is still yours. A robot item you give away belongs to whoever puts it down.
- The [Robot Monitor](Robot-Monitor.md) shows whose each robot is.
- Servers can turn all of this off in the [config](Configuration.md) (`robots.robot_protection`), and then anyone can use any robot, as before.
