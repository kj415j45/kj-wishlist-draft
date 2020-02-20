# kj wishlist draft

As you may know, [DIM](https://github.com/DestinyItemManager/DIM) has a [community maintain wishlist](https://github.com/48klocs/dim-wish-list-sources). But this wishlist is just a bad smell, full of cartesian product. It's big and hard to read. This wishlist draft aims to refine it with a new format.

## What's new in this format?

- Tag your god roll groups for faster searching.
- Pick not only perks, but also masterwork and mod.
- Pick more than one perk at each slot and accurate match them. (Introduced in Season of Dawn level 92)

## Difference between DIM ver and kj ver

I just pick some perks that I prefered.

### DIM ver

```
//Tranquility PvE
//notes:PvE
dimwishlist:item=1170891373&perks=4090651448,106909392,3300816228,1771339417,384158423
dimwishlist:item=1170891373&perks=2467967826,106909392,3300816228,1771339417,384158423
dimwishlist:item=1170891373&perks=1840239774,106909392,3300816228,1771339417,384158423
dimwishlist:item=1170891373&perks=1392496348,106909392,3300816228,1771339417,384158423
dimwishlist:item=1170891373&perks=1482024992,106909392,3300816228,1771339417,384158423
dimwishlist:item=1170891373&perks=4090651448,1087426260,3300816228,1771339417,384158423
dimwishlist:item=1170891373&perks=2467967826,1087426260,3300816228,1771339417,384158423
dimwishlist:item=1170891373&perks=1840239774,1087426260,3300816228,1771339417,384158423
dimwishlist:item=1170891373&perks=1392496348,1087426260,3300816228,1771339417,384158423
dimwishlist:item=1170891373&perks=1482024992,1087426260,3300816228,1771339417,384158423
... (total line 482. 42,150 Bytes)
```

### kj ver

```json
{
    "$schema": "./wishlist-schema.json",
    "1170891373": [{
        "name": "Tranquility",
        "description": "PvE pick",
        "tags": ["y3", "s8", "pve"],
        "accurate_match": false,
        "perks": {
            "slot1": [4090651448, 2467967826, 1840239774, 1392496348, 1482024992],
            "slot2": [106909392, 1087426260, 3230963543, 3177308360],
            "slot3": [3300816228, 2869569095, 1168162263],
            "slot4": [1771339417, 1354429876, 2551157718],
            "masterworks": [384158423, 186337601],
            "mods": [3336648220, 2788909693]
        }
    }]
}
```

Indent just for reading (604 Bytes, can be smaller if remove indents).

## Schema

See [schema file](wishlist-schema.json) for more info.

## License

[CC-BY-SA 4.0](LICENSE.md)
