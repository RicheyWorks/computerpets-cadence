# Cadence design

Implement against this file, not folklore.

## Identity

- Product: **Cadence**
- Repo: `computerpets-cadence`
- Idea: Pet Rhythm Beat
- Genre: Rhythm minigame
- Engine: Godot
- Surface: `Godot editor`

## Loop

Motion already bakes walk cycles. Cadence bakes dance: hit windows keyed to species size (frog vs panda). Misses drop mood slightly, never HP.

## Play beats

- Pick a track + pet.
- Notes from official chart pack (SDK can add).
- Full combo = treat. Fail = embarrassed emote.
- Twitch can send emoji notes later.

## Neighbors

- computerpets-motion
- computerpets-vox
- computerpets-encore
- computerpets-quests

## Failure doctrine

Audio drift → recalibrate, do not punish. No GPU → lower FPS, same windows. Custom track without chart → refuse.

## Hard rules

1. Minigames cannot mint or burn NFTs by themselves (Minter is the write path).
2. Stats come from lived overlay care + Dojo caps, not cash shop.
3. Species kits stay inside Lore. Illegal hybrids never spawn.
4. Fail soft: the desktop overlay process is not this process.
