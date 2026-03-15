# PULSE

> **NEURAL EXTRACTION PROTOCOL · 2041**

PULSE is a minimalist arcade reflex game set in a cyberpunk dystopia. You are FIZZ — a rogue signal trying to escape a collapsing neural network before the system erases you.

Navigate your operator through an endless stream of expanding rings. Time your orbits. Pass through the gap. Don't get hit. Reach 100 rings and escape.

---

## Play

🎮 **[Play on GitHub Pages](https://syscolor.github.io/PULSE/)**

---

## Screenshots

![Menu Principal](https://github.com/user-attachments/assets/2b24fd4d-4dc1-4e4b-a134-ba34d56c6cd1)
![Gameplay](https://github.com/user-attachments/assets/42b40138-cbf6-4512-9b75-d6503d88a70c)
![Dark Mode](https://github.com/user-attachments/assets/05d45364-b2f5-4afc-8060-400ef23ff53b)
![Neural Store](https://github.com/user-attachments/assets/afb9cbad-476e-485f-ba36-2393f4e3d0d2)
![Conquistas](https://github.com/user-attachments/assets/18d8b795-3b5a-4d37-b8ac-07a8027a5a2e)

---

## Gameplay

Rings expand outward from the center of the screen. Each ring has a gap — pass through it to score. Miss the gap and you lose a life. Lose all four lives and the signal dies.

The game escalates automatically through 5 difficulty tiers:

| Tier | Description |
|---|---|
| `INIT` | Slow rings, wide gaps. Learn the system. |
| `TRACE` | Speed increases. Gaps tighten. |
| `BREACH` | Spinning rings appear. Gaps shrink further. |
| `CRITICAL` | Shrinking gaps. Higher pressure. |
| `HELL_SYNC` | Maximum speed. Minimum mercy. |

Every 25 rings, the game pauses and offers a **Signal Upgrade** to choose from — making each run unique.

As you pass rings, you unknowingly compose a **full piano melody** of 100 notes. It builds, peaks, and resolves by ring 100.

---

## Features

- **Solo Extraction** — reach 100 rings to trigger the escape sequence
- **Signal Upgrades** — roguelike upgrade system exclusive to Solo mode
- **Neural Duel** — local 1v1 split-screen with sabotage mechanics
- **5 difficulty tiers** that escalate automatically based on score
- **Procedural melody** — each ring pass plays the next note of a composed piano piece
- **Musical peak at ring 40** — signal surge, volume spike, dissonant chord
- **Visual climax at rings 50–75** — the background pulses with the music
- **Skin system** with Neural Store — 4 operators + 1 secret, P1 and P2 equipped independently
- **Robot faces** — each operator has a unique animated eye and body shape
- **Neural Credits** — earned by playing, spent in the store
- **Combo multiplier** — chain rings for score bonuses
- **Shield overflow** — collecting a second shield converts to +1 life
- **Near-miss detection** — canvas flash + particles when you barely survive
- **Warning ring** — ghost arc previews incoming ring gap position
- **Dot trail** — motion trail follows your operator at speed
- **Achievement system** — 8 unlockable achievements tracked across sessions
- **Dark mode** — toggleable via `[ ◑ ]` button, persisted across sessions
- **Contextual narrative** — dialogue reacts to what happens in real time
- **Procedural soundtrack** — 6 unique ambient tracks (3 menu + 3 battle), no audio files
- **Terminal / Cheat codes** — secret codes accessible in-game
- **First-time tutorial** — gentle hints on first play, never shown again
- **CrazyGames SDK** integrated and compliant
- **Full mobile support** with touch controls
- **Responsive scaling** — adapts to any screen size

---

## Signal Upgrades *(Solo only)*

Every 25 rings the game pauses and offers 3 random upgrades to choose from. Each run is different — upgrades never repeat within a run and stack across choices. Use `HOGHOG` in the terminal to trigger an upgrade screen on demand (4 uses per run).

| Category | Upgrade | Effect |
|---|---|---|
| ⚡ Mobility | `OVERCLOCK` | Move 25% faster |
| 〜 Mobility | `DRIFT` | Less friction — smoother orbit |
| ◎ Mobility | `SNAP ORBIT` | Orbit switch is instant |
| ▮ Survival | `EXTRA LIFE` | +1 life (max 5) |
| ✦ Survival | `SECOND CHANCE` | Survive one fatal hit |
| ◈ Survival | `GHOST SHIELD` | Next hit is ignored |
| ⬡ Score | `DOUBLE CREDITS` | Neural credits earned ×2 this run |
| × Score | `COMBO EXTEND` | Combo timer lasts 50% longer |
| ◉ Score | `RING MAGNET` | Gap size increased slightly |
| ★ Style | `OVERCHARGE` | Trail is longer and brighter |
| ◐ Style | `NEON` | Rings glow intensely |

---

## Operators

| Operator | Body | Eye | Color | Price | Notes |
|---|---|---|---|---|---|
| **FIZZ** | Rounded pill | White bar, blinks | Orange `#c84000` | Free | Default P1, P2 default |
| **SERAPH** | Sharp rectangle | Cold slit, never blinks | Blue `#0070aa` | 150 ⬡ | |
| **VOID** | Diamond | Pulsing purple eye | Purple `#660099` | 300 ⬡ | Unlocks exclusive ending |
| **YAN** | Rectangle | RGB bar | Chromatic | 500 ⬡ | Full RGB rings |
| **MEQUINTOSHI** | Macintosh 128K | CRT screen with pixel face | Beige `#c8b89a` | Secret | Unlock with terminal code |

Playing as VOID and completing Solo Extraction triggers a unique ending sequence.

---

## Controls

| Action | P1 | P2 |
|---|---|---|
| Move | `A` / `D` | `←` / `→` |
| Orbit inward | `SPACE` | `SHIFT` |
| Orbit outward | `S` | `↓` |
| Pause | `ESC` | — |
| Mute | `M` | — |

---

## Achievements

| Icon | Name | Condition |
|---|---|---|
| ◈ | `GHOST` | Pass 5 rings without moving |
| ✦ | `FLAWLESS` | Complete extraction with full HP |
| ⚡ | `HELL SURVIVOR` | Pass 20 rings in HELL_SYNC |
| ◉ | `VOID TOUCHED` | Play as the VOID operator |
| × | `COMBO MASTER` | Reach ×10 combo |
| ▣ | `UNTOUCHABLE` | Pass 15 rings in a row |
| 💀 | `SERIOUSLY?` | Die 100 times |
| ↯ | `ROTOR` | ??? |

All achievements are tracked across sessions via `localStorage`.

---

## Soundtrack

PULSE has 6 fully procedural ambient tracks built with Web Audio API — no audio files, no external dependencies. All music is synthesized in real time.

**Menu (3 tracks, random rotation):**
- Track 1 — C418 style: long silences, sparse piano, contrabass, metallic bell tones
- Track 2 — Chamber piano: Cm arpeggios, light kick at 70bpm, crystal bells
- Track 3 — Abandoned server room: Am piano, high celesta, wind layers

**Battle (3 tracks, random rotation):**
- Track 1 — HFF Winter: glockenspiel, cutting wind, ice drone, D minor
- Track 2 — Häggström style: individual Am notes, very long sustain, slow bass
- Track 3 — Sweden style: Cm arpeggios played one note at a time, cathedral reverb, 7–15s silences between chords

Each ring pass triggers the next note of a 100-note piano melody structured in 4 phrases: intro → development → climax → resolution.

---

## Terminal Codes

Open the terminal with `[ TERMINAL ]` button or during gameplay. Type a code and press `Enter`.

| Code | Effect |
|---|---|
| `BERRYBURN` | +1000 Neural Credits |
| `SKIP` | Jump to ring 99 |
| `1337` / `ROTOR` | Force HELL_SYNC |
| `PULSE2` | Restore all lives, exit hell mode |
| `GHOST` | Invincibility |
| `MATRIX` | Particle burst |
| `ONIX` | Unlock all achievements |
| `HOGHOG` | Force upgrade screen — 4 uses per run *(Solo only)* |
| `MESSIAS` | Unlock secret operator |
| `LISO LISO LISO` | Force maximum performance mode |
| `SEQUINHO` | Restore auto performance mode |

---

## Tech

- Pure **HTML + CSS + JavaScript** — single file, zero dependencies, zero build tools
- **Web Audio API** — 6 ambient tracks, procedural melody, hit sounds, victory fanfare, all synthesized
- **Canvas 2D** — all rendering, particles, rings, robot faces, dot trail
- **localStorage** — credits, skins, achievements, dark mode, best score, deaths, play history
- **CrazyGames SDK** — gameplayStart/Stop, mute handler, ad integration

---

## Structure

```
PULSE/
├── index.html      # entire game — single file
├── README.md
└── LICENSE
```

---

## License

© 2026 Marzio. All rights reserved.  
Original game created by Marzio. Unauthorized copying or redistribution is prohibited.
