# Blackline Contract

*Every shot is real. Every quota is a gamble.*

A hyperrealistic tactical extraction shooter built in **Unreal Engine 5.5** by **Tri-Op Studios**.

Blackline Contract blends bodycam-realistic gunplay with a co-op loot-and-survive loop: squad up with up to three friends, drop into a location, collect items, fight off monsters and enemies to survive, extract before time runs out, and pour everything into weapons and stats that scale infinitely.

## Status

This is a pre-seed stage project. The core loop — deploy, collect, survive, extract, upgrade — is playable end-to-end in Unreal Engine 5.5.

## What's in this repository

This repo is a **partial, source-level snapshot** of the project, not a fully buildable clone. It contains:

- `BlacklineContract.uproject` — the project descriptor
- `Config/` — project configuration (engine, editor, input, game defaults)
- `Content/Demo.umap` — the current demo level

### What's intentionally excluded

The full project's `Content/` folder is ~29GB, almost entirely third-party Fab/Unreal Marketplace asset packs (environment kits, character bundles, AI behavior packs) rather than original work. Those packs are excluded from this repository for two reasons:

1. **Licensing** — marketplace EULAs generally restrict redistributing the raw asset files outside of a compiled game, which a public source repo would violate.
2. **Size** — this repository does not use Git LFS, and 29GB of binary `.uasset`/`.umap` data isn't practical to version without it.

Also excluded: `Binaries/`, `DerivedDataCache/`, `Intermediate/`, and `Saved/` — standard Unreal build/cache output that's regenerated locally and should never be versioned.

As a result, `Content/Demo.umap` will not open correctly without separately reacquiring the referenced marketplace packs. See `.gitignore` for the exact exclusion list.

## Engine

Unreal Engine **5.5**, Windows target platform.

## Team

Built by Tri-Op Studios.

## License

All rights reserved. This repository is shared for portfolio and review purposes; it is not licensed for reuse, redistribution, or derivative works.
