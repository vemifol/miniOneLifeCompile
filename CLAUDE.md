# miniOneLifeCompile

Lightweight build harness for compiling the One Life game from source.

## Key Scripts

| Script | Purpose |
|--------|---------|
| `compile.sh` | Main build script — compiles the full game |
| `cloneRepos.sh` | Clones all required repositories |
| `getDependencies.sh` | Fetches pre-built dependency libraries |

## Build Process

1. Run `cloneRepos.sh` to clone `OneLife`, `OneLifeData7`, `minorGems`, and `dependencies`
2. Run `getDependencies.sh` to fetch pre-built libs (SDL 1.2, libpng, zlib, Discord SDK)
3. Run `compile.sh` to build

## Dependencies

Pre-built libs expected in `dependencies/`:
- `SDL-1.2.15` — windowing, input, audio
- `libpng-1.6.37` — PNG image handling
- `zlib-1.2.12` — compression (used for `CM` compressed messages and `MC` map chunks)
- `discord_game_sdk` — Discord rich presence
