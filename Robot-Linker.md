# Robot Linker

[Home](README.md)

![Robot Linker](images/robot_linker.png)

The Robot Linker tells a robot where to work: its chests, its charging station and its area.

![Robot Linker recipe](images/recipes/robot_linker.png)

## Setting up a robot
1. **Right-click the robot** with the linker. This starts a new setup for that kind of robot.
2. **Click what it asks for.** The next step is shown above the hotbar, and you can do the steps in any order:
   - chests, by clicking them;
   - the charging station;
   - an **area**, by clicking the ground at one corner and then at the opposite corner. While you choose the second corner, the area is outlined and its size is shown.
3. **Right-click the robot again** to hand it the setup.

What each robot asks for is listed on [Robots](Robots.md).

## The side you click
The linker remembers which side of a chest or machine you clicked, and the robot uses that side. For a chest it makes no difference, but a furnace or another mod's machine takes different things on different sides:
- click the **top** of a furnace to deliver ore to it, and its **side** to deliver fuel;
- click its **bottom** as the pickup to take out what it has made.

## More places to deliver to
Robots that deliver (Transporter, Collector, Harvester, Fisher, Butcher and Miner) can deliver to more than one inventory.
- **Shift + click two chests:** the robot also delivers to every inventory in the box between them, such as a wall of chests, a row of barrels or a row of furnaces. A group can be up to 16 blocks long.
- **Shift + click the same chest twice:** adds just that one, so chests can be spread around.
- **Shift + click a chest in a group:** takes that group away again.
- Up to 8 groups, and 64 inventories in all. The delivery chest you clicked normally comes first. Double chests count once.
- Every inventory in a group is delivered to from the side you clicked on the last chest of it.
- **Transporter:** once it has a delivery group, a chest clicked without Shift is always a new pickup chest. A delivery chest is not needed then.

How the robot shares out, switched with **Shift + right-click in the air** while the linker is setting up the robot:
- **Fill one at a time** (the default): it fills one inventory, and moves on to the next when it is full.
- **Round robin:** one load to each inventory in turn.

When all of them are full, it waits, and tries again from the first one.

## Shortcuts
- **Same setup for more robots:** after handing a setup to one robot, right-click more robots of the same kind to give them the same setup.
- **Copy a setup:** Shift + right-click a robot to copy its setup into the linker.
- **Start over:** Shift + right-click in the air. With delivery groups, the first click switches how the robot shares out, so click twice quickly.
- The linker's tooltip shows what is set so far.

## Area size
An area can be up to **32 × 32** blocks, or **48 × 48** for a robot with a [Range Upgrade](Upgrades.md). The linker warns you when an area needs the upgrade. Servers can change both sizes in the [config](Configuration.md).

If you put a robot down without a setup, it tells you to set it up with a linker.
