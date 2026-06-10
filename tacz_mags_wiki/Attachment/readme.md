## Attachments

### Attachment Slots
Flashlights and Lasers can go into each-other's slots and will position themselves on the gun based on the slot installed into.
![swap.gif](resources/swap.gif)

### Attachment Rework
```json
{
  "tacz:attachment_id": {
    "whitelisted_attachments": [
      "tacz:sample_allowed_attachment"
    ],
    "blacklisted_listed_attachment_slots": [
      "GRIP", "BIPOD"
    ],
    "blacklisted_attachments": [
      "tacz:sample_blacklisted_attachment"
    ],
    "transforms": {
      "barrel": [0, 0, 0],
      "bipod": [0, 0, 0],
      "canted_sight":  [0, 0, 0],
      "chamber": [0, 0, 0],
      "charging_handle": [0, 0, 0],
      "extended_mag": [0, 0, 0],
      "flashlight": [0, 0, 0],
      "front_sight": [0, 0, 0],
      "gas_block": [0, 0, 0],
      "grip": [0, 0, 0],
      "handguard": [0, 0, 0],
      "handguard_rail": [0, 0, 0],
      "laser": [0, 0, 0],
      "mount": [0, 0, 0],
      "muzzle": [0.5, 0, 0],
      "pistol_grip": [0, 0, 0],
      "rear_sight": [0, 0, 0],
      "scope": [0, 0, 0],
      "stock": [0, 0, 0],
      "threaded_barrel": [0.5, 0, 0],
      "tube": [0, 0, 0],
      "ub_mag":  [0, 0, 0]
    }
  }
}
```
More attachments will be allowed based on the currently installed attachment's parameters. Transformations are also cumulative. 

### Triple Attachment Blacklist
```json
["tacz:barrel_145_ar", "tacz:gas_block_iron", "tacz:handguard_adar"]
```
This will block any attachment from being installed if 2 out of the 3 attachments with linked listed ID's are already installed.