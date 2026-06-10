## Json Format

```json
{
  "ammo": ["tacz:556x45", "tacz:556x45_hp", "tacz:m855", "tacz:m855a1","tacz:m856","tacz:mk262"],
  "ammo_amount": 1,
  "extended_mag_ammo_amount": [
    10,
    20,
    30,
    40,
    60,
    100
  ],
  "bolt": "closed_bolt",
  "loadType": "mag_fed",
  "rpm": 800,
  "length": 0.194,
  "min_gas": 0.75,
  "gas": 1.02,
  "bullet": {
    "life": 0.75,
    "bullet_amount": 1,
    "damage": 6.5,
    "tracer_count_interval": 0,
    "extra_damage": {
      "armor_ignore": 0.2,
      "head_shot_multiplier": 1.5,
      "damage_adjust": [
        {"distance": 25, "damage": 6.5},
        {"distance": 60, "damage": 5.5},
        {"distance": "infinite", "damage": 4.5}
      ]
    },
    "speed": 914,
    "gravity": 0.15,
    "knockback": 0,
    "friction": 0.019,
    "ignite": false,
    "pierce": 1,
    "explosion": {
      "explode": true,
      "damage": 50,
      "radius": 6,
      "knockback": true,
      "delay": 30
    }
  },
  "heat":  {

    "max": 410,

    "per_shot": 1.1,

    "cooling_multiplier": 0.067,

    "cooling_delay": 200,

    "over_heat_time": 1000,

    "min_inaccuracy": 1,

    "max_inaccuracy": 3.2,

    "min_rpm_mod": 1,

    "max_rpm_mod": 1.2
  },
  "reload": {
    "type": "magazine",
    "feed": {
      "empty": 2.4,
      "tactical": 2.3
    },
    "cooldown": {
      "empty": 2.2,
      "tactical": 1.87
    }
  },
  "draw_time": 0.3,
  "put_away_time": 0.43,
  "aim_time": 0.09,
  "sprint_time": 0.18,
  "weight": 1.02,
  "movement_speed": {
    "base": 0.0,
    "aim": -0.15,
    "reload": -0.1
  },
  "crawl_recoil_multiplier": 0.5,
  "fire_mode": [
    "auto",
    "semi"
  ],
  "recoil": {
    "pitch": [
      {"time": 0, "value": [1.74, 1.74]},
      {"time": 0.3, "value": [0.55, 0.55]},
      {"time": 0.5, "value": [-0.125, -0.125]},
      {"time": 0.65, "value": [0, 0]}
    ],
    "yaw": [
      {"time": 0, "value": [-0.92, 0.92]},
      {"time": 0.3, "value": [-0.35, 0.25]},
      {"time": 0.5, "value": [0, 0]}
    ]
  },
  "inaccuracy": {
    "stand": 0.9,
    "move": 5.7,
    "sneak": 0.6,
    "lie": 0.58,
    "aim": 0.167
  },
  "melee": {
    "distance": 1,
    "cooldown": 0.6,
    "default": {
      "animation_type": "melee_stock",
      "distance": 1,
      "range_angle": 30,
      "damage": 2,
      "knockback": 0.5,
      "prep": 0.1
    }
  },
  "allow_attachment_types": [
    "scope",
    "stock",
    "laser",
    "grip",
    "muzzle",
    "extended_mag",
    "bipod",
    "barrel",
    "gas_block",
    "flashlight",
    "pistol_grip",
    "charging_handle",
    "front_sight",
    "rear_sight",
    "tube",
    "threaded_barrel",
    "handguard",
    "chamber",
    "handguard_rail",
    "mount",
    "ub_mag",
  "canted_sight"

  ],
  "mandatory_attachments": [
    "barrel",
    "gas_block",
    "pistol_grip",
    "charging_handle",
    "tube",
    "handguard"
  ],
  "exclusive_attachments": {
  }
}

```
Allow Attachment Types is the definitive list on what types of attachment can possibly be allowed. Mandatory attachments are the mandatory slots that must be filled in order for the gun to be functional. 