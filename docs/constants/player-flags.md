# Player Flags

The following flags are available to check player status.

```lua
PLAYER_FLAGS.POISON
PLAYER_FLAGS.FIRE
PLAYER_FLAGS.ENERGY
PLAYER_FLAGS.DRUNK
PLAYER_FLAGS.MANA_SHIELD
PLAYER_FLAGS.PARALYSED
PLAYER_FLAGS.BATTLE
PLAYER_FLAGS.FREEZING
PLAYER_FLAGS.DAZZLING
PLAYER_FLAGS.CURSED
PLAYER_FLAGS.STRENGTHENDED
PLAYER_FLAGS.RED_SWORDS
PLAYER_FLAGS.PROTECTION_ZONE
PLAYER_FLAGS.BLEEDING
PLAYER_FLAGS.LESSER_HEX
PLAYER_FLAGS.INTENSE_HEX
PLAYER_FLAGS.GREATER_HEX
PLAYER_FLAGS.ROOTED
PLAYER_FLAGS.FEARED
PLAYER_FLAGS.GOSHNAR_1
PLAYER_FLAGS.GOSHNAR_2
PLAYER_FLAGS.GOSHNAR_3
PLAYER_FLAGS.GOSHNAR_4
PLAYER_FLAGS.GOSHNAR_5
PLAYER_FLAGS.MANA_SHIELD_NEW
```

Example code of casting `exana flam` when the player has burning condition.

```lua
auto(200)

local isburning = playerflag(PLAYER_FLAGS.FIRE)

if isburning and mp() >= 30 and vocation() == 'druid' then
	cast('exana flam') 
	wait(300, 500)
end
```
