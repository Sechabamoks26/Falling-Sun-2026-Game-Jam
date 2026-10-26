# Falling Sun

> *The sun is dying. Catch its light before it hits the dark.*

**Falling Sun** is a fast arcade survival game for the **Falling Sun 2026 Game Jam** (Game Development, Track 01, 24-25 October 2026). Slide your lantern under the falling sun, catch the golden shards that keep it alive, and dodge the shadows. When the dark gets too thick, charge your Pulse and break the Eclipse.

| | |
|---|---|
| **Genre** | Arcade, survival, score attack |
| **Players** | 1 |
| **Platforms** | Any modern browser (desktop and mobile), plus a Unity version |
| **Play now** | `https://<your-username>.github.io/<repo-name>/` |
| **Team** | `<team name>`: `<member names>` |



## Quick start

**Play in the browser:** open the link above, or open `index.html` (or `falling-sun.html`) from this repo in Chrome, Edge, Firefox or Safari. No install, no server and no internet connection are needed once you have the file.

**Run the Unity version:** see [`unity/README_UNITY.md`](unity/README_UNITY.md).

## How to play

1. **Move** your lantern left and right to line it up under falling objects.
2. **Catch gold shards.** Each one refills the sun's light and raises your score. Catch several in a row to build a streak: every 5 in a row adds 1 to your multiplier, up to x8.
3. **Dodge the shadows.** A hit drains a big chunk of light and resets your streak. Missing a shard costs a little light too.
4. **Charge and fire your Pulse.** Catching shards fills the Pulse bar. When it is full, trigger it to destroy nearby shadows, pull in shards and damage bosses.
5. **Break the Eclipse.** A boss appears at 40 seconds, and again about 50 seconds after each defeat. It fires fans of shadows at you, and only a Pulse can hurt it. Later bosses are tougher.
6. **Survive.** The sun's light constantly drains, faster as time passes. When it hits zero, the light goes out.

Your best score is saved in your browser.

## Controls

| Action | Desktop | Mobile |
|---|---|---|
| Move the lantern | Mouse, Arrow keys, or A / D | Drag your finger |
| Fire the Pulse | Space | Tap the PULSE button (bottom right) |
| Start / restart | Enter, Space or click | Tap |
| Mute sound | M | - |

## Features

- **Streak and multiplier scoring** that rewards clean play.
- **Pulse mechanic** that turns defence into an attack and is the only way to beat bosses.
- **The Eclipse boss wave** with sweeping movement, fan-shaped attacks and scaling health.
- **Rising difficulty:** faster falls, quicker spawns and more shadows over time.
- **Live-reactive visuals:** the sun shrinks and dims as your light drops, and the sky darkens with it. Screen shake, particles and score pop-ups give hits and catches some weight.
- **Fully synthesized audio:** the looping music and every sound effect are generated in code, with a catch sound that rises in pitch with your streak. The music speeds up as the game gets harder.
- **Touch and keyboard support** with a responsive layout.

## Tech

| Version | Stack |
|---|---|
| **Web** | A single HTML file with vanilla JavaScript, Canvas 2D and the Web Audio API. No libraries, frameworks, images or external requests. |
| **Unity** | C# in one script (`FallingSun.cs`). Camera, sprites, audio and HUD are all created in code. Works with the old Input Manager, the new Input System or both. |

## Repository layout

```
index.html          Web build (entry point for GitHub Pages)
falling-sun.html    Same build under its original name
README.md           This file
cover.png           Cover image (
unity/
  README_UNITY.md   Unity setup and build steps
  Assets/Scripts/FallingSun.cs
```

## Credits

- Game design, code and audio synthesis: `Moksnation`
- Built with assistance from Gemini (Google)
