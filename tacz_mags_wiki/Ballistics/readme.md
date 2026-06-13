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

The damage of a bullet is largely a function of its velocity. It may be approximated with the formula:

$$
V(d) = \sqrt{\left(v_{0}(p)-20fd\right)^{2}+\left(\frac{400gd}{v_{0}(p)}\right)^{2}}
$$

Where:

- *V(d)* is the bullet's velocity at distance *d*.
- *v₀* is the gun's base velocity (including attachments).
- *p* is the pressure.
- *f* is the friction coefficient.
- *d* is the distance traveled by the bullet.
- *g* is the gravitational acceleration.

Damage can be approximated with the formula

$$D(d) = 0.0084\,V_0\,e^{-\left(\frac{22A_f}{V_0}\right)d} + 0.28\,(D_{\mathrm{ammo}} + 0.01) $$

Pressure is a special stat, as it influences [heat](https://github.com/koolkid94/koolkid94/blob/main/tacz_mags_wiki/Pressure%20System/Heat/readme.md), [pressure](https://github.com/koolkid94/koolkid94/blob/main/tacz_mags_wiki/Pressure%20System/readme.md).

### Buckshot and Slugs
If slugs are loaded, it will slightly increase the accuracy of  whatever it is loaded into, as well as only firing a single pellet. Slug rounds are defined as slugs if the ammo id ends with "sl".
![ammotypes.gif](resources/ammotypes.gif)


![img_1.png](resources/img_1.png)