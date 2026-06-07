## Underbarrels

Underbarrels can be equipped on guns. The default keybind is X.

| Function     | Animation Name             |
|--------------|----------------------------|
| Equip        | "sub_transform_UBID"       |
| Static Idle  | "sub_static_idle_UBID"     |
| Shoot        | "sub_shoot_UBID"           |
| UnEquip      | "transform_UBID"           |
| Draw         | "sub_draw_UBID"            |
| Stow         | "sub_put_away_UBID"        |
| Inspect      | "sub_inspect_UBID"         |
| Reload       | "sub_reload_tactical_UBID" |
| Reload Empty | "sub_reload_empty_UBID"    |
<br>

![blockbench example.png](resources/blockbench%20example.png)
<br>
In order to get animated underbarrels, it uses the "attachment_adapter". The attachment is always a part of the gun, it only shows up once its corresponding "attachment_adapter" is installed. It is reccomended that in "master_parameter_attachment.json" to set the grip translation to be [1000,1000,1000], to avoid any model clipping.
<br>
<br>
<br>
The underbarrels are declared in "underbarrels.json"
<br>
![underbarrelsjsonex.png](resources/underbarrelsjsonex.png)
<br>


Underbarrels can be mag fed. If mag fed, the player must manually prime between shots to cycle the action.
<br>
![underbarrelmag.gif](resources/underbarrelmag.gif)![underbarrel mag.mp4](resources/underbarrel%20mag.mp4)
<br>
Traditional tube underbarrels also work just fine.
<br>
![ubgl.gif](resources/ubgl.gif)


