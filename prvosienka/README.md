# Prvosienka

![Board overview](https://github.com/richardstefun/suzvuk/raw/master/prvosienka/renders/overview.png)

*Eurorack Busboard*

Prvosienka is an eurorack standard compatible busboard capable of providing power for up to 16 modules.
The board can be mounted using standoffs by 17 different screw holes, with 3mm diameter holes. 

## Schematic diagram

![Schematic diagram](https://github.com/richardstefun/suzvuk/raw/master/prvosienka/renders/schematic.png)

**Features**

Board contains a **LF50AB** very low-dropout 5V voltage regulator, which can be used to provide 5V rail, if your PSU does not provide it. You should also cross the "**5V?**" header to enable the regulator.
There are also three **TE-5** type THT fuses. The recommended fuse amperage is *3.15A*, but it's up to you to choose. If you decide to omit it, a thick wire should be used to connect both terminals.
If you want to split the GATE and CV buses, do not install a jumper in the "**Join?**" terminals.
Board also provides polarity markings for flat cables, because it's designed to use pin headers rather than plastic pin header connectors, to save cost and space.

**Capacitors**

This board is designed for **0603** ceramic capacitors (decoupling) and **B-Type** package electrolytic capacitors. It's up to you to choose their values, but recommended to use **100nF** for decoupling and **10uF 25V** for all electrolytic capacitors. You don't need to populate all pads with decoupling capacitors. Recommended placements are next to connectors on edges of board, and **WAGO 256** connectors. The board works fine without any capacitors, you should only add them if you're experiencing any interference

![enter image description here](https://github.com/richardstefun/suzvuk/raw/master/prvosienka/renders/resistors.png)

**Power indicator**

In the middle of the board is a small power indicator that uses 3 LEDs to determine if all power rails do have voltage on them. Those LEDs need 2 kinds of resistors. For **12V** and **-12V** use **1k 0603** resistor, **330R 0603** fits the **5V** rail nicely. You should use an **0603 LED** **10**-**20mA** **LED**. This feature is also optional. 

**! Always check LED's and electrolytic capacitor polarity before soldering**
