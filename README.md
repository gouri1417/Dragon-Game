# Dragon-Game

## How the Game Works

### Objective
Control the dragon and collect magic orbs to increase your score. Avoid obstacles and self-collisions (if enabled). The game ends when the dragon collides with a hazard or when the player quits.

### Setup
- The game runs in the browser on an HTML `<canvas>` (default size: **600×600 px**).
- The dragon starts at the center of the canvas, facing right.
- Magic orbs (food) spawn at random positions on the canvas.

## Gameplay Mechanics

### 1. Dragon Movement
- The dragon **follows the mouse**: it continuously moves toward the current mouse position.
- Movement speed is constant by default and can scale slightly with score (optional toggle).
- Screen edges can be set to:
  - **Wrap-around** (exit one side, appear on the opposite), or
  - **Solid walls** (hitting the boundary ends the game).

### 2. Collecting Orbs (Food)
- Orbs appear randomly as small circles.
- When the dragon’s head overlaps an orb, it **collects** it.

### 3. Growing & Scoring
- On each orb collected, the **score increases by 1** (or a configurable amount).
- Optionally, the dragon’s tail grows by adding a new segment (snake-like) to make control more challenging.

### 4. Game Over Conditions
- Collision with **hazards/obstacles** (if enabled).
- **Self-collision** (if tail growth mode is on).
- **Boundary collision** when wrap-around is disabled.

## Features

### Color Scheme
- **Dragon**: gradient gold → orange (configurable in `styles.css`).
- **Orbs**: teal/blue.
- **Background**: dark canvas grid for depth.

### User Interaction
- **Mouse** controls direction.
- **P** – Pause / Resume.
- **R** – Restart.
- **M** – Toggle music/SFX (if assets provided).
- On-screen HUD shows **Score** and **High Score** (stored via `localStorage`).

### Polish
- Smooth movement with `requestAnimationFrame`.
- Collision detection using circle/rect math.
- Responsive canvas (fits window while keeping aspect ratio).

## Future Improvements
- Difficulty scaling (speed increases every few points).
- Power-ups: shield, slow-time, magnet for orbs.
- Boss/enemy sprites with simple AI.
- Themed levels and parallax backgrounds.
- Touch controls for mobile devices.
- Online leaderboard integration.

## Installation

### Requirements
Before running the game, make sure you have:
- A **modern browser** (Chrome, Edge, Firefox, Safari).
- (Optional) **VS Code** with the **Live Server** extension for auto-reload.

### Installation Steps
1. **Clone the Repository**

   Clone the Repository: git clone https://github.com/grishma-gedela/Snake-Game.git


