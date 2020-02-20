# kj wishlist draft

As you may know, [DIM](https://github.com/DestinyItemManager/DIM) has a [community maintain wishlist](https://github.com/48klocs/dim-wish-list-sources). But this wishlist is just a bad smell, full of cartesian product. It's big and hard to read. This wishlist draft aims to refine it with a new format.

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

Check [json file](wishlist.json) for latest result.
Indent just for reading (can be smaller by removing indents).

## Schema

See [schema file](wishlist-schema.json) for more info.

## Thanks

- [48klocs](https://github.com/48klocs) - Create DIM Wishlist format
- [jaoryuken](https://github.com/marquesinijatinha) - Suggestions in draft writing
- [RaSSieL86](https://github.com/RaSSieL86) - Suggestions in draft writing

## License

[CC-BY-SA 4.0](LICENSE.md)
