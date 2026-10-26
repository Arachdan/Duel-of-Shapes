# Duel of Shapes

**Duel of Shapes** is a local two-player arena game built with HTML, CSS, JavaScript, and the Canvas API. Two players choose their shape and battlefield, move across their respective arenas, and summon projectiles to defeat their opponent.

## Features

- **Local multiplayer:** Two players compete using a shared keyboard.
- **Shape selection:** Play as a circle or triangle, each with a distinct greater-summon ability.
- **Four battlefields:** Choose Mistwood, Sunscar, Tideglass, or Emberfall, each with its own color palette.
- **Combat system:** Launch lesser and greater summons with different cooldowns, movement speeds, and effects.
- **Resource management:** Summoning limits and recovery periods add a tactical element to combat.
- **Canvas-based rendering:** Characters, projectiles, arena boundaries, and player fields are drawn dynamically.
- **Built-in instructions:** Explore the game's lore, character types, and rules from the main menu.

## Controls

| Action | Player 1 | Player 2 |
|---|---|---|
| Move | `W` `A` `S` `D` | Arrow keys |
| Lesser summon | `Z` | `N` |
| Greater summon | `X` | `M` |

Movement is grid-based, and each movement or attack requires a separate key press.

## Gameplay

<img width="1280" height="615" alt="Screenshot 2026-10-26 at 18 38 34" src="https://github.com/user-attachments/assets/e95c3f64-b057-4a8c-9e99-bd1bd305965b" />

Each player starts with **100 health points**. Summons travel automatically toward the opposing arena and deal **20 damage** on a successful hit.

- **Lesser summons:** Faster to recharge, with a 1-second cooldown.
- **Greater summons:** Have a 3-second cooldown. Circle summons travel faster, while triangle summons launch an additional projectile into another lane.
- **Summoning limit:** After 10 summons, a player must wait 5 seconds before summoning again.
- **Projectile interactions:** Colliding opposing summons can be redirected into adjacent lanes.
- **Victory condition:** The first player to reduce their opponent's health to zero wins.

## Getting Started

<img width="871" height="537" alt="Screenshot 2026-10-26 at 18 40 07" src="https://github.com/user-attachments/assets/60c6d788-ea91-4289-ad4a-a94241d02ac7" />

1. Clone or download this repository.
2. Open `index.html` in a modern desktop browser.
3. Select a shape for each player and choose a battlefield.
4. Click **DUEL!** and start fighting.

No build tools, package installation, or external libraries are required.

## Tech Stack

- **HTML5** — Game structure and interface.
- **CSS3** — Layout, styling, selection states, and battlefield previews.
- **Vanilla JavaScript (ES6+)** — Game logic, input handling, cooldowns, collision detection, and entity management.
- **HTML Canvas API** — Real-time rendering of game entities and arena fields.
- **Animation and timing APIs** — `requestAnimationFrame()` for the game loop and `performance.now()` for cooldown tracking.

