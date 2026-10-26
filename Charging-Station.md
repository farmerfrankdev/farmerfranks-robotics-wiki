# Charging Station

[Home](README.md)

![Charging Station](images/charging_station.png)

A low pad that robots stand on to charge. **Every robot needs its own Charging Station**, set with the [Robot Linker](Robot-Linker.md).

When a robot's battery drops to 10 %, it walks back to its station, stands on it until it is full, and then goes back to work. The pad lights up while a robot charges.

![Charging Station recipe](images/recipes/charging_station.png)

## Powering it
The station holds 20 000 FE and takes up to 500 FE/t. It takes energy in from any side:
- a [Battery or a generator](Energy.md) right next to it;
- a pipe or cable from another mod.

Each side that has something attached gets a connector at the edge of the pad: a socket standing up for a pipe or cable, or a low dock along a whole block such as a battery.

Right-click the station to see how much energy it has.

## Tips
- A [Coppersteel Battery Module](Battery-Modules.md) makes a robot charge twice as fast.
- Several stations can share one battery, as long as each touches it or is piped to it.
