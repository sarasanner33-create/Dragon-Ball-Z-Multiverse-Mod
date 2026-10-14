# Dragon-Ball-Z-Multiverse-Mod

A modular, mod-friendly 3D multiverse action game prototype. This repository is a starter scaffold, not a finished game.

## Project goals
- Third-person movement and arena combat
- Character definitions, abilities, transformations, and progression
- Multiple original worlds, arenas, quests, and enemies
- Data-driven mod packages with validation
- PC-first development; Android and console are later targets

## IP and assets
This scaffold contains no official Dragon Ball assets. For public distribution, use original characters, names, art, audio, models, and lore unless you have the required permissions. The repository name is a working title and is not an indication of affiliation.

## Suggested engine
Unreal Engine 5, using C++ for core systems and Blueprint for iteration. Keep the core runtime authoritative and treat mod packages as untrusted input.

## Repository layout
See [`docs/PROJECT_STRUCTURE.md`](docs/PROJECT_STRUCTURE.md).

## Getting started
1. Install Git and Unreal Engine 5.
2. Create an Unreal C++ project named `MultiverseMod` in this repository, or place the generated `.uproject` and `Source/` files here.
3. Enable Enhanced Input and the plugins you actually need.
4. Copy `Config/ModSchema/` examples into a test mod under `Mods/`.
5. Follow [`docs/SETUP.md`](docs/SETUP.md).

## Current status
Planning scaffold only. Gameplay systems, editor tooling, packaging, and platform support must be implemented and tested in Unreal Engine.

## License
Choose a license after deciding whether this is a personal prototype or a distributable project. Do not add third-party assets without checking their licenses.
