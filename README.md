# minecraft-server-pack

Combined resource pack for a small Paper 26.1.2 survival server, served through GitHub Pages
so the server can push it to every player via `resource-pack=` in `server.properties`.

Download: https://ardazeybek-dev.github.io/minecraft-server-pack/pack.zip

## Contents

| Part | Source | License |
|---|---|---|
| Backpack models and textures | [Vanilla Backpacks](https://modrinth.com/datapack/vanilla-backpacks) by Eclipse Studios, v1.3.5 | Apache-2.0 |
| Elytra chestplate models | [Elytra Chestplates](https://modrinth.com/datapack/elytra-chestplates), v1.6.0 | MIT |

Both packs are unmodified; only `pack.mcmeta` was merged. Resource pack format 84.

## Updating

1. Replace `pack.zip`, commit and push.
2. Put the new SHA-1 (`sha1sum pack.zip`) into `resource-pack-sha1` in `server.properties`.

## Pitfalls

- The server sends a single resource pack, so every pack that needs client textures has to be merged into this one zip.
