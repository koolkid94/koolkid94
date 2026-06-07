## Barrel Blocking

The length of the weapon is now simulated in the world. Longer guns are positioned farther from the center of the screen the closer to an obstructing surface the player gets. The length of distance to the wall is determined by the installed attachments, as well as the gun's base length. [Folded stocks](https://github.com/koolkid94/koolkid94/tree/main/tacz_mags_wiki/Weapon%20Handling/Canted%20Aiming) can shorten a weapon at the cost of recoil gain. If possible, the player will compress the gun closer to the camera before deflecting the barrel out of center. 

![mp5 length.gif](resources/mp5%20length.gif)

![m4 length.gif](resources/m4%20length.gif)


## Return to Center

The time it takes for a gun to return to the center of the screen after being blocked depends on how far it was pushed out of the way, as well as the weight. The following expression approximates the multiplier on the rate of return to center:

$$\left(\frac{1}{0.013w}\cdot 0.001547681 + 0.02\right)\cdot s$$

where **w** is the weight and **s** is the global scale modifier.

![barrel length.gif](resources/barrel%20length.gif)


