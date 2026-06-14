## Ammo Types

Various different ammo types, each with their own properties, can be loaded into a gun through various [magazines](https://github.com/koolkid94/koolkid94/blob/main/tacz_mags_wiki/Ballistics/Magazines/readme.md). Scopes will need to be zeroed based on load and barrel length.

## Attributes
```json
  "tacz:m855": {
"armor_pen": 1.1,
"damage": 0.55,
"pressure": 1.018,
"air_friction": 0.041572,
"gravity": 0.0439,
"accuracy": 0.83,
"variance": 0.03,
"incendiary": false,
"explosive": false,
"tracer":  false
},
```
# Velocity

The damage of a bullet is largely a function of its velocity. Velocity may be approximated with the formula:

$$
V(d) = \sqrt{\left(v_{0}(p)-20fd\right)^{2}+\left(\frac{400gd}{v_{0}(p)}\right)^{2}}
$$

Where:

- *V(d)* is the bullet's velocity at distance *d* in meters per second.
- *v₀* is the gun's base velocity (including attachments).
- *p* is the pressure.
- *f* is the friction coefficient.
- *d* is the distance traveled by the bullet.
- *g* is the gravitational coefficient.

# Damage

From this, damage as a function of distance can be approximated with the formula:

$$D(d)=\left(\left(\frac{\sqrt{\left(v_0(p)-20fd\right)^2+\left(\frac{400gd}{v_0(p)}\right)^2}}{5\cdot20}\cdot0.75\right)+\left(0.25\left(D_a+0.01\right)\right)\right)\cdot1.12$$

Where:

- *D(d)* is the bullet's damage at distance *d*.
- *v₀* is the gun's base velocity (including attachments).
- *p* is the pressure.
- *f* is the friction coefficient.
- *d* is the distance traveled by the bullet.
- *g* is the gravitational coefficient.
- *$D_a$* is the ammo's damage stat.

There is a secondary $ 1/20 $ term in the velocity weighted section to convert from meters per tick back to meters per second. 

![img.png](../Pressure%20System/resources/img.png)

The variables of pressure, gravity, and friction control both trajectory and damage. Friction is a reduction on the î, and gravity is a scalar magnification of ĵ. To make a bullet fly truer, without speeding it up, decrease both gravity and friction. 

Pressure is a special stat, as it influences [heat](https://github.com/koolkid94/koolkid94/blob/main/tacz_mags_wiki/Pressure%20System/Heat/readme.md), [pressure](https://github.com/koolkid94/koolkid94/blob/main/tacz_mags_wiki/Pressure%20System/readme.md).
<br>
Variance is how much the pressure can vary by. This can cause bullets to fly a bit slower or faster.

### Buckshot and Slugs
If slugs are loaded, it will slightly increase the accuracy of  whatever it is loaded into, as well as only firing a single pellet. Slug rounds are defined as slugs if the ammo id ends with "sl".
![ammotypes.gif](resources/ammotypes.gif)


![img_1.png](resources/img_1.png)