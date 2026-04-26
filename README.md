# Codex Drift Circuit

A complete browser-based 3D arcade racing game built with Vite, TypeScript, Three.js, HTML, and CSS. Everything in the scene is procedural/custom geometry: cars, road, guardrails, banners, lights, trees, rocks, buildings, particles, smoke, skid marks, HUD, pause screen, and finish results.

## Features

- 3D procedural race track with guardrails, city/forest scenery, start gate, and road markings
- Player car with arcade driving physics, drifting, handbrake, off-road penalty, reset, and chase camera
- 4 AI opponent cars
- 3-lap race logic with countdown, lap timing, best lap, position tracking, and finish results
- Full-screen responsive UI and keyboard controls

## Controls

- W or Arrow Up: accelerate
- S or Arrow Down: brake / reverse
- A or Arrow Left: steer left
- D or Arrow Right: steer right
- Space: handbrake / drift
- R: reset car
- Esc or P: pause

## Launch on Windows

Install dependencies once:

```bash
npm install
```

Start the local game server:

```bash
npm run dev
```

Open the URL printed by Vite, usually:

```text
http://127.0.0.1:5173/
```

## Build for production

```bash
npm run build
```

The production files will be created in the `dist` folder.

## Project Structure

- `package.json` - Vite, TypeScript, and Three.js setup
- `index.html` - browser entry point
- `src/main.ts` - app bootstrap
- `src/game/Game.ts` - scene, race loop, camera, effects, lap logic
- `src/game/Car.ts` - procedural car model and vehicle state
- `src/game/AIController.ts` - opponent driving logic
- `src/game/Track.ts` - procedural track and environment
- `src/game/Physics.ts` - arcade driving physics
- `src/game/UI.ts` - menu, HUD, pause, finish UI
- `src/styles.css` - full-screen game and HUD styling
