<div align="center">

# ox_target

### Prodigy 4.0 RP Inspired Target System

**Made by Lunny Developments**

Built on [ox_target](https://github.com/communityox/ox_target) 1.17.3 · Free · `ox_lib` is the only dependency

[![Discord](https://img.shields.io/badge/Discord-Join%20us-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/yQednQCa6y)

**[Join our Discord](https://discord.gg/yQednQCa6y) for more quality scripts like this one.**

</div>

---

## What this is

A drop-in replacement for stock `ox_target` that ships the Prodigy 4.0 RP style targeting
interface: options fan out around a rotating reticle, you aim at one with the mouse
instead of clicking down a list, and the highlight follows the direction you point.

The Lua API is untouched, so every resource on your server that already targets keeps
working with no changes.

<div align="center">

<!-- Drop a gif or screenshot of the interface here -->

</div>

## Features

- **Directional targeting.** Options are laid out around the crosshair — the first one on
  top, the rest split into a left and a right column. You pick one by pointing at it,
  within a 45° window either side.
- **Fully standalone.** No framework core required, no paid dependency, no build step.
  `ox_lib` is the only thing it needs.
- **Drop-in compatible.** `api.lua`, `defaults.lua`, `debug.lua`, the `qtarget`
  compatibility layer and every framework adapter are byte-identical to upstream
  ox_target 1.17.3. Exports, events and convars all behave exactly as documented.
- **Resolution independent.** Everything scales from a single root rule, so the
  interface looks the same at 1080p and at 4K.
- **Self-contained UI.** Fonts are bundled — no CDN, no internet needed at runtime.

## Installation

1. Download the latest release and **name the folder `ox_target`.**

   In FiveM the export namespace is the folder name. Every script that calls
   `exports.ox_target:addBoxZone(...)` will only find this resource if the folder is
   called `ox_target`. Leaving it as `ox_target-main` will silently break every other
   resource that targets.

2. Remove your existing `ox_target` folder first.

3. Make sure `ox_lib` **3.30.0 or newer** starts before it:

   ```cfg
   ensure ox_lib
   ensure ox_target
   ```

That's it. No database, no config file, no npm install.

## Framework support

Group filters (`options.groups`) resolve through whichever of these is running:

| Framework | Supported |
|---|---|
| `ox_core` | Yes |
| `es_extended` | Yes |
| `qbx_core` | Yes |
| `ND_Core` | Yes |

If none of them are present, group filters are simply not applied and the resource still
works. Item filters (`options.items`) use `ox_inventory` when it is installed.

## Convars

| Convar | Default | Effect |
|---|---|---|
| `ox_target:defaultHotkey` | `LMENU` | Key that opens targeting |
| `ox_target:toggleHotkey` | `0` | `1` toggles targeting instead of holding the key |
| `ox_target:leftClick` | `1` | `1` grabs the cursor with LMB, `0` with RMB |
| `ox_target:drawSprite` | `24` | Max zone sprites drawn per frame, `0` disables |
| `ox_target:defaults` | `1` | `0` removes the built-in vehicle door options |
| `ox_target:debug` | `0` | `1` draws the raycast marker and entity outlines |

## API

Identical to upstream ox_target — the [official documentation](https://coxdocs.dev/ox_target)
applies as-is. Nothing was renamed, removed or added.

```lua
exports.ox_target:addBoxZone({
    coords = vec3(0.0, 0.0, 0.0),
    size = vec3(2, 2, 2),
    rotation = 0,
    options = {
        {
            label = 'Do the thing',
            onSelect = function() print('done') end,
        },
    },
})
```

## Building the interface

`web/dist/` is committed, so the resource runs straight out of the box. This is only
needed if you want to change the interface yourself:

```bash
cd web
npm install
npm run build
```

`web/src/styles/base.css` carries the root scale rule
(`font-size: min(0.83333333vw, 1.48148148vh)`) that keeps every measurement
resolution-independent — changing it rescales the entire interface.

## Credits

- Targeting logic by [Overextended / CommunityOx](https://github.com/communityox/ox_target), MIT licensed — see [LICENSE](LICENSE).
- Interface inspired by the Prodigy 4.0 RP target system.
- Packaged, rebuilt and maintained by **Lunny Developments**.

## License

MIT — see [LICENSE](LICENSE).

---

<div align="center">

**Want more scripts at this level of polish?**

### [discord.gg/yQednQCa6y](https://discord.gg/yQednQCa6y)

*Lunny Developments*

</div>
