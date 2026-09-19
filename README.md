# corex-zones

> Safe zones — no damage, no weapons, no PvP.

Part of the [COREX Framework](https://github.com/corex-zombies).

## Install

Drop the `corex-zones` folder into:
```
server-data/resources/[corex]/corex-zones/
```

Make sure it loads after `corex-core`:
```cfg
ensure corex-core
ensure corex-zones
```

## Public API

The current client exports are:

- `IsPlayerInSafeZone`
- `GetNearestSafeZone`
- `GetSafeZones`
- `GetSafeZoneDistance`

The server implementation also exposes safe-zone geometry to server-side
population/spawn policy code. Consumers should query Zones instead of copying
zone coordinates into their own resource.

## Update

Use a matching reviewed COREX build and merge `config.lua` changes. This local
workspace candidate is not documented here as a published release.

## Docs
📖 <https://corex-zombies.gitbook.io/corex-docs/reference/zones>

## Community
💬 <https://discord.gg/G95rtnb9sg>

## License
Released under the [MIT License](LICENSE).
