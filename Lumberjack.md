# Lumberjack

[Home](README.md) · [Robots](Robots.md)

![Lumberjack](images/robot_lumberjack.png)

The Lumberjack fells whole trees in its area at once, swinging its axe until the tree comes down. A big tree takes longer than a small one. It keeps the saplings that fall from the leaves and plants **the same kind** where each tree stood: a birch where the birch was, four dark oak saplings where a dark oak stood. The logs and everything else that drops are left on the ground. It wears a red flannel shirt.

## Recipe
Build it at the [Robot Workshop](Robot-Workshop.md) from a Robot Frame and a **Lumberjack Neural Chip**.

![Lumberjack Neural Chip recipe](images/recipes/lumberjack_chip.png)

## Setup
With the [Robot Linker](Robot-Linker.md), click:
1. two corners on the ground for its area;
2. its charging station.

That's all: it needs no chest.

## Starting a tree farm
Plant some saplings in its area yourself, or just **throw a few on the ground** there. It picks them up and plants them in rows, three blocks apart, with room to walk between the trees. Any kinds can grow in the same area.

## Its saplings
It keeps up to **16 saplings of each kind**, for when a tree drops too few to replace itself. What it has no room for stays on the ground. If a kind runs out, the spot waits until it gets one: from another tree, from the ground, or from a chest. It never plants the wrong kind.

A chest is only needed if the trees keep running out. Add one with **+ Add** next to "Fetches from" in its [Robot Panel](Robot-Linker.md#the-robot-panel) (Ctrl + right-click the robot), and it takes saplings from there when it has none of a kind it needs.

## Tips
- It only cuts trees with natural leaves, so log houses and other buildings made of logs are safe.
- Let a [Collector](Collector.md) work in the same area to pick up the logs.
- Saplings on [Fertilized Dirt](Fertilized-Dirt.md) grow four times as fast.
- The [Axe Upgrade](Upgrades.md) makes it fell trees twice as fast.
- A [Filter](Filter-Chips.md) decides which saplings it plants.
- Uses twice the normal amount of energy (2×).
