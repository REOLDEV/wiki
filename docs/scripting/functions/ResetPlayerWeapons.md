---
id: ResetPlayerWeapons
title: ResetPlayerWeapons
description: Removes all weapons from a player.
tags: ["player"]
---

## Description

Removes all weapons from a player.

| Name     | Description                                   |
| -------- | --------------------------------------------- |
| playerid | The ID of the player whose weapons to remove. |

## Returns

1: The function was executed successfully.

0: The function failed to execute. This means the player specified does not exist.

## Examples

```c
public OnPlayerDeath(playerid, killerid, reason)
{
    // Remove the killer's weapons
    ResetPlayerWeapons(killerid);
    return 1;
}
```

## Notes

:::tip

To remove individual weapons from a player, set their ammo to 0 using SetPlayerAmmo.

:::

## Related Functions

- [GivePlayerWeapon](../functions/GivePlayerWeapon.md): Give a player a weapon.
- [GetPlayerWeapon](../functions/GetPlayerWeapon.md): Check what weapon a player is currently holding.
