# Cadence

**Pet Rhythm Beat** — Rhythm game where pets dance on synchronized beats using Motion clips.

Part of the [ComputerPets](https://github.com/RicheyWorks/computerpets) universe. Map: [computerpets-ecosystem](https://github.com/RicheyWorks/computerpets-ecosystem).

> Status: **design scaffold**. Gameplay contract is frozen. Engine choice is the one in the brief. Implementation comes next.

## Loop

Motion already bakes walk cycles. Cadence bakes dance: hit windows keyed to species size (frog vs panda). Misses drop mood slightly, never HP.

## Genre & engine

- Genre: **Rhythm minigame**
- Engine: **Godot**
- Stack: Godot 4 · AnimatedSprite · Motion dance clips · Web Audio-equivalent in Godot
- Default surface: `Godot editor`

## How you play

1. Pick a track + pet.
2. Notes from official chart pack (SDK can add).
3. Full combo = treat. Fail = embarrassed emote.
4. Twitch can send emoji notes later.

## Talks to

- computerpets-motion
- computerpets-vox
- computerpets-encore
- computerpets-quests

## Failure doctrine

Audio drift → recalibrate, do not punish. No GPU → lower FPS, same windows. Custom track without chart → refuse.

Canon rules that never yield:

- 210 living kinds. No illegal hybrids.
- Overlay pets can get tired, sick, or hide. Tokens are not burned by a minigame.
- Desktop walk stays the main quest. Closing Cadence must leave Rui walking.

## Layout

```
computerpets-cadence/
  README.md
  LICENSE
  docs/DESIGN.md
  src/                implementation lands here
```

## Run (Windows)

```powershell
godot --path . ; F5
```

Meet Rui first via the [flagship start-here](https://github.com/RicheyWorks/computerpets/blob/main/docs/START-HERE.md). This game is optional.

## License

MIT. See [LICENSE](LICENSE).

---

*Two hundred ten living kinds. Keep them so a line does not go quiet.*
