## Heat

Every gun has its own maximum heat capacity, heat generated per shot, and cooling rate. Attachments can change the max heat capacity and rate, while [bullets](https://github.com/koolkid94/koolkid94/blob/main/tacz_mags_wiki/Ballistics/readme.md) change the heat generated per shot as a function of the system's [pressure](https://github.com/koolkid94/koolkid94/blob/main/tacz_mags_wiki/Pressure%20System/readme.md).
When the heat reaches above 40% of the maximum heat capacity, the barrel will begin to glow, as well as any attachments attached to it. 

![heating.gif](resources/heating.gif)

## Barrel Swap

Certain barrels, as defined in "swappable_barrels.json" are quick change barrels. When a barrel is quick changed, it takes 80% of the total heat with it, substantially cooling down the gun. While in the inventory, any hot barrel will lose 1 point of heat every 20 ticks. 

![barrel swap.gif](resources/barrel%20swap.gif)

## Muzzle Flash

Muzzle flashes also become more common and larger as the gun heats up. Flashiders, as configured by "flash_hiders.json" can scale down the size of any rendered flash.